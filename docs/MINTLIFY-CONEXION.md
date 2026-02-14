# Conectar Mintlify y subir la documentación

Esta guía explica cómo conectar Mintlify con el repositorio Git y desplegar la documentación. **El contenido de la doc vive en Bitbucket (uni-backend)** y se sincroniza al repo de Mintlify en **GitHub** ([elbugs/mintlify-docs](https://github.com/elbugs/mintlify-docs)), que es el que Mintlify usa para desplegar.

---

## 0. Repo Mintlify en GitHub (elbugs/mintlify-docs)

Mintlify solo soporta **GitHub** y **GitLab**, no Bitbucket. Por eso:

- **Origen del contenido:** Bitbucket (este repo, uni-backend): `docs.json`, carpeta `docs/`, y los `.swagger.json`.
- **Repo que conectas en Mintlify:** GitHub [elbugs/mintlify-docs](https://github.com/elbugs/mintlify-docs).

Cada vez que cambies la documentación en Bitbucket, hay que **sincronizar** ese contenido al repo de GitHub. Para eso sirve el script `scripts/sync-docs-to-mintlify-github.js` (ver sección 6b).

---

## 1. Crear cuenta y proyecto en Mintlify

1. Entra en [mintlify.com](https://mintlify.com) y crea una cuenta (o inicia sesión con GitHub).
2. En el [dashboard de Mintlify](https://dashboard.mintlify.com), crea un **nuevo proyecto** (o usa uno existente).
3. Cuando te pida conectar un repositorio, puedes hacerlo en el paso siguiente.

---

## 2. Instalar la GitHub App de Mintlify

1. Ve a **Organization settings** → **GitHub App** en el dashboard:  
   [dashboard.mintlify.com/settings/organization/github-app](https://dashboard.mintlify.com/settings/organization/github-app)
2. Instala la **Mintlify GitHub App** en tu organización o cuenta de GitHub.
3. Al instalarla, concede acceso **solo al repositorio** donde está esta documentación (por ejemplo `uni-backend`).
4. Acepta los permisos que pide: lectura de metadatos, lectura/escritura de PRs, deployments, código y checks.

---

## 3. Conectar el repositorio en Mintlify

Conecta el **repo de GitHub** (no el de Bitbucket):

1. En el dashboard de Mintlify, ve a **Git Settings**:  
   [dashboard.mintlify.com/settings/deployment/git-settings](https://dashboard.mintlify.com/settings/deployment/git-settings)
2. Conecta el repositorio de GitHub:
   - **Organization / User**: `elbugs`
   - **Repository**: `mintlify-docs`  
     (https://github.com/elbugs/mintlify-docs)
   - **Branch**: `main` (la rama desde la que Mintlify desplegará).

### Si el repo es un monorepo (varios proyectos en uno)

Si la documentación está dentro de una subcarpeta (por ejemplo `uni-backend` dentro de un repo único):

1. Activa el toggle **Set up as monorepo**.
2. En **Documentation path** indica la ruta relativa hasta la carpeta que contiene `docs.json` (por ejemplo `uni-backend`), **sin** barra final.
3. Guarda los cambios.

### Si el repo es solo el backend (uni-backend)

Si el repositorio conectado es directamente el que tiene `docs.json` en la raíz y la carpeta `docs/`:

- No actives monorepo; deja el path vacío. Mintlify usará la raíz del repo.

---

## 4. Dominio y publicación

- Por defecto Mintlify te da una URL tipo `tunombre.mintlify.app`.
- Para usar un dominio propio (p. ej. `docs.hotelgest.com`): **Settings** → **Custom domain** en el dashboard y sigue las instrucciones de DNS.

---

## 5. Probar en local (opcional)

Para previsualizar la doc antes de subir:

```bash
# Desde la raíz del repo (donde está docs.json)
npx mintlify dev
```

Se abrirá una vista previa en `http://localhost:3000`. Si da error, instala el CLI globalmente:

```bash
npm i -g mintlify
mintlify dev
```

---

## 6. Flujo de trabajo: Bitbucket → GitHub → Mintlify

### 6a. Subir cambios en Bitbucket (origen)

Cuando edites `docs/` o `docs.json` en uni-backend:

```bash
git add docs.json docs/
git commit -m "$(git branch --show-current): actualizar documentación"
git push origin $(git branch --show-current)
```

Eso deja la documentación guardada en Bitbucket. Para que Mintlify se actualice, hay que sincronizar al repo de GitHub (paso 6b).

### 6b. Sincronizar al repo de Mintlify en GitHub

1. **Clona el repo de Mintlify** (solo la primera vez) en una carpeta al mismo nivel que uni-backend, por ejemplo:
   ```bash
   cd /ruta/donde/está/uni-backend
   git clone https://github.com/elbugs/mintlify-docs.git ../mintlify-docs
   ```

2. **Ejecuta el script de sincronización** desde la raíz de uni-backend:
   ```bash
   MINTLIFY_REPO_PATH=../mintlify-docs npm run docs:sync-mintlify
   ```
   (O: `MINTLIFY_REPO_PATH=../mintlify-docs node scripts/sync-docs-to-mintlify-github.js`)
   El script copia `docs.json`, toda la carpeta `docs/` y los dos `.swagger.json` al repo de GitHub.

3. **Haz commit y push en el repo de Mintlify**:
   ```bash
   cd ../mintlify-docs
   git add -A && git status
   git commit -m "docs: sincronizar desde uni-backend"
   git push origin main
   ```

4. Mintlify detectará el push en GitHub y desplegará automáticamente.

**Resumen:** Trabajas en Bitbucket; cuando quieras publicar la doc, ejecutas el script y luego push en `mintlify-docs` (GitHub).

**Primera vez:** El repo [elbugs/mintlify-docs](https://github.com/elbugs/mintlify-docs) puede tener aún el template (mint.json, introduction.mdx, etc.). Tras el primer sync tendrás también `docs.json` y la carpeta `docs/` con todo el contenido. Mintlify usará `docs.json` para la navegación. Si quieres dejar el repo limpio, puedes borrar del repo de GitHub los archivos del template que no uses (mint.json, introduction.mdx, quickstart.mdx, development.mdx, carpetas essentials/, api-reference/, etc.) y dejar solo `docs.json`, `docs/` y los dos `.swagger.json`.

---

## Resumen de archivos para Mintlify

- **docs.json** (en la raíz del repo o de la ruta de monorepo): configuración del sitio, navegación, APIs.
- **docs/**:
  - Guías en `.md` y `.mdx` (01 a 17, README).
  - OpenAPI: los archivos `public-api.swagger.json` y `booking-engine-api.swagger.json` deben estar en la raíz referenciada por Mintlify (junto a `docs.json`), ya que en `docs.json` se referencian como `public-api.swagger.json` y `booking-engine-api.swagger.json`.

Si los `.swagger.json` están en la raíz del repo, Mintlify los encontrará. Si no, ajusta las rutas en la sección `navigation` de `docs.json`.
