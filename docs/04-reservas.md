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
  - **NB** - Sin régimen (No Board)
  - **BB** - Alojamiento y Desayuno (Bed and Breakfast)
  - **HB** - Media Pensión (Half Board)
  - **FB** - Pensión Completa (Full Board)
  - **AI** - Todo Incluido (All Inclusive)
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
| **Tentativa (Tentative)** | Reserva provisional, pendiente de confirmación. Tiene fecha de caducidad |
| **Cancelada (Cancelled)** | Reserva cancelada |
| **No-Show** | El huésped no se presentó |

---

## Estados de Check-in

El proceso de check-in tiene sus propios estados:

| Estado | Descripción |
|--------|-------------|
| **Pendiente de check-in** | La reserva está confirmada pero el huésped aún no ha llegado |
| **Esperando check-in** | El huésped ha iniciado el proceso (ej. check-in online) |
| **Checked-in** | El huésped está alojado |
| **Checked-out** | El huésped ha dejado el alojamiento |
| **Cancelado** | El check-in ha sido cancelado |

---

## Detalle de la Reserva

Al hacer clic en una reserva se abre su vista de detalle completa con las siguientes secciones:

### Cabecera con acciones

En la parte superior del detalle tienes todas las acciones disponibles:

| Acción | Qué hace |
|--------|----------|
| **Escanear huéspedes** | Escanear documentos de identidad con la cámara |
| **Check-in / Check-out** | Cambiar el estado del huésped |
| **Housekeeping** | Ver y cambiar el estado de limpieza de la habitación |
| **Editar** | Modificar datos de la reserva (fechas, habitación, ocupación, etc.) |
| **Grupo** | Crear o gestionar un grupo de reservas vinculadas |
| **Llaves** | Gestionar cerraduras electrónicas (si las tienes) |
| **Historial** | Ver todo el historial de cambios de la reserva |
| **Enviar recordatorio** | Enviar email (pre-estancia, post-estancia, cancelación, etc.) |
| **Web App** | Copiar o abrir el enlace de la web app del huésped |
| **WhatsApp** | Enviar mensaje por WhatsApp al huésped |
| **Autoridades** | Enviar parte de viajeros a las autoridades |
| **Bloquear / Desbloquear** | Impedir que la reserva se pueda mover o modificar |
| **Clonar** | Crear una copia exacta de la reserva |
| **Dividir** | Partir la reserva en una fecha concreta en dos reservas |
| **Intercambiar habitación** | Intercambiar la habitación con otra reserva |
| **Cambiar color** | Asignar un color personalizado a la reserva en el calendario |
| **Descargar recibo** | Descargar un recibo de la reserva |

### Perfil del cliente (columna izquierda)
- Avatar y nombre completo
- Logo de la OTA de origen
- Teléfono de contacto

### Bloque de detalles
- Fecha y hora de llegada y salida
- Ocupación (adultos, niños, bebés)
- Número de noches
- Política de cancelación
- Régimen
- Fecha de recepción de la reserva

### Indicadores
- Estado de limpieza de la habitación (código de color)
- Aviso de "reserva importada" si procede
- Aviso de "huéspedes pendientes de escanear" si hay documentos pendientes

### Notas (columna derecha)
- **Tareas (To-Dos)**: Tareas asociadas a la reserva, con contadores de pendientes y totales
- **Notas de petición**: Solicitudes del huésped
- **Notas internas**: Notas del personal
- **Notas planas**: Notas generales

### Sección financiera (parte inferior)
Tres columnas con la información económica:

1. **Productos**: Productos y servicios vinculados a la reserva
2. **Facturas y Proformas**: Documentos de facturación
3. **Pagos y Depósitos**: Registros de cobro

---

## Huéspedes

Cada reserva puede tener uno o más huéspedes. El huésped titular es el principal y los demás son acompañantes.

### Datos del huésped

| Campo | Descripción |
|-------|-------------|
| Nombre y apellidos | Nombre completo |
| Email | Correo electrónico |
| Teléfono | Número de teléfono |
| Tipo de documento | DNI, Pasaporte, NIE, etc. |
| Número de documento | Número del documento de identidad |
| Fecha emisión / caducidad | Del documento |
| Nacionalidad | País de origen |
| Idioma | Idioma preferido |
| Fecha de nacimiento | Para cálculo de edad |
| Sexo | Masculino/Femenino |
| Dirección completa | Calle, ciudad, código postal, provincia, país |
| Consentimiento marketing | Si acepta comunicaciones comerciales |

### Escaneo de documentos

El sistema permite escanear documentos de identidad para:
- Rellenar automáticamente los datos del cliente con OCR
- Cumplir con las obligaciones legales de registro de viajeros
- Enviar automáticamente los partes a las autoridades competentes

