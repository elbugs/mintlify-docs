---
title: Recepción automática
description: Self check-in, web app para huéspedes y recepción autónoma en Hotelgest Unified.
---

# Recepción automática

La recepción automática permite que los huéspedes hagan el check-in online desde su móvil antes de llegar al alojamiento. El huésped recibe un enlace a una web app donde rellena sus datos, escanea su documento de identidad, firma digitalmente y recibe instrucciones de acceso.

**URL de configuración:** [app.hotelgest.com/settings/autonomousReception](https://app.hotelgest.com/settings/autonomousReception)
**URL para huéspedes:** `https://guest.hotelgest.com/?t={TOKEN}`

---

## Cómo funciona para el huésped

### 1. Recibir el enlace

El huésped recibe un enlace único a la web app por email o WhatsApp. Este enlace se genera automáticamente para cada reserva.

### 2. Rellenar datos personales

El huésped introduce:
- Nombre y apellidos
- Teléfono y email
- Sexo y fecha de nacimiento
- Nacionalidad y país
- Dirección completa (calle, ciudad, provincia, código postal)

### 3. Escanear el documento de identidad

El huésped usa la cámara del móvil para escanear:
- **Parte frontal del documento** (obligatorio)
- **Parte trasera** (opcional, según tipo de documento)

El sistema usa OCR (lectura automática) para extraer los datos del documento y rellenar los campos automáticamente.

Si el documento tiene foto, se puede solicitar un selfie para validación facial.

### 4. Firmar digitalmente

El huésped firma en la pantalla del móvil con el dedo. Esta firma es obligatoria y queda registrada.

### 5. Recibir confirmación

Tras completar el check-in online:
- El huésped recibe la confirmación.
- Si hay cerraduras electrónicas integradas, recibe el código PIN de acceso.
- Se muestra información del alojamiento (WiFi, normas, etc.).

---

## Datos que recoge el check-in online

| Dato | Obligatorio |
|------|-------------|
| Nombre y apellidos | Sí |
| Teléfono | Sí |
| Email | Sí |
| Sexo | Sí |
| Fecha de nacimiento | Sí |
| Nacionalidad | Sí |
| País | Sí |
| Dirección completa | Sí |
| Tipo de documento (DNI, Pasaporte, etc.) | Sí |
| Número de documento | Sí |
| Fecha de emisión | Sí |
| Fecha de expiración | Sí |
| Estado emisor | Sí |
| Foto frontal del documento | Sí |
| Foto trasera del documento | No |
| Foto de perfil del documento | No |
| Firma digital | Sí |

---

## Cómo enviar el enlace al huésped

Desde el detalle de la reserva:

1. Haz clic en el botón **Web App** en la cabecera.
2. Se abre un menú con dos opciones:
   - **Copiar enlace**: copia la URL al portapapeles para pegarla donde quieras.
   - **Abrir enlace**: abre la web app en el navegador para verla.
3. También puedes enviar el enlace por **WhatsApp** usando la opción "Enviar Web App" del menú de WhatsApp.

Si la reserva no tiene enlace generado, se crea automáticamente al hacer clic.

---

## Estado del check-in online

En los informes y el calendario puedes ver el estado del check-in:

| Estado | Qué significa |
|--------|---------------|
| **Pendiente** | El huésped no ha completado el check-in online |
| **Check-in Online** | El huésped ha completado el formulario online |
| **Check-in** | El check-in presencial se ha realizado |

---

## Configuración

Desde **Configuración > Recepción autónoma** puedes ajustar:

| Opción | Qué hace |
|--------|----------|
| **Web App Setup** | Activar o desactivar la web app para los huéspedes |
| **Check-in online estricto** | Solo permite completar el check-in si se detecta una foto válida del documento |
| **Mostrar código PIN** | Muestra el código PIN de acceso en la web app (si hay cerraduras integradas) |
| **Widget del tiempo** | Código de integración para mostrar el pronóstico del tiempo en la web app |
| **Hora de generación del PIN** | Define a qué hora se genera automáticamente el PIN para los check-ins del día |

---

## Qué pasa con los datos

- Los datos del documento (frontal, trasera, foto de perfil) se almacenan de forma segura.
- La firma digital queda registrada junto a los datos del huésped.
- El OCR marca automáticamente si los datos fueron escaneados (`is_ocr`).
- Los datos se utilizan para enviar los partes de viajeros a las autoridades.

---

## Permisos necesarios

| Permiso | Qué permite |
|---------|-------------|
| **Abrir Web App** | Ver el botón Web App en el detalle de la reserva |
| **Configuración de recepción autónoma** | Modificar los ajustes. Solo Admin y Dirección por defecto |

---

## Notas importantes

- La web app (`guest.hotelgest.com`) es una aplicación separada que se comunica con Hotelgest a través del backend.
- El enlace es único por reserva y contiene un token encriptado.
- No hay upselling (venta de extras) en la web app actualmente.
- La configuración de recepción autónoma está parcialmente implementada; algunas opciones son visuales pero los ajustes se aplican en el backend legacy.
