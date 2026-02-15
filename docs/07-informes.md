---
title: Informes y reportes
description: Todos los informes disponibles en Hotelgest Unified, con sus datos, filtros y opciones de exportación.
---

# Informes y reportes

Hotelgest Unified incluye 13 informes principales accesibles desde el menú lateral. Cada informe muestra una tabla interactiva con filtros, ordenación y exportación a Excel.

**URL base:** [app.hotelgest.com/report/bookings](https://app.hotelgest.com/report/bookings)

---

## Funcionalidades comunes a todos los informes

Todos los informes comparten estas funcionalidades:

- **Tabla interactiva**: columnas redimensionables, reordenables y que puedes ocultar o mostrar.
- **Filtros por columna**: texto, número, fecha o rango. Los filtros se guardan en el navegador.
- **Ordenación**: haz clic en la cabecera para ordenar. Puedes ordenar por varias columnas a la vez.
- **Agrupación**: arrastra una cabecera de columna para agrupar los datos.
- **Exportar a Excel**: botón para descargar todas las filas en formato XLSX. Si hay muchos datos, verás una barra de progreso.
- **Totales**: algunos informes muestran totales por propiedad en la parte inferior.
- **Paginación**: los datos se cargan de 100 en 100 (puedes cambiar a 500 o 1000 filas por página).

---

## Lista de informes

### 1. Reservas

**URL:** [report/bookings](https://app.hotelgest.com/report/bookings)

Listado completo de todas las reservas con datos del cliente, fechas, precios y estados.

**Datos principales:**
- ID de reserva, código del canal
- Nombre, apellidos, teléfono, email, nacionalidad del cliente
- Tipo de habitación, habitación asignada, número de puerta
- Fechas: creación, llegada, salida, caducidad, cancelación
- Ocupación: adultos, niños, noches
- Régimen, política de cancelación, código promocional
- Precio alojamiento, comisión, total, total artículos
- Total pagado, total pendiente
- Estado: Confirmada, Tentativa, Cancelada, No-show
- Facturado (sí/no), empresa, notas, usuario creador

**Totales:** precio alojamiento, comisión, noches, ocupación, total, total pagado, total pendiente.

---

### 2. Facturación

**URL:** [report/invoices](https://app.hotelgest.com/report/invoices)

Listado de todas las facturas, proformas y notas de crédito.

**Datos principales:**
- Número/referencia, prefijo
- Tipo: Factura, Proforma, Nota de crédito
- Fecha emisión, llegada, salida
- Base imponible, impuestos, IRPF, total
- Total pagado, total pendiente
- NIF, nombre, teléfono, dirección, ciudad, provincia
- Tipo de habitación, número de puerta
- Firmada (sí/no)

**Totales:** base, impuestos, total, total pagado, total pendiente.

---

### 3. Llegadas

**URL:** [report/arrivals](https://app.hotelgest.com/report/arrivals)

Reservas que llegan en una fecha concreta (por defecto, hoy).

**Datos principales:**
- Nombre, apellidos, habitación, puerta
- Adultos, niños, noches, régimen
- Fecha y hora de llegada, fecha de salida
- Código del canal, origen
- Pendiente de pago, estado de check-in
- Notas del cliente, notas internas

**Totales:** adultos, niños.

---

### 4. Salidas

**URL:** [report/departures](https://app.hotelgest.com/report/departures)

Reservas que se van en una fecha concreta.

**Datos principales:**
- Nombre, apellidos, teléfono, habitación, puerta
- Adultos, niños, noches, régimen
- Fecha llegada, fecha y hora de salida
- Código del canal, origen
- Estado de check-out

**Totales:** adultos, niños.

---

### 5. Pagos

**URL:** [report/payments](https://app.hotelgest.com/report/payments)

Listado de todos los pagos registrados.

**Datos principales:**
- Nombre, apellidos, código de reserva
- Fecha de pago, código de operación
- Factura asociada, facturado (sí/no), fecha emisión factura
- Fechas llegada y salida
- Total, método de pago
- Notas, origen, prepago (sí/no)

**Totales:** total.

---

### 6. Orígenes

**URL:** [report/origins](https://app.hotelgest.com/report/origins)

Resumen de reservas agrupadas por canal de origen (OTA).

**Datos principales:**
- Agencia/Canal (Booking.com, Expedia, Directa, etc.)
- Total reservas (confirmadas y canceladas)
- Importe total
- Noches confirmadas
- Fechas de llegada y salida

**Totales:** reservas totales, confirmadas, canceladas, importes, noches.

---

### 7. Morosos (Atrasado)

**URL:** [report/overdues](https://app.hotelgest.com/report/overdues)

Reservas con pagos pendientes.

**Datos principales:**
- Nombre, apellidos, número de reserva
- Fechas llegada y salida
- Fecha factura, fecha recepción, referencia factura
- Total, pagado, pendiente
- Origen

**Totales:** total pagado, total pendiente, total.

---

### 8. Alojados (In-House)

**URL:** [report/in-house](https://app.hotelgest.com/report/in-house)

Huéspedes que están alojados ahora mismo.

**Datos principales:**
- Nombre, apellidos, nacionalidad, número de documento
- Habitación, número de puerta, régimen
- Email, edad
- Fechas llegada y salida, noches
- Notas, origen/canal

---

### 9. Huéspedes

**URL:** [report/hosts](https://app.hotelgest.com/report/hosts)

Listado de todos los huéspedes registrados.

**Datos principales:**
- Nombre, apellidos, email, teléfono
- Nacionalidad, idioma, país
- Código postal, ciudad, provincia, dirección
- Fecha nacimiento, edad, NIF/CIF
- Notas, consentimiento marketing
- Nombre y apellidos del titular de la reserva

---

### 10. Nacionalidades

**URL:** [report/nationalities](https://app.hotelgest.com/report/nationalities)

Resumen de reservas agrupadas por nacionalidad del huésped.

**Datos principales:**
- Nacionalidad
- Total reservas (totales, confirmadas, canceladas)
- Importe de estancia, importe de extras
- Noches confirmadas, noches canceladas
- ALOS (estancia media en noches)
- Lead Time (antelación media en días)
- Adultos, niños, bebés
- ADR (tarifa media diaria)

**Totales:** reservas totales, confirmadas, canceladas.

---

### 11. Artículos

**URL:** [report/articles](https://app.hotelgest.com/report/articles)

Listado de artículos y extras vendidos.

**Datos principales:**
- Reserva, propiedad
- Fecha creación, inicio y fin de servicio, fecha facturación
- Categoría, artículo
- Estado reembolso, tipo artículo
- Cantidad, base, impuestos, total
- Usuario, unidades vendidas

---

### 12. Empresas

**URL:** [report/companies](https://app.hotelgest.com/report/companies)

Listado de empresas registradas.

**Datos principales:**
- Nombre empresa, nombre comercial
- Email, teléfono
- Dirección, código postal, ciudad, país
- NIF/CIF, cuenta contable

---

### 13. Autoridades

**URL:** [report/authorities](https://app.hotelgest.com/report/authorities)

Estado de los envíos de partes de viajeros a las autoridades.

**Datos principales:**
- Reserva, propiedad
- Fecha creación, ID transacción
- Tipo evento, tipo autoridad
- Estado: Enviado, Error, Pendiente de reintento
- Detalle del error, fecha de reintento

---

## Informes adicionales (Backoffice)

Estos informes están disponibles según los permisos del usuario, pero se acceden desde el backoffice (no desde la interfaz principal):

| Informe | Descripción |
|---------|-------------|
| Contabilidad | Datos contables |
| Limpiezas | Historial de limpiezas |
| Producción | Producción por habitación |
| Ocupación | Porcentajes de ocupación |
| Régimenes | Desglose por régimen (solo alojamiento, media pensión, etc.) |
| Cartera | Cartera de reservas futuras |
| Cierre de turno | Resumen de operaciones del turno |
| Impuestos | Desglose de impuestos |
| INE | Informe para el Instituto Nacional de Estadística |
| Tasa turística | Tasa turística por huésped |
| Caja diaria | Movimientos de caja del día |

---

## Exportar un informe a Excel

1. Abre el informe que quieras exportar.
2. Aplica los filtros que necesites (fechas, estados, etc.).
3. Haz clic en el botón **Exportar a Excel**.
4. Si hay muchos datos, verás una barra de progreso mientras se descargan todas las páginas.
5. El archivo se descarga en formato XLSX con las columnas visibles y en el orden actual.

---

## Permisos

Cada informe requiere un permiso específico. Si no ves un informe en el menú, pide a tu administrador que te conceda el permiso correspondiente.