**Cómo escanear:**
1. Abre la reserva y haz clic en **Escanear huéspedes**.
2. Usa la cámara del dispositivo para capturar el documento.
3. El sistema extrae los datos automáticamente (tecnología Regula).
4. Verifica y confirma los datos extraídos.

### Firma digital

Para el proceso de check-in se solicita la firma digital del huésped:
1. El huésped firma en la pantalla del dispositivo.
2. La firma queda registrada y asociada a la reserva.
3. Cumple con los requisitos legales de consentimiento.

---

## Grupos de reservas (Multibook)

Los grupos vinculan varias reservas entre sí (por ejemplo, un grupo de turistas con varias habitaciones).

### Crear un grupo
1. Abre una reserva.
2. Haz clic en **Grupo** en la cabecera.
3. Selecciona las reservas que quieras vincular.
4. Se crea el grupo con un identificador compartido.

### Qué permite un grupo
- Ver las reservas vinculadas con líneas en el calendario.
- Compartir notas entre las reservas del grupo (si está configurado).
- Mover el grupo completo.
- Identificar rápidamente qué reservas pertenecen al mismo grupo.

---

## Acciones avanzadas

### Dividir una reserva
Parte la reserva en una fecha concreta, creando dos reservas separadas. Útil cuando un huésped cambia de habitación a mitad de la estancia.

### Clonar una reserva
Crea una copia exacta de la reserva con los mismos datos. Útil para crear reservas similares rápidamente.

### Intercambiar habitaciones
Intercambia la habitación asignada entre dos reservas que coinciden en fechas. Útil para resolver conflictos de asignación.

### Bloquear / Desbloquear
Impide que la reserva se pueda mover o redimensionar en el calendario. Útil para proteger reservas VIP o confirmaciones especiales.

---

## Tarjetas de crédito

El sistema permite almacenar de forma segura la información de tarjetas de crédito asociadas a la reserva para:
- Garantizar la reserva
- Cobros posteriores
- Gestión de no-shows

---

## Qué puede ir mal y cómo solucionarlo

**No encuentro una reserva.** Compruebe las fechas que está viendo en el calendario (cambie de semana o mes). Revise si tiene filtros activos (por origen, estado o tipo de habitación) y quite los que no necesite. Si gestiona varias propiedades, compruebe que ha elegido la correcta en el selector.

**He guardado la reserva con un dato equivocado.** Abra de nuevo la reserva y pulse Editar. Corrija el dato y guarde. Si el error es en una factura o un pago ya emitido, puede que necesite anular o ajustar desde Facturación; en caso de duda, consulte con su administrador.

**El sistema no me deja crear la reserva.** Puede que esas fechas o esa habitación no estén disponibles, o que falte un dato obligatorio. Lea el mensaje que aparece en pantalla: suele indicar qué campo revisar.

**Recuerde.** Puede abrir y cerrar reservas para consultar sin miedo: no cambia nada hasta que pulse Guardar o un botón de acción (Check-in, Check-out, etc.).

---

## Permisos necesarios

| Permiso | Qué permite |
|---------|-------------|
| Crear reservas | Dar de alta nuevas reservas |
| Editar y mover | Modificar datos, mover y redimensionar |
| Check-in | Realizar check-in |
| Ver nombre del cliente | Ver el nombre en lugar del número |
| Ver precio | Ver información de precios |
| Gestionar artículos | Añadir, editar y eliminar productos |
| Gestionar facturas | Crear, editar, eliminar y reembolsar facturas |
| Gestionar proformas | Crear, editar y enviar proformas |
| Gestionar pagos | Registrar, editar y reembolsar pagos |
| Enviar email | Enviar emails al huésped |
| Enviar WhatsApp | Enviar WhatsApp al huésped |
| Escanear | Usar el escáner de documentos |
| Abrir Web App | Ver el enlace de la web app |
| Ver notas | Ver notas internas y de petición |
| Gestionar tareas | Crear, editar y eliminar tareas |
| Gestionar limpieza | Cambiar estado de limpieza |
| Agrupar reservas | Crear y gestionar grupos |
| Ver autoridades | Ver estado de envío a autoridades |
| Ver detalle | Abrir el detalle completo de la reserva |
| Buscar reservas | Usar la búsqueda de reservas |

---

## Consejos

- Use el calendario cada día para ver llegadas y salidas; desde ahí puede abrir cualquier reserva con un clic.
- Antes de hacer check-out, compruebe en la pestaña Facturación que los pagos estén registrados.
- Las notas internas son solo para el personal; el huésped no las ve.

**Ver también:** [Facturación y pagos](/docs/05-facturacion-y-pagos), [Planificación](/docs/03-planificacion), [Housekeeping](/docs/06-housekeeping).
