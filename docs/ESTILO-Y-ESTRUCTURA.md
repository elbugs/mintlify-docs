# Guía de estilo y estructura para artículos de help desk

Este documento define cómo deben redactarse los artículos y, si se publican en Intercom, cómo darles formato con HTML específico (tablas como bloques, botones, títulos).

**Formato Intercom.** Para que un artículo se vea en Intercom con bloques tipo “card”, botones y títulos claros, se puede crear un archivo **`.intercom.html`** con el mismo nombre que el `.md` (ej. `01-inicio-y-autenticacion.intercom.html`). Al sincronizar con Intercom, si existe ese archivo se usa su contenido como cuerpo del artículo; si no, se convierte el Markdown a HTML. En el HTML para Intercom solo están permitidos: `h1`, `h2`, `p`, `ul`, `ol`, `li`, `table`, `a`, `strong`, `em`, `br`, `hr`, `img`, etc. No se permiten `div` ni `span`. Clases útiles: `intercom-h2b-button` (enlaces con estilo botón) e `intercom-align-center` (centrar). Se pueden usar tablas de una celda como bloques/cards. Ver [HTML soportado por Intercom](https://developers.intercom.com/docs/guides/help-center/supported-html).

---

Este documento define cómo deben redactarse los artículos para que, al subirlos a Intercom (o cualquier help center), tengan **contenido suficiente**, **estructura clara** y **armonía** entre ellos. No se publica como artículo; sirve de referencia interna.

---

## Estructura tipo de cada artículo

1. **Título**
   - Frase clara y orientada al usuario: "Cómo hacer X" o "Qué es X y para qué sirve".
   - Sin códigos ni prefijos tipo "01 -".

2. **Bloque inicial (obligatorio)**
   - **Resumen:** 2–4 frases que explican de qué va el artículo y qué conseguirá el usuario.
   - **En este artículo:** lista breve de los temas que se van a tratar (enlaces internos opcionales).
   - **Acceso / URL** (si aplica): enlace directo a la pantalla o sección.

3. **Cuerpo**
   - Cada sección sigue el **mismo esquema**:
     - **Título de sección:** pregunta o afirmación clara ("Cómo es...", "He olvidado...", "Qué hacer si...").
     - **Párrafo de contexto:** 2–4 frases que explican por qué existe esa función o qué verá el usuario.
     - **Pasos numerados:** 1. Acción. 2. Siguiente acción. Una idea por paso.
     - **Nota o consejo** (si aplica): aclaración, diferencia web/móvil, error frecuente.

4. **Cierre**
   - **Resumen:** párrafo corto que recapitula los pasos o ideas principales.
   - **Qué hacer si algo falla** (si aplica): comprobar X, contactar a Y.
   - **Ver también:** 1–2 enlaces a otros artículos relacionados.

---

## Contenido

- **Explicar el "por qué"** en una o dos frases cuando ayude (por ejemplo: "El login está en dos pasos para mayor seguridad").
- **Indicar qué verá el usuario** en pantalla cuando sea útil ("Verás la segunda pantalla, la de la contraseña").
- **Incluir errores frecuentes o limitaciones** (solo web, solo móvil, revisar spam, hora del dispositivo en 2FA).
- **Evitar listas sueltas** sin contexto: cada lista debe tener un título y, si hace falta, un párrafo previo.

---

## Armonía

- **Mismo tipo de pasos:** siempre numerados (1. 2. 3.) y con una acción clara por paso.
- **Mismo tono:** tú/usted según lo que use el resto del help (elegir uno y mantenerlo).
- **Longitud similar** de párrafos (2–4 frases) y de secciones (no una sección de 2 líneas y otra de 20).
- **Mismos elementos repetidos:** "Resumen" al inicio, "Resumen" al final, "Ver también" al cierre.
- **Palabras clave consistentes:** mismo término para la misma cosa (ej. "pantalla de login", "Iniciar sesión").

---

## Qué evitar

- Títulos que sean solo etiquetas ("Login", "2FA") sin verbo o pregunta.
- Bloques de solo viñetas sin texto introductorio.
- Pasos mezclados con sublistas confusas; si hay subpasos, que estén bien indentados y sean breves.
- Artículos que terminen de golpe sin resumen ni "Ver también".
- Jerga técnica sin explicar (si usas "2FA", explicar "autenticación en dos pasos" la primera vez).

---

## Ejemplo de sección bien formada

**Título de sección:** He olvidado mi contraseña: cómo restablecerla

**Contexto:** Si no recuerdas la contraseña, puedes pedir un enlace para crear una nueva. Importante: el restablecimiento solo está disponible en la versión web. Si estás en la app, abre el navegador y ve a la misma dirección de login.

**Pasos:** (sublógica "Solicitar enlace" y "Crear nueva contraseña", cada una con 1. 2. 3.)

**Nota:** Si no ves el email, revisa la carpeta de spam.

Este mismo esquema (título → contexto → pasos → nota) se repite en todas las secciones del artículo para dar **estructura** y **armonía**.
