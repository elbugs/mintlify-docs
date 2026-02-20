---
title: Integraciones y Marketplace
description: Todas las integraciones disponibles en el Marketplace de Hotelgest Unified, autoridades, pasarelas de pago, firma digital, TV y CRM.
---

# Integraciones y Marketplace

El Marketplace es donde activas y configuras las integraciones de Hotelgest con otros sistemas: autoridades para partes de viajeros, pasarelas de pago, firma digital de facturas, TV interactiva, CRM y más.

**URL:** [app.hotelgest.com/marketplace](https://app.hotelgest.com/marketplace)

---

## Cómo activar una integración

1. Ve al **Marketplace** en el menú lateral.
2. Busca la integración que quieras activar.
3. Haz clic en **Activar**.
4. Rellena los datos de configuración (si los tiene).
5. Guarda.

---

## Autoridades (Partes de viajeros)

### SES (Servicio de Seguridad del Estado)

Envía automáticamente los datos de los huéspedes al SES cuando se hace check-in. Obligatorio en la mayoría de comunidades autónomas de España.

**Cuándo se envían datos:**
- Al crear una reserva confirmada: se registra la reserva.
- Al hacer check-in: se envían los datos de los huéspedes.
- Al cancelar: se anula el registro previo.

**Configuración necesaria:**
| Campo | Descripción |
|-------|-------------|
| **Usuario** | Tu usuario del SES |
| **Contraseña** | Tu contraseña del SES |
| **Código de establecimiento** | El código que te asigna el SES |
| **Credenciales adicionales** | Opcional: credenciales diferentes por tipo de habitación |

---

### Ertzaintza (País Vasco)

Envía automáticamente los datos de los huéspedes a la Ertzaintza. Específico para alojamientos en el País Vasco.

**Cuándo se envían datos:**
- Al crear una reserva confirmada.
- Al hacer check-in: se envían los datos de los huéspedes firmados digitalmente con certificado.

**Configuración necesaria:**
| Campo | Descripción |
|-------|-------------|
| **Certificado digital** | Ruta al certificado digital (.pfx) |
| **Contraseña del certificado** | Contraseña para usar el certificado |
| **ID del arrendador** | Tu identificador como arrendador |
| **Código de establecimiento** | Código del establecimiento |
| **Credenciales adicionales** | Opcional: por tipo de habitación |

---

### Mossos d'Esquadra (Cataluña)

Integración para el envío de partes de viajeros a los Mossos d'Esquadra. Específica para alojamientos en Cataluña.

**Estado:** Definida en el sistema. La configuración se gestiona desde el backoffice.

---

## Firma digital de facturas

### Verifactu

Firma digitalmente las facturas según la normativa española. Al crear una factura, Hotelgest la firma y envía automáticamente.

**Tipos de facturas que firma:**
- Facturas normales
- Facturas de reembolso (notas de crédito)

**Flujo de activación:**
1. Activa Verifactu en el Marketplace.
2. Añade una descripción y selecciona si es producción o pruebas.
3. Solicita la activación (se envía al equipo de Hotelgest).
4. Un Super Admin revisa y aprueba la solicitud.
5. Una vez aprobada, las facturas se firman automáticamente.

**Estados de la integración:**
| Estado | Qué significa |
|--------|---------------|
| **Pendiente** | Acabas de activar, puedes configurar |
| **Solicitada** | Has solicitado la activación, esperando aprobación |
| **Lista** | Aprobada y funcionando |

**Configuración:**
| Campo | Descripción |
|-------|-------------|
| **Descripción** | Texto descriptivo de la integración |
| **Producción** | Sí/No. Indica si envía a la AEAT real o al entorno de pruebas |

---

### TicketBai (País Vasco)

Sistema de firma digital de facturas específico del País Vasco. Funciona de forma similar a Verifactu.

**Tipos de facturas que firma:**
- Facturas normales
- Facturas de reembolso

**Estado:** Implementado en el backend. La configuración se gestiona desde el backoffice.

---

## Pasarelas de pago

Hotelgest se integra con 4 pasarelas de pago para cobrar a los huéspedes desde el motor de reservas y desde la recepción.

### Redsys

Pasarela de pago española ampliamente utilizada. Al pagar, el huésped es redirigido a la página segura de Redsys.

### Monei

Pasarela de pago alternativa. El huésped es redirigido a la URL de Monei para completar el pago.

### Paycomet

Pasarela de pago con soporte para tokenización y pagos recurrentes.

### Stripe

Pasarela de pago internacional con soporte para múltiples monedas y métodos de pago.

**Estado:** Las 4 pasarelas están definidas en el sistema. La configuración se realiza desde el backoffice o desde la configuración de la propiedad.

---

## TV interactiva

### Yuvod

Integración con el sistema de TV interactiva **Yuvod**. Cuando un huésped hace check-in, Hotelgest envía automáticamente sus datos a Yuvod para que la TV de la habitación muestre una pantalla de bienvenida personalizada con el nombre del huésped, su idioma y los servicios del hotel.

#### Para qué sirve

- **Pantalla de bienvenida personalizada**: la TV saluda al huésped por su nombre en su idioma.
- **Información del huésped en la TV**: nombre, apellido, país e idioma.
- **Actualización automática**: al hacer check-in, check-out o al cambiar de habitación, la TV se actualiza sola.

#### Eventos que se envían a Yuvod

Hotelgest envía datos a Yuvod en tres momentos:

1. **Check-in**: cuando el huésped entra en la habitación. La TV muestra la bienvenida.
2. **Check-out**: cuando el huésped se va. La TV vuelve al estado por defecto.
3. **Cambio de habitación**: si se mueve al huésped a otra habitación, la TV de la nueva habitación recibe los datos.

#### Datos que se envían

En cada evento, Hotelgest envía a Yuvod:

| Dato | Descripción |
|------|-------------|
| **hotelId** | Identificador del hotel en Yuvod |
| **eventCode** | Tipo de evento: `CHECKIN`, `CHECKOUT` o `ROOMMOVE` |
| **roomId** | Identificador de la habitación en Yuvod (mapeado desde Hotelgest) |
| **reservation** | Número de reserva |
| **guests** | Lista de huéspedes: nombre, apellido, país (ISO) e idioma (ISO) |

#### Requisitos para que funcione

1. La integración Yuvod debe estar **activada** en el Marketplace.
2. Debe existir un **hotelId** configurado (el que te da Yuvod).
3. Cada habitación de Hotelgest debe estar **mapeada** a su roomId de Yuvod.
4. La reserva debe tener una **habitación asignada**. Si la reserva no tiene habitación, no se envía nada.

#### Cómo activar Yuvod

Actualmente, Yuvod aparece en el Marketplace con el botón **"Configuración próximamente"**. Esto significa que la configuración desde la interfaz de usuario aún no está disponible. Para activar Yuvod, contacta con el equipo de soporte de Hotelgest, que se encargará de:

1. Activar la integración en tu propiedad.
2. Configurar el **hotelId** que te ha proporcionado Yuvod.
3. Mapear cada habitación de Hotelgest con el identificador correspondiente en Yuvod (roomId).

Una vez configurado, cada check-in, check-out o cambio de habitación enviará los datos automáticamente.

#### Qué pasa si algo falla

- Si Yuvod no recibe los datos (por ejemplo, si su servidor no responde), el error queda registrado en los logs del sistema.
- No hay reintentos automáticos. Si un envío falla, puedes hacer un check-out y check-in de nuevo para que se reenvíen los datos.
- La integración no bloquea el check-in: si Yuvod falla, el check-in se completa igualmente en Hotelgest.

---

## CRM

### Clientify

Integración con Clientify, un CRM para gestionar la relación con los clientes.

**Estado:** Definida en el sistema. La implementación y configuración está en desarrollo.

---

## Puntos de venta (POS)

Las integraciones con sistemas de punto de venta (POS) como Ágora permiten enviar cargos desde restaurantes, bares, spa y otros servicios directamente al PMS.

### Cómo funcionan los cargos

Los cargos enviados desde el punto de venta siempre van vinculados a una **habitación con reserva activa**. No es posible procesar cargos "sueltos" que no estén asociados a ninguna reserva.

**Flujo de un cargo:**
1. El empleado selecciona la habitación del huésped en el POS.
2. El POS envía el cargo al PMS.
3. Hotelgest recibe el cargo y lo asocia a la reserva de esa habitación.
4. El cargo aparece en la cuenta del huésped.

### Requisitos para que un cargo se procese

| Requisito | Descripción |
|-----------|-------------|
| **Habitación asignada** | El cargo debe ir dirigido a una habitación específica |
| **Reserva activa** | La habitación debe tener una reserva con check-in realizado |
| **Integración activa** | La integración POS debe estar configurada y activa |

### Qué pasa si no hay reserva

Si se intenta enviar un cargo a una habitación sin reserva activa, el cargo **no se procesará**. El sistema requiere siempre el vínculo entre cargo, habitación y reserva.

**Alternativas:**
- Cobrar directamente en el punto de venta (sin enviar al PMS).
- Crear una reserva de paso (walk-in) para asociar el cargo.

---

## Motor de reservas (Booking Engine)

El motor de reservas también aparece como integración en el Marketplace. Para más detalles, consulta la sección [Motor de reservas](/docs/08-motor-de-reservas).

**Configuración rápida desde el Marketplace:**
| Campo | Descripción |
|-------|-------------|
| **Color primario** | Color principal (hexadecimal) |
| **Color secundario** | Color de acentos (hexadecimal) |
| **Forma de botones** | Cuadrado, redondeado o circular |
| **Google Tag Manager** | ID de GTM (opcional, formato GTM-XXXXXXX) |

---

## Channel Managers

Hotelgest se integra con varios channel managers para sincronizar disponibilidad y precios con las OTAs (Booking.com, Expedia, Airbnb, etc.).

Los channel managers disponibles se configuran desde **Configuración > Channel Manager**.

---

## Cerraduras electrónicas

Las integraciones de cerraduras (HubBuildings y otras) permiten:
- Abrir puertas desde la app al hacer check-in.
- Generar códigos PIN para los huéspedes.
- Registrar accesos.

Estas integraciones aparecen en el historial de actividad cuando se usa check-in/check-out con cerraduras.

---

## Webhooks

Además de las integraciones del Marketplace, puedes configurar webhooks personalizados desde **Configuración > Webhooks** para enviar datos a cualquier sistema externo cuando ocurran eventos en Hotelgest. Consulta la sección [Configuración > Webhooks](/docs/11-configuracion#webhooks) para más detalles.

---

## Resumen de integraciones

| Integración | Categoría | Configuración | Estado |
|-------------|-----------|---------------|--------|
| SES | Autoridades | Desde Marketplace | Activa |
| Ertzaintza | Autoridades | Desde Marketplace | Activa |
| Mossos | Autoridades | Backoffice | Definida |
| Verifactu | Firma digital | Desde Marketplace | Activa |
| TicketBai | Firma digital | Backoffice | Activa |
| Redsys | Pagos | Backoffice | Activa |
| Monei | Pagos | Backoffice | Activa |
| Paycomet | Pagos | Backoffice | Activa |
| Stripe | Pagos | Backoffice | Activa |
| Yuvod | TV | Desde Marketplace | Activa |
| Clientify | CRM | En desarrollo | Definida |
| Motor de reservas | Reservas | Desde Marketplace | Activa |
