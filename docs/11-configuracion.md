# Configuración y ajustes

**URL base:** [https://app.hotelgest.com/settings](https://app.hotelgest.com/settings)

**Subsecciones:** Perfil (`/settings/profile`), Usuarios (`/settings/users`), Roles (`/settings/roles`), Suscripción (`/settings/subscription`), API Keys (`/settings/api-keys`), Webhooks (`/settings/webhooks`), Comunicación (`/settings/communication`), Auto-asignación de tareas (`/settings/auto-assign-todos`), Políticas (`/settings/policies`), Cuenta (`/settings/account`), Reservas (`/settings/bookings`), Contabilidad (`/settings/accounting`), Habitaciones (`/settings/rooms`), Recepción autónoma (`/settings/autonomousReception`), Privacidad de datos (`/settings/dataPrivacy`), Impuestos (`/settings/taxes`), Channel Manager (`/settings/channel`).

El módulo de Configuración permite personalizar todos los aspectos de Hotelgest Unified. Se accede desde el menú **Configuración** (icono de engranaje).

---

## Perfil

Gestión de tu cuenta de usuario personal.

### Datos personales
- **Nombre** y **apellidos**
- **Nombre de usuario** (solo lectura o editable según permisos)
- **Correo electrónico**

### Seguridad
- **Cambiar contraseña**: Introduce la contraseña actual y la nueva
- **Autenticación de dos factores (2FA)**: Activar o desactivar la verificación con aplicación de autenticación (Google Authenticator, Authy, etc.)

### Sesiones
- Lista de **sesiones activas** en distintos dispositivos
- **Cerrar sesiones** en dispositivos remotos

### Consentimiento
- Gestión del consentimiento de tratamiento de datos

---

## Usuarios

Gestión de los usuarios que acceden al sistema.

### Lista de usuarios
Tabla con las columnas:
- Nombre de usuario
- Nombre completo
- Email
- Rol asignado
- Habitaciones asignadas

### Acciones
- **Añadir usuario**: Crear un nuevo usuario con nombre, apellidos, email, contraseña, rol y permisos de habitación
- **Editar**: Modificar los datos de un usuario existente
- **Bloquear/Desbloquear**: Suspender el acceso de un usuario sin eliminarlo
- **Compartir**: Compartir credenciales con el usuario
- **Eliminar**: Eliminar un usuario permanentemente
- **Activar/Desactivar 2FA**: Gestionar la autenticación de dos factores por usuario
- **Enviar email de verificación**: Reenviar el email de verificación

---

## Roles

Gestión de roles y permisos de acceso.

### Crear un rol
1. Haz clic en **Añadir rol**
2. Asigna un **nombre** al rol
3. Configura los **permisos** por módulo:

### Módulos de permisos

| Módulo | Permisos disponibles |
|--------|---------------------|
| **Dashboard** | Ver dashboard, ver widgets específicos |
| **Calendario** | Ver planificación, crear/editar/mover reservas |
| **Reservas** | Ver, crear, editar, eliminar, check-in, check-out, escanear |
| **Housekeeping** | Ver rack, cambiar estados, gestionar limpieza |
| **Menú** | Acceso a secciones del menú lateral |
| **Configuración** | Acceso a las distintas secciones de configuración |

### Acciones sobre roles
- **Editar**: Modificar nombre y permisos
- **Eliminar**: Eliminar el rol (no puede estar asignado a usuarios)
- **Compartir**: Exportar la configuración del rol
- **Crear desde plantilla**: Usar un rol existente como base

---

## Suscripción

Gestión del plan de suscripción y facturación.

- Ver el **plan actual** contratado
- **Cambiar de plan**: Upgrade o downgrade
- **Gestionar facturación**: Datos de pago, historial de facturas
- Integración con **Chargebee** para la gestión de suscripciones

---

## API Keys

Gestión de claves de API para integraciones externas.

### Lista de API Keys
- **Descripción** de la clave
- **Fecha de creación**
- **Estado**: Habilitada o deshabilitada

### Crear una API Key
1. Haz clic en **Añadir API Key**
2. Introduce una **descripción** identificativa
3. La clave se genera automáticamente
4. **Copia la clave** (solo se muestra una vez)

---

## Webhooks

Configuración de webhooks para enviar datos a sistemas externos cuando ocurren eventos.

### Eventos disponibles
- Nueva reserva
- Modificación de reserva
- Cancelación de reserva
- Check-in
- Check-out
- Pago recibido

### Configurar un webhook
1. Haz clic en **Añadir webhook**
2. Introduce la **URL** de destino
3. Selecciona los **eventos** que activarán el webhook
4. Opcionalmente, añade **cabeceras** personalizadas
5. Activa o desactiva el webhook

---

## Auto-asignación de Tareas

Automatiza la creación de tareas según reglas predefinidas.

### Crear una regla
1. Haz clic en **Añadir regla**
2. Define el **nombre** de la regla
3. Configura las **condiciones** (cuándo se activa)
4. Define las **tareas** que se crean automáticamente
5. Asocia **recursos** (habitaciones, usuarios) a los que aplica

### Gestión de reglas
- **Ver tareas**: Ver las tareas generadas por esta regla
- **Ver recursos**: Ver los recursos asociados
- **Editar**: Modificar la regla
- **Activar/Desactivar**: Habilitar o deshabilitar la regla
- **Eliminar**: Eliminar la regla

---

## Comunicación

Gestión de plantillas de comunicación.

### Plantillas de WhatsApp
- **Crear plantilla**: Nombre, contenido, idiomas
- **Editar**: Modificar el contenido
- **Activar/Desactivar**: Habilitar o deshabilitar
- Ver **fecha de creación** e idiomas configurados

---

## Políticas

Configuración de políticas de cancelación para las reservas.

### Tipos de política
- **Flexible**: Cancelación gratuita hasta una fecha determinada
- **No reembolsable**: Sin posibilidad de cancelación gratuita

### Gestión
- **Ver plantillas**: Políticas predefinidas del sistema
- **Ver políticas personalizadas**: Políticas creadas por ti
- **Añadir política**: Crear una nueva política con sus condiciones

---

## Cuenta

Información y configuración de la propiedad.

### Datos de la propiedad
| Campo | Descripción |
|-------|-------------|
| **Tipo de propiedad** | Hotel, apartamento turístico, hostal, etc. |
| **Nombre** | Nombre del establecimiento |
| **Teléfono** | Número de contacto |
| **Email** | Correo electrónico de la propiedad |
| **Web** | Sitio web |
| **Moneda** | Moneda de operación (EUR, USD, GBP, etc.) |
| **Logo** | Logo del establecimiento |
| **Descripción** | Descripción del alojamiento |

### Ubicación
- Dirección
- Ciudad
- Código postal
- Provincia
- País
- Zona horaria

### Imágenes
- Galería de fotos de la propiedad

---

## Privacidad de Datos

Configuración de retención y protección de datos conforme al RGPD.

### Retención de datos
- **Período**: De 1 a 10 años
- Datos afectados:
  - Datos de identificación
  - Número de documento
  - Imágenes de documentos
  - Datos de facturación
  - Notas internas

---

## Impuestos

Configuración de impuestos aplicables.

### Impuesto local
- Configuración del IVA u otros impuestos locales

### Impuestos adicionales
- Configuración de impuestos extra

### Tasa turística
- **Precio por adulto** por noche
- **Precio por niño** por noche
- **Número de noches** que aplica
- **Recargo municipal** (si procede)
- **Tarifas por temporada** (si varían según la época)

---

## Contabilidad

Configuración del sistema de facturación.

### Datos fiscales de la empresa
- Nombre fiscal
- NIF/CIF
- Dirección fiscal

### Numeración de documentos
- **Prefijo de facturas**: Ej. "F-"
- **Prefijo de proformas**: Ej. "P-"
- **Prefijo de notas de crédito**: Ej. "NC-"
- **Prefijo de servicios**: Ej. "S-"

### Impuestos en facturas
- Configuración de los tipos impositivos aplicables

### Opciones de facturación
- **Campos obligatorios**: Qué datos del cliente son requeridos en la factura
- **Hora de cierre**: Hora a la que se cierra la contabilidad del día
- **Opciones de facturación**: Configuración avanzada
- **Pie de factura**: Texto legal o informativo en la parte inferior

---

## Habitaciones

Gestión de habitaciones y tipologías.

### Tipologías de habitación
Cada tipología incluye:
| Campo | Descripción |
|-------|-------------|
| **Nombre** | Nombre del tipo (Doble, Suite, Individual, etc.) |
| **Camas** | Número de camas |
| **Baños** | Número de baños |
| **Tamaño** | Metros cuadrados |
| **Ocupación** | Máxima y mínima |
| **Número de puerta** | Número identificativo |
| **Planta** | En qué planta se encuentra |
| **Orden** | Orden de visualización |
| **Inventario** | Unidades disponibles |
| **Motor de reservas** | Si se muestra en el Booking Engine |
| **Fotos** | Galería de imágenes |
| **Ubicación** | Posición en el mapa del hotel |
| **Coste de limpieza** | Precio por limpieza |
| **Tipo INE** | Clasificación para el Instituto Nacional de Estadística |

---

## Reservas (Configuración)

Opciones que afectan al funcionamiento de las reservas.

### Operación diaria
- Configuración de la operativa diaria

### Campos obligatorios
Selecciona qué campos son obligatorios al crear una reserva:
- Nombre, Apellidos, Teléfono, Dirección, etc.

### Opciones
- **Decimales**: Número de decimales en precios
- **Notas compartidas**: Si las notas son visibles entre propiedades
- **Días de limpieza**: Periodicidad de limpieza (0 = desactivado)
- **Hora de check-in**: Hora estándar de entrada
- **Hora de check-out**: Hora estándar de salida
- **Asignación de habitación**: Automática o manual
- **Check-out restrictivo**: Si se requiere facturación completa para hacer check-out
- **Colores**: Personalización de colores por estado o origen

### Comunicación con el huésped
- Configuración de emails automáticos
- Configuración de mensajes

### Configuración SMTP
- Servidor SMTP propio para envío de emails desde tu dominio

---

## Recepción Autónoma

Configuración del sistema de check-in automático. Ver la sección [Recepción Automática](10-recepcion-automatica.md) para más detalles.

---

## Channel Manager

Integración con el Channel Manager (Channex) para gestionar la distribución en OTAs.

### Pasos de configuración
1. **Inventario**: Configurar el inventario de habitaciones
2. **Reservas**: Configurar la sincronización de reservas
3. **Habitaciones**: Mapear las habitaciones con los canales
4. **Canales**: Conectar y configurar cada OTA (Booking.com, Expedia, etc.)
