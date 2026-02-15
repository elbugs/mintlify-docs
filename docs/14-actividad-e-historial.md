---
title: Actividad e historial
description: Registro de actividad, historial de cambios y auditoría de todas las acciones en Hotelgest Unified.
---

# Actividad e historial

Hotelgest registra automáticamente todas las acciones que se realizan en el sistema: quién hizo qué, cuándo y sobre qué reserva. Esto permite auditar cambios, detectar errores y saber exactamente qué ha ocurrido con cada reserva.

**URL:** [app.hotelgest.com/activity](https://app.hotelgest.com/activity)

---

## Qué se registra

El historial registra más de 80 tipos de eventos, agrupados por categoría.

### Reservas

| Evento | Qué significa |
|--------|---------------|
| Nueva reserva | Se creó una reserva |
| Reserva actualizada | Se modificaron datos de la reserva |
| Reserva cancelada | Se canceló la reserva |
| Cambio de estado | Cambio a confirmada, tentativa, etc. |
| Cambio de habitación | Se movió a otra habitación |
| Cambio de habitación con precio | Se movió con ajuste de precio |
| División de reserva | Se dividió en dos reservas |
| Multireserva creada | Se creó un grupo de reservas |
| Reserva al playground | Se envió al playground |
| Cambio de precio | Se modificó el precio |
| Cambio de color | Se cambió el color de la reserva |
| Comentario actualizado | Se modificaron las notas |

### Check-in / Check-out

| Evento | Qué significa |
|--------|---------------|
| Check-in | Check-in realizado |
| Check-out | Check-out realizado |
| Deshacer check-in | Se deshizo el check-in |
| Deshacer check-out | Se deshizo el check-out |
| Check-in error | Error al intentar check-in |
| Check-in con cerraduras | Check-in con integración de cerraduras (HubBuildings, Char, IO) |
| Check-out con cerraduras | Check-out con integración de cerraduras |

### Facturación

| Evento | Qué significa |
|--------|---------------|
| Factura creada | Se generó una nueva factura |
| Factura actualizada | Se modificó una factura |
| Factura eliminada | Se eliminó una factura |
| Proforma creada | Se generó una proforma |
| Factura enviada | Se envió por email |
| Proforma enviada | Se envió por email |
| Artículo creado | Se añadió un artículo a la reserva |
| Artículo actualizado | Se modificó un artículo |
| Artículo eliminado | Se eliminó un artículo |
| Impuesto eliminado | Se eliminó un impuesto de la factura |

### Pagos

| Evento | Qué significa |
|--------|---------------|
| Pago registrado | Se añadió un pago |
| Pago de factura creado | Pago asociado a factura |
| Pago parcial | Pago parcial de factura |
| Nota de crédito | Se generó una nota de crédito |
| Pago por canal | Pago recibido de una OTA |
| Pago eliminado | Se eliminó un pago |
| Reembolso | Se procesó un reembolso |
| Pago TPV | Pago por TPV (Monei, Paycomet, Redsys, Stripe) |
| Pago convertido a anticipo | Un pago se convirtió en anticipo |
| Depósito añadido | Se registró un depósito |
| Depósito actualizado | Se modificó un depósito |
| Depósito eliminado | Se eliminó un depósito |
| Depósito reembolsado | Se reembolsó un depósito |
| Depósito convertido a pago | Se convirtió el depósito en pago definitivo |

### Bloqueos

| Evento | Qué significa |
|--------|---------------|
| Bloqueo creado | Se bloqueó una habitación |
| Bloqueo eliminado | Se desbloqueó |
| Bloqueo fuera de orden | Habitación fuera de servicio |
| Bloqueo fuera de servicio | Habitación en mantenimiento |

### Comunicaciones

| Evento | Qué significa |
|--------|---------------|
| Email enviado | Se envió un email al huésped |
| SMS enviado | Se envió un SMS |
| Error SMS | Error al enviar SMS |
| Error WhatsApp | Error al enviar WhatsApp |
| Email de confirmación | Email de nueva reserva |
| Email de cancelación | Email de cancelación |
| Email de expiración | Email de tentativa expirada |
| Email de modificación | Email de reserva modificada |

### Autoridades

| Evento | Qué significa |
|--------|---------------|
| Parte enviado | Parte de viajeros enviado a las autoridades |
| Registro SES | Parte enviado al Sistema de Entrada y Salida |
| Registro Ertzaintza | Parte enviado a la Ertzaintza (País Vasco) |
| Registro Mossos | Parte enviado a los Mossos d'Esquadra (Cataluña) |
| Error en envío | Error al enviar a autoridades |

### Firma digital (Verifactu)

| Evento | Qué significa |
|--------|---------------|
| Factura simplificada firmada | Se firmó y envió factura simplificada |
| Factura normal firmada | Se firmó y envió factura normal |
| Factura de reembolso enviada | Se envió factura de reembolso |
| Cambio de simplificada a normal | Se convirtió una factura simplificada en normal |

### Otros

| Evento | Qué significa |
|--------|---------------|
| Huésped actualizado | Se modificaron datos de un huésped |
| Huésped eliminado | Se eliminó un huésped de la reserva |
| Registro de vehículo | Se registró la matrícula |
| Estado de habitación | Cambio de estado de habitación (cerraduras) |
| Cerradura | Acción sobre cerradura electrónica |
| Impuesto generado | Se generó un impuesto de reserva |

---

## Qué información muestra cada evento

Cada entrada del historial incluye:

| Campo | Descripción |
|-------|-------------|
| **Tipo de evento** | Qué acción se realizó |
| **Reserva** | Número de la reserva afectada |
| **Autor** | Nombre y apellidos del usuario que realizó la acción |
| **Fecha y hora** | Cuándo se realizó |
| **Icono** | Icono visual según la categoría (calendario, tarjeta, email, etc.) |
| **Detalles** | Información adicional específica del evento |

Los eventos se agrupan por fecha, mostrando los más recientes primero.

---

## Cómo acceder al historial

### Historial general
Desde el menú lateral, haz clic en **Actividad**. Verás todas las acciones realizadas en la propiedad actual.

### Historial de una reserva
Desde el detalle de una reserva, puedes ver el historial específico de esa reserva: todos los cambios, pagos, emails y acciones realizadas sobre ella.

---

## Permisos necesarios

| Permiso | Qué permite |
|---------|-------------|
| **Actividad (menú)** | Ver la sección de Actividad en el menú lateral |

El historial de una reserva es visible para cualquier usuario que pueda ver los detalles de la reserva.
