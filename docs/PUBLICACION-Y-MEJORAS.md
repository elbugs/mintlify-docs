# Publicación de la documentación y mejoras

Este documento describe **qué más se puede agregar** a la documentación, **dónde publicarla** y cómo **automatizar** la subida a help.hotelgest.com (Intercom).

---

## 1. Qué más podemos agregar a la documentación

### Contenido
- **Capturas de pantalla**: Añadir imágenes clave (login, dashboard, calendario, detalle de reserva, informes) en cada sección para guía visual.
- **Vídeos cortos**: Enlaces a vídeos “cómo hacer X” (por ejemplo: crear reserva, hacer check-in, exportar informe).
- **FAQ por módulo**: Preguntas frecuentes al final de cada documento (ej. “¿Cómo cancelo una reserva?”).
- **Casos de uso**: Pequeños escenarios paso a paso (ej. “Llegada de un grupo”, “Check-out con factura pendiente”).
- **Glosario**: Archivo `docs/GLOSARIO.md` con términos (pcode, OTA, régimen, proforma, etc.).
- **Changelog de documentación**: Archivo que indique qué se ha añadido o cambiado en la doc por versión/fecha.

### Formato y estructura
- **Versión y fecha**: En cada doc o en el README, indicar “Última actualización: DD/MM/AAAA” y versión de la app si aplica.
- **Enlaces internos**: Revisar que todos los enlaces entre documentos (por ejemplo “Ver [Configuración](11-configuracion.md)”) funcionen.
- **Índice al inicio**: En documentos largos, un pequeño índice con anclas para ir a cada sección.

---

## 2. Dónde publicar la documentación

### Opción A: Intercom (help.hotelgest.com) — recomendado
- La ayuda actual ya está en **Intercom** (help.hotelgest.com).
- Se puede conectar con la **API de Intercom** para crear/actualizar artículos en el Help Center.
- Los artículos se pueden subir como **borrador** (`state: "draft"`) para revisarlos antes de publicar.
- Ventajas: mismo sitio que el soporte, búsqueda unificada, mismo branding.

### Opción B: Repositorio como “single source of truth”
- Mantener los `.md` en **uni-backend/docs/** (o en un repo solo de docs).
- Publicar desde ahí:
  - A Intercom (con el script que se describe más abajo), o
  - A cualquier otro sitio (GitHub Pages, GitBook, Docusaurus, etc.) si en el futuro se cambia de herramienta.

### Opción C: GitHub Pages / GitBook / Docusaurus
- Generar un sitio estático desde los Markdown y publicarlo en una URL (por ejemplo `docs.hotelgest.com`).
- Útil si se quiere una documentación pública separada del Help Center de Intercom.

---

## 3. Automatización: documentar y subir en cada cambio

### 3.1 Mantener la doc al día con el desarrollo
- **Convención en commits**: Incluir en las PRs que añadan funcionalidad nueva o cambien flujos la actualización (o creación) del `.md` correspondiente en `docs/`.
- **Checklist en PR**: Añadir en la descripción de la PR algo como: “Si cambia algo visible para el usuario, ¿se ha actualizado la documentación en `docs/`?”.
- **Script opcional**: Un script que recorra módulos/rutas y genere un índice o esqueleto de doc (avanzado; se puede plantear más adelante).

### 3.2 Subir automáticamente a Intercom
- **Script incluido en el repo**: `scripts/sync-docs-to-intercom.js` (ver más abajo).
  - Lee los `.md` de `docs/`.
  - Convierte Markdown → HTML.
  - Crea o actualiza artículos en Intercom vía API, en estado **draft**.
- **Cuándo ejecutarlo**:
  - **Manualmente**: cuando alguien quiera refrescar el Help Center: `npm run docs:sync-intercom`.
  - **En CI (recomendado)**:
    - En cada push a `main` (o a una rama `docs`) que toque archivos en `docs/`, ejecutar el script.
    - Ejemplo **GitLab CI**: job que solo corra si hay cambios en `docs/**`, con `INTERCOM_ACCESS_TOKEN` e `INTERCOM_AUTHOR_ID` como variables secretas del proyecto:
      ```yaml
      sync-docs-intercom:
        stage: deploy
        image: node:18
        rules:
          - if: $CI_COMMIT_BRANCH == "main"
            changes: [docs/**]
        script:
          - npm ci
          - npm run docs:sync-intercom
        variables:
          INTERCOM_ACCESS_TOKEN: $INTERCOM_ACCESS_TOKEN
          INTERCOM_AUTHOR_ID: $INTERCOM_AUTHOR_ID
      ```
    - En **GitHub Actions** se puede usar `paths: ['docs/**']` en el trigger y definir los secrets en el repo.

Así, “cada cosa nueva que se desarrolle” puede:
1. Incluir los cambios en los `.md` en el mismo PR.
2. Al fusionar (y si el pipeline está configurado), correr el script y subir los artículos a Intercom en borrador para revisión.

---

## 4. Conexión con la API de Intercom para subir artículos

Intercom expone una **REST API** para el Help Center (Knowledge Base):

- **Crear artículo**: `POST https://api.intercom.io/articles`
- **Autenticación**: `Authorization: Bearer <ACCESS_TOKEN>`
- **Cabecera**: `Intercom-Version: 2.14` (o la versión que use vuestra app).
- **Campos relevantes**:
  - `title` (obligatorio)
  - `author_id` (obligatorio): ID de un teammate en Intercom.
  - `body`: contenido en **HTML**.
  - `description`: resumen del artículo.
  - `state`: `"draft"` (borrador) o `"published"` (publicado).
  - `parent_id` y `parent_type`: para organizar en una colección/sección.

El **Access Token** no es el mismo que el App ID del chat: es un **token de API** que se genera en Intercom en **Developer Hub > Configure > Authentication** (o en la configuración del workspace). Ese token debe guardarse como secreto (por ejemplo `INTERCOM_ACCESS_TOKEN` en CI/variables de entorno) y no commitearse.

En este repo tenéis un **script** que hace la sincronización desde `docs/` a Intercom en borrador; ver el README del script y la sección siguiente.

---

## 5. Uso del script de sincronización con Intercom

- **Script**: `scripts/sync-docs-to-intercom.js`
- **Documentación del script**: Ver el comentario al inicio del archivo y `docs/README.md` (sección “Sincronización con Intercom”).
- **Variables de entorno**:
  - `INTERCOM_ACCESS_TOKEN`: token de API de Intercom (Help Center).
  - `INTERCOM_AUTHOR_ID`: ID del autor (teammate) en Intercom.
  - Opcional: `INTERCOM_COLLECTION_ID` para agrupar los artículos en una colección.

Con eso se puede:
- Publicar en **borrador** de forma automática cada vez que se actualice la doc y se ejecute el script (manual o en CI).

Si queréis que los artículos se publiquen directamente sin revisión, el script puede aceptar un flag (por ejemplo `--publish`) para usar `state: "published"` en lugar de `"draft"`.
