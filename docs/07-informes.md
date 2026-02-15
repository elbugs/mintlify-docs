---
title: Informes y reportes
description: Todos los informes disponibles y sus filtros en Hotelgest Unified.
---

# Informes y reportes

**URLs de informes:**
- [Reservas](https://app.hotelgest.com/report/bookings) · [Facturas](https://app.hotelgest.com/report/invoices) · [Llegadas](https://app.hotelgest.com/report/arrivals) · [Salidas](https://app.hotelgest.com/report/departures) · [Pagos](https://app.hotelgest.com/report/payments) · [Orígenes](https://app.hotelgest.com/report/origins) · [Morosos](https://app.hotelgest.com/report/overdues) · [In-house](https://app.hotelgest.com/report/in-house) · [Huéspedes](https://app.hotelgest.com/report/hosts) · [Nacionalidades](https://app.hotelgest.com/report/nationalities) · [Artículos](https://app.hotelgest.com/report/articles) · [Autoridades](https://app.hotelgest.com/report/authorities) · [Empresas](https://app.hotelgest.com/report/companies)

Hotelgest Unified ofrece un amplio conjunto de informes para analizar la operativa y el rendimiento de tu propiedad. Todos los informes comparten funcionalidades comunes y además están disponibles informes adicionales a través del backoffice.

---

## Funcionalidades Comunes

Todos los informes comparten las siguientes características:

- **Tabla interactiva**: Basada en AG Grid con columnas redimensionables y reordenables
- **Filtros flotantes**: Filtros visibles en la cabecera de cada columna
- **Visibilidad de columnas**: Mostrar/ocultar columnas según necesidad
- **Agrupación por filas**: Agrupar datos por cualquier columna
- **Fijación de columnas (Pinning)**: Fijar columnas a la izquierda o derecha
- **Exportar a Excel**: Descargar los datos en formato Excel
- **Guardar filtros**: Guardar combinaciones de filtros para uso futuro
- **Pie de totales**: Mostrar/ocultar fila de totales en la parte inferior
- **Paginación**: 100, 500 o 1000 filas por página (paginación del servidor)

---

## Informe de Reservas

Vista completa de todas las reservas con información detallada.

**Columnas principales:**
- ID, Código de reserva del canal
- Nombre y apellidos del huésped
- Tipología, Habitación, Número de puerta
- Teléfono, Email, Nacionalidad
- Fecha de creación, Llegada, Salida, Noches
- Ocupación, Régimen, Pack, Código promocional
- Adultos, Niños
- Precio de alojamiento, Comisión
- Política, Facturado (sí/no)
- Notas, Notas planas, Motivo de estado
- Empresa, Nombre de empresa
- Fecha de expiración, Estado, Fecha de cancelación
- Origen, Total, Total pagado, Total pendiente, Total artículos
- Consentimiento de marketing, Usuario que creó

**Filtros especiales:**
- Estado: Confirmada, Tentativa, Cancelada, No-show
- Política: Flexible, No reembolsable
- Régimen: SA, AD, MP, PC, TI
- Facturado: Sí/No
- Empresa: Sí/No
- Consentimiento marketing: Sí/No
- Motivo de estado

**Indicadores visuales:** Las reservas canceladas y tentativas se muestran con estilos diferenciados.

---

## Informe de Facturas

**Columnas principales:**
- Prefijo, Referencia
- Tipo: Factura, Proforma o Nota de crédito
- Código RS
- Fecha de emisión
- Total, Total pagado, Total pendiente
- Base imponible, Impuestos, IRPF
- Observaciones
- Llegada, Salida
- Tipo de habitación, Número de puerta

**Filtros:** Por tipo de documento, fechas, importes.

---

## Informe de Llegadas

Reservas con llegada en el período seleccionado.

**Columnas principales:**
- ID, Nombre, Apellidos
- Pago pendiente, Estado de check-in
- Habitación, Número de puerta
- Adultos, Niños
- Número de reserva del canal
- Fecha y hora de llegada, Fecha de salida
- Noches, Régimen
- Notas del cliente, Notas internas, Origen

**Filtro por defecto:** Fecha de llegada = hoy.

---

## Informe de Salidas

Reservas con salida en el período seleccionado.

**Columnas principales:**
- ID, Nombre, Apellidos, Teléfono
- Habitación, Número de puerta
- Adultos, Niños
- Número de reserva del canal
- Fecha de llegada, Fecha y hora de salida
- Noches, Régimen
- Estado de check-out
- Notas del cliente, Notas internas, Origen

---

## Informe de Pagos

Todos los pagos registrados en el período.

**Columnas principales:**
- Código RS, Nombre, Apellidos
- Fecha de pago, Código de operación
- Factura asociada, Facturado (sí/no)
- Fecha de emisión de factura
- Llegada, Salida
- Total, Método de pago
- Notas, Origen, Prepago (sí/no)

---

## Informe de In-House (Huéspedes Actuales)

Huéspedes actualmente alojados en la propiedad.

**Columnas principales:**
- Nombre, Apellidos
- Nacionalidad, Número de documento
- Habitación, Número de puerta
- Régimen, Email, Edad
- Llegada, Salida, Noches
- Notas, Fuente/Origen

---

## Informe de Huéspedes (Hosts)

Listado detallado de todos los huéspedes registrados.

**Columnas principales:**
- ID, ID de reserva, Propiedad
- Nombre, Apellidos, Email, Teléfono
- Nacionalidad, Idioma, País
- Código postal, Origen
- Fecha de creación, Llegada, Salida
- Estado, Tipología
- Adultos, Niños
- Nombre y apellidos del titular de la reserva
- Consentimiento de marketing, Edad, Fecha de nacimiento
- NIF/CIF, Ciudad, Provincia, Dirección, Notas

---

## Informe de Orígenes

Análisis de reservas agrupadas por canal de origen.

**Columnas principales:**
- Agencia/Canal
- Total de reservas (confirmadas y canceladas)
- Importe total (confirmadas y canceladas)
- Total de noches confirmadas
- Fecha de llegada, Fecha de salida

---

## Informe de Nacionalidades

Análisis de reservas agrupadas por nacionalidad.

**Columnas principales:**
- Nacionalidad
- Total de reservas, Confirmadas, Canceladas
- Fecha de llegada
- Importe total de estancia, Importe de extras
- Noches confirmadas, Noches canceladas
- ALOS (Estancia media)
- Lead Time (Antelación de reserva)
- Adultos, Niños, Bebés
- ADR (Tarifa media diaria)

---

## Informe de Morosos (Overdues)

Reservas con pagos pendientes o facturas vencidas.

**Columnas principales:**
- Nombre, Apellidos
- Número de reserva
- Llegada, Salida
- Fecha de factura, Fecha de recepción
- Referencia de factura
- Total, Pagado, Pendiente
- Origen

---

## Informe de Empresas

Listado de empresas y agencias registradas.

**Columnas principales:**
- Nombre de empresa, Nombre comercial
- Email, Teléfono
- Dirección, Código postal, Ciudad, País
- NIF/CIF, Contabilidad

---

## Informe de Artículos

Detalle de todos los productos y servicios vendidos.

**Columnas principales:**
- Reserva, Fecha de creación
- Inicio y fin del servicio
- Fecha de factura, Categoría, Artículo
- Estado de reembolso, Tipo de artículo
- Cantidad de impuestos, Base, Impuestos, Total
- Usuario, Pedido externo, Unidades vendidas

---

## Informe de Autoridades

Estado de los envíos a autoridades (partes de viajeros).

**Columnas principales:**
- Propiedad, Reserva
- Fecha de creación, ID de transacción
- Tipo de evento, Tipo de autoridad
- Estado, Error, Fecha de reintento

---

## Informes Adicionales (Backoffice)

Los siguientes informes están disponibles a través del backoffice de Hotelgest:
- Contabilidad
- Limpiezas
- Producción
- Ocupación
- Régimen (Boards)
- Cartera
- Cierre del día
- Impuestos
- INE (Instituto Nacional de Estadística)
- Policía
- Tasa turística
- Caja diaria
