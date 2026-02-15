---
title: Aplicación móvil
description: App nativa de Hotelgest Unified para iOS y Android con escaneo de documentos, biometría y notificaciones push.
---

# Aplicación móvil

Hotelgest tiene una aplicación nativa para iOS y Android construida con Ionic y Capacitor. La app incluye todas las funcionalidades de la versión web más algunas exclusivas del móvil: escaneo de documentos con la cámara, acceso con Face ID / huella dactilar y notificaciones push nativas.

**Nombre en las tiendas:** unified by hg
**ID:** com.hotelgest.hotelgestscan

---

## Cómo descargar

| Plataforma | Dónde |
|------------|-------|
| **iPhone / iPad** | App Store |
| **Android** | Google Play Store |
| **Web (sin instalar)** | [app.hotelgest.com](https://app.hotelgest.com) |

---

## Navegación en el móvil

### Barra inferior (5 pestañas)

| Pestaña | Qué muestra |
|---------|-------------|
| **Dashboard** | Panel con widgets y resumen del día |
| **Planificación** | Calendario de reservas |
| **Housekeeping** | Rack de limpieza y tareas pendientes |
| **Actividad** | Registro de actividad reciente |
| **Notificaciones** | Centro de notificaciones |

### Menú lateral

Desliza desde la izquierda o toca el icono de menú para acceder a:
- Todas las secciones según tus permisos
- Selector de propiedad (si gestionas varias)
- Marketplace
- Configuración
- Academia
- Ayuda (Intercom)
- Cerrar sesión

### Vista adaptativa

- **Teléfono vertical**: navegación por pestañas, contenido en una columna.
- **Teléfono horizontal**: pestañas ocultas para maximizar el espacio.
- **Tablet**: vista similar a la web con menú lateral desplegable.

---

## Funciones exclusivas del móvil

### 1. Acceso biométrico (Face ID / Huella dactilar)

Puedes acceder a la aplicación con tu cara (Face ID en iPhone) o con tu huella dactilar (Touch ID en iPhone, sensor de huella en Android) en lugar de escribir tu usuario y contraseña cada vez.

**Cómo activarlo:**
1. En la pantalla de inicio de sesión, marca la casilla **Acceso biométrico**.
2. Inicia sesión con tu usuario y contraseña como siempre.
3. Las credenciales se guardan de forma segura en tu dispositivo.
4. La próxima vez que abras la app, solo necesitarás tu cara o huella.

**Si falla la biometría:**
- Puedes reintentar.
- Siempre puedes volver a escribir tu usuario y contraseña manualmente.

---

### 2. Escaneo de documentos de identidad

La app usa la cámara del móvil para escanear documentos de identidad (DNI, pasaporte, etc.) y extraer los datos automáticamente con OCR.

**Cómo escanear:**
1. Abre el detalle de una reserva.
2. Toca **Escanear documento**.
3. Apunta la cámara al documento.
4. La app lee automáticamente los datos de la zona legible por máquina (MRZ).
5. Los datos se rellenan en el formulario del huésped.

**Datos que se extraen:**
- Nombre y apellidos
- Número de documento
- Nacionalidad y país
- Fecha de nacimiento
- Fecha de emisión y caducidad
- Sexo
- Tipo de documento
- Imágenes: retrato, frente y reverso del documento

**Nota:** El escáner funciona incluso sin conexión a internet, ya que tiene una base de datos local de documentos.

---

### 3. Notificaciones push nativas

La app envía notificaciones nativas a tu dispositivo cuando ocurren eventos importantes.

**Tipos de notificaciones:**
- Nueva reserva recibida
- Reserva cancelada
- Check-in realizado
- Pago recibido
- Tarea asignada
- Mensaje nuevo
- Errores del sistema

**Cómo funcionan:**
- Las notificaciones llegan aunque la app esté cerrada.
- Al tocar una notificación, se abre directamente la reserva o sección relacionada.
- Los iconos de badge muestran el número de notificaciones sin leer.

**Permisos:**
- En iOS: te pedirá permiso la primera vez que abras la app.
- En Android: se activan automáticamente.

---

### 4. Escaneo QR

La app puede escanear códigos QR con la cámara para acceder rápidamente a reservas o verificar facturas.

---

## Qué puedes hacer en la app (igual que en la web)

Todo lo que puedes hacer en la versión web lo puedes hacer también en la app:

- Ver el dashboard con widgets y métricas
- Gestionar el calendario de reservas (ver, crear, mover)
- Ver y gestionar detalles de reservas
- Hacer check-in y check-out
- Gestionar housekeeping (cambiar estados, ver tareas)
- Ver informes y exportar a Excel
- Enviar WhatsApp y emails a huéspedes
- Gestionar la facturación
- Registrar pagos
- Configurar la propiedad
- Cambiar de propiedad (si gestionas varias)

---

## Qué es diferente en la app

| Funcionalidad | Web | App móvil |
|---------------|-----|-----------|
| Acceso biométrico | No | Sí (Face ID, huella) |
| Escaneo de documentos con cámara | No | Sí (OCR automático) |
| Notificaciones push nativas | Solo navegador | Nativas del sistema |
| Escaneo QR | No | Sí |
| Resetear contraseña | Sí | No (se hace desde la web) |
| Verificar email | Sí | No (se hace desde la web) |
| Drag & drop de widgets | Sí | No |
| Informes del backoffice | Sí | No |

---

## Requisitos del dispositivo

| Plataforma | Versión mínima |
|------------|---------------|
| **iOS** | iOS 13 o superior |
| **Android** | Android 5.0 (API 21) o superior |

**Permisos necesarios:**
- Cámara (para escaneo de documentos y QR)
- Notificaciones (para push)
- Biometría (para Face ID / huella)
- Almacenamiento (Android, para documentos)

---

## Versión de la app

Puedes ver la versión de la app en:
- La parte inferior de la pantalla de inicio de sesión.
- Configuración de la aplicación.

Si contactas con soporte, indica siempre la versión de la app que estás usando.
