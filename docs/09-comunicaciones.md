---
title: Comunicaciones
description: WhatsApp, email, notificaciones push y bandeja de entrada en Hotelgest Unified.
---

# Comunicaciones

Hotelgest Unified permite comunicarte con los huéspedes por WhatsApp y email, y envía notificaciones automáticas al equipo cuando ocurren eventos importantes (nueva reserva, cancelación, errores).

**URLs:**
- Notificaciones: [app.hotelgest.com/notifications](https://app.hotelgest.com/notifications)
- Configuración: [app.hotelgest.com/settings/communication](https://app.hotelgest.com/settings/communication)

---

## Canales de comunicación

### 1. WhatsApp

Puedes enviar mensajes de WhatsApp a los huéspedes directamente desde el detalle de la reserva.

**Cómo enviar un WhatsApp:**
1. Abre el detalle de una reserva.
2. Haz clic en el botón **WhatsApp** (aparece si la reserva tiene teléfono).
3. Se muestra un menú con estas opciones:
   - **Abrir chat**: abre WhatsApp con el número del huésped (sin mensaje).
   - **Enviar Web App**: envía al huésped el enlace de la web app (check-in online).
   - **Usar plantilla**: envía un mensaje usando una de tus plantillas configuradas.
   - **Gestionar plantillas**: va a Configuración > Comunicación para crear o editar plantillas.
4. Al seleccionar una opción, se abre la app de WhatsApp del dispositivo con el mensaje preparado.

**Importante:** Hotelgest no usa la API de WhatsApp Business. El sistema prepara el mensaje y abre la app nativa de WhatsApp en tu dispositivo (web o móvil).

#### Plantillas de WhatsApp

Puedes crear plantillas de mensajes con variables dinámicas que se rellenan automáticamente con los datos de la reserva.

**Variables disponibles:**

| Variable | Qué se sustituye |
|----------|-----------------|
| `clientName` | Nombre del huésped |
| `url` | Enlace a la web app |
| `start` | Fecha de llegada |
| `end` | Fecha de salida |
| `nights` | Número de noches |
| `roomName` | Nombre del tipo de habitación |
| `doorNum` | Número de puerta |
| `price` | Precio total |
| `currency` | Moneda (EUR, USD, etc.) |
| `bookingId` | Número de reserva |
| `channelId` | Código del canal |

**Crear una plantilla:**
1. Ve a **Configuración > Comunicación**.
2. Haz clic en **Añadir modelo de WhatsApp**.
3. Escribe un nombre para la plantilla.
4. Redacta el mensaje en los idiomas que necesites, usando las variables entre llaves.
5. Guarda.

Las plantillas se pueden activar o desactivar individualmente.

---

### 2. Email

Hotelgest envía emails automáticos y también permite enviar emails manuales desde el detalle de la reserva.

#### Emails automáticos

| Email | Cuándo se envía |
|-------|----------------|
| **Confirmación de reserva** | Al crear una nueva reserva (si está activado) |
| **Pre-estancia** | X días antes del check-in (configurable) |
| **Post-estancia** | X días después del check-out (configurable) |
| **Check-in online** | Cuando se envía el enlace de la web app al huésped |
| **Confirmación de cancelación** | Al cancelar una reserva |
| **Confirmación de tentativa** | Al confirmar una reserva tentativa |

#### Configurar emails automáticos

Desde **Configuración > Reservas > Comunicación** puedes ajustar:
- **Días de recordatorio pre-estancia**: cuántos días antes del check-in se envía el email.
- **Días de recordatorio post-estancia**: cuántos días después del check-out se envía el email.
- **Enviar confirmación al crear reserva**: activar o desactivar.
- **Enviar copia al administrador**: que el admin reciba una copia de la confirmación.

#### Servidor SMTP personalizado

Puedes configurar tu propio servidor de correo saliente (SMTP) en **Configuración > Reservas > Emails** con estos campos:
- Protocolo, host, puerto
- Email remitente y nombre visible
- Usuario y contraseña
- Seguridad (SSL, STARTTLS, ninguna, auto)
- Email BCC (copia oculta, opcional)

---

### 3. Notificaciones push

El sistema envía notificaciones push automáticas a los dispositivos de tu equipo a través de Firebase Cloud Messaging.

**Plataformas:** Android, iOS y Web (navegador).

**Cuándo se envían:**

| Evento | Notificación |
|--------|-------------|
| Nueva reserva recibida | Push + bandeja de entrada |
| Reserva cancelada | Push + bandeja de entrada |
| Reserva movida (éxito) | Push + bandeja de entrada |
| Reserva movida (error) | Push + bandeja de entrada |
| Reserva redimensionada (éxito) | Push + bandeja de entrada |
| Reserva redimensionada (error) | Push + bandeja de entrada |
| Errores del sistema | Push + bandeja de entrada |

Las push se envían automáticamente; no necesitas configurar nada.

---

### 4. Bandeja de entrada (Inbox)

La bandeja de entrada muestra todas las notificaciones internas de la aplicación.

**URL:** [app.hotelgest.com/notifications](https://app.hotelgest.com/notifications)

**Qué muestra:**
- Notificaciones de nuevas reservas, cancelaciones, movimientos.
- Procesos en curso (mover o redimensionar reservas).
- Errores del sistema e integraciones.
- Notificaciones de otros usuarios.

**Acciones:**
- Marcar como leída / no leída (individual o todas).
- Eliminar notificación (individual o todas).
- Filtrar por categoría: Información, Advertencia, Error.
- Hacer clic en una notificación para ir a la reserva relacionada.

**Caducidad:** Las notificaciones se eliminan automáticamente después de 7 días.

---

## Permisos necesarios

| Permiso | Qué permite |
|---------|-------------|
| **Enviar WhatsApp** | Usar el botón de WhatsApp en el detalle de la reserva |
| **Configuración de comunicación** | Gestionar plantillas de WhatsApp y ajustes de email |
