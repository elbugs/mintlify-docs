# 04 - Gestión de Reservas

**URL del detalle de reserva:** `https://app.hotelgest.com/details/{pcode}/{bookingId}`  
*(Sustituye `{pcode}` por el código de la propiedad y `{bookingId}` por el ID de la reserva. También puedes abrir una reserva desde el calendario o el dashboard.)*

Las reservas son el elemento central del PMS. Desde aquí puedes gestionar todo el ciclo de vida de una estancia: desde la creación hasta el check-out.

---

## Crear una Reserva

Para crear una nueva reserva puedes:
1. Usar la **acción rápida** "Crear reserva" desde el Dashboard o el menú
2. **Seleccionar un rango** de fechas en el calendario de Planificación
3. Pulsar la tecla **P** en el calendario

### Datos de la reserva
- **Fechas**: Llegada y salida
- **Tipo de habitación**: Selección de tipología
- **Habitación**: Asignación específica (opcional al crear)
- **Ocupación**: Número de adultos, niños y bebés
- **Régimen (Board)**:
  - **SA** (Solo Alojamiento / Room Only)
  - **AD** (Alojamiento y Desayuno / Bed & Breakfast)
  - **MP** (Media Pensión / Half Board)
  - **PC** (Pensión Completa / Full Board)
  - **TI** (Todo Incluido / All Inclusive)
- **Política**: Flexible o No Reembolsable
- **Origen**: Canal de la reserva (directa, Booking.com, Expedia, etc.)
- **Código promocional**: Si aplica
- **Empresa/Agencia**: Asociar a una empresa
- **Notas del cliente**: Peticiones especiales del huésped
- **Notas internas**: Notas visibles solo para el personal

---

## Estados de la Reserva

Las reservas pasan por distintos estados a lo largo de su ciclo de vida:

| Estado | Descripción |
|--------|-------------|
| **Confirmada (Ready)** | Reserva confirmada y activa |
| **Tentativa (Tentative)** | Reserva provisional, pendiente de confirmación |
| **Cancelada (Cancelled)** | Reserva cancelada |
| **No-Show** | El huésped no se presentó |

---

## Estados de Check-in

El proceso de check-in tiene sus propios estados:

| Estado | Descripción |
|--------|-------------|
| **Pendiente de check-in** | La reserva está confirmada pero el huésped aún no ha llegado |
| **Esperando check-in** | El huésped ha iniciado el proceso de check-in (ej. registro online) |
| **Checked-in** | El huésped está alojado |
| **Checked-out** | El huésped ha dejado el alojamiento |
| **Cancelado** | El check-in ha sido cancelado |

---

## Detalle de la Reserva

Al hacer clic en una reserva se abre su vista de detalle completa con las siguientes secciones:

### Información principal (columna izquierda)

#### Cabecera con acciones
- **Escanear huéspedes**: Escanear documentos de identidad
- **Estado de check-in**: Cambiar el estado (check-in, check-out)
- **Housekeeping**: Ver estado de limpieza de la habitación
- **Editar**: Modificar datos de la reserva
- **Gestión de grupo**: Para reservas agrupadas
- **Llaves**: Gestionar cerraduras electrónicas
- **Historial**: Ver historial de cambios del huésped
- **Enviar recordatorio**: Enviar email de recordatorio
- **Web App**: Enviar enlace de la web app al huésped
- **WhatsApp**: Enviar mensaje por WhatsApp
- **Autoridades**: Enviar parte de viajeros

#### Perfil del cliente
- Avatar y nombre completo
- Logo de la OTA de origen

#### Bloque de detalles
- Fecha y hora de llegada
- Fecha y hora de salida
- Ocupación (adultos, niños, bebés)
- Número de noches
- Política de cancelación
- Régimen
- Teléfono de contacto
- Fecha de recepción de la reserva

#### Indicadores
- Estado de limpieza de la habitación (código de color)
- Aviso de "reserva importada" si procede
- Aviso de "huéspedes pendientes de escanear" si hay documentos pendientes

### Notas (columna derecha)
- **Tareas (To-Dos)**: Tareas asociadas a la reserva
- **Notas de petición**: Solicitudes del huésped
- **Notas internas**: Notas del personal
- **Notas planas**: Notas generales

### Sección financiera (parte inferior)
Tres columnas con la información económica:

1. **Productos**: Productos y servicios vinculados a la reserva
2. **Facturas y Proformas**: Documentos de facturación
3. **Pagos y Depósitos**: Registros de cobro

---

## Escaneo de Documentos

El sistema permite escanear documentos de identidad de los huéspedes para:
- Rellenar automáticamente los datos del cliente (nombre, apellidos, número de documento, nacionalidad, fecha de nacimiento)
- Cumplir con las obligaciones legales de registro de viajeros
- Enviar automáticamente los partes a las autoridades competentes

### Cómo escanear
1. Abre la reserva y haz clic en **"Escanear huéspedes"**
2. Usa la cámara del dispositivo para capturar el documento
3. El sistema extrae los datos automáticamente (tecnología Regula)
4. Verifica y confirma los datos extraídos

---

## Firma Digital

Para el proceso de check-in se puede solicitar la firma digital del huésped:
1. El huésped firma en la pantalla del dispositivo
2. La firma queda registrada y asociada a la reserva
3. Cumple con los requisitos legales de consentimiento

---

## Datos del Cliente

Cada reserva contiene la información del huésped:

| Campo | Descripción |
|-------|-------------|
| Nombre | Nombre del huésped |
| Apellidos | Apellidos del huésped |
| Email | Correo electrónico |
| Teléfono | Número de teléfono |
| Tipo de documento | DNI, Pasaporte, NIE, etc. |
| Número de documento | Número del documento de identidad |
| Nacionalidad | País de origen |
| Idioma | Idioma preferido |
| Fecha de nacimiento | Para cálculo de edad y requisitos legales |
| Sexo | Masculino/Femenino |
| Dirección | Dirección completa (calle, ciudad, código postal, provincia, país) |
| Consentimiento de marketing | Si acepta comunicaciones comerciales |

---

## Imágenes

Se pueden adjuntar imágenes a la reserva:
- Fotos de documentos de identidad
- Fotos de daños o incidencias
- Cualquier imagen relevante

---

## Tarjetas de Crédito

El sistema permite almacenar de forma segura la información de tarjetas de crédito asociadas a la reserva para:
- Garantizar la reserva
- Cobros posteriores
- Gestión de no-shows
