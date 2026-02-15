---
title: Reservas
description: Cómo crear, editar y gestionar reservas en Hotelgest Unified.
---

# Cómo gestionar las reservas

**Para qué sirve.** Las reservas son el núcleo del programa: cada reserva es un huésped (o grupo) que viene en unas fechas concretas. Desde aquí puede crear reservas nuevas, ver y editar las que ya tiene, hacer check-in y check-out y pasar a la facturación. Todo lo que hace con un huésped pasa por la ficha de su reserva.

**Dónde está.** Puede abrir el calendario de reservas desde el menú (Planificación o Reservas) o desde el Panel de Control. Al pulsar sobre una reserva en el calendario se abre su ficha con todos los datos. No se preocupe: al abrir una reserva solo la está consultando; no la modifica hasta que pulse Guardar o un botón de acción (por ejemplo Check-in).

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

---

## Qué puede ir mal y cómo solucionarlo

**No encuentro una reserva.** Compruebe las fechas que está viendo en el calendario (cambie de semana o mes). Revise si tiene filtros activos (por origen, estado o tipo de habitación) y quite los que no necesite. Si gestiona varias propiedades, compruebe que ha elegido la correcta en el selector.

**He guardado la reserva con un dato equivocado.** Abra de nuevo la reserva y pulse Editar. Corrija el dato y guarde. Si el error es en una factura o un pago ya emitido, puede que necesite anular o ajustar desde Facturación; en caso de duda, consulte con su administrador.

**El sistema no me deja crear la reserva (fechas, habitación).** Puede que esas fechas o esa habitación no estén disponibles, o que falte un dato obligatorio. Lea el mensaje que aparece en pantalla: suele indicar qué campo revisar. Corrija y vuelva a intentar. Sus datos no se pierden si cierra el formulario sin guardar.

**Recuerde.** Puede abrir y cerrar reservas para consultar sin miedo: no cambia nada hasta que pulse Guardar o un botón de acción (Check-in, Check-out, etc.). Si tiene dudas, no guarde y consulte con un compañero o con soporte.

---

## Consejos

- Use el calendario cada día para ver llegadas y salidas; desde ahí puede abrir cualquier reserva con un clic.
- Antes de hacer check-out, compruebe en la pestaña Facturación que los pagos estén registrados.
- Las notas internas son solo para el personal; el huésped no las ve. Use las "notas del cliente" para peticiones que deba ver el huésped.

**Ver también:** [Facturación y pagos](/docs/05-facturacion-y-pagos), [Planificación](/docs/03-planificacion), [Housekeeping](/docs/06-housekeeping).
