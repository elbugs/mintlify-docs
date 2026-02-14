# 05 - Facturación y Pagos

**URL:** La facturación se gestiona desde el detalle de cada reserva: [https://app.hotelgest.com/dashboard](https://app.hotelgest.com/dashboard) → abre una reserva para ver Facturas, Proformas, Pagos y Depósitos.

Hotelgest Unified ofrece un sistema completo de gestión financiera vinculado a las reservas: facturas, proformas, pagos y depósitos.

---

## Facturas

### Crear una factura
1. Abre el detalle de una reserva
2. En la sección de **Facturas**, haz clic en **Añadir factura**
3. Selecciona los productos/servicios a incluir
4. Revisa los importes, impuestos y totales
5. Confirma la creación

### Tipos de factura
| Tipo | Descripción |
|------|-------------|
| **Factura** | Documento fiscal estándar |
| **Proforma** | Documento previo a la factura (sin validez fiscal) |
| **Nota de crédito** | Rectificación o devolución |

### Estados de factura
- **Borrador**: Factura creada pero no finalizada
- **Emitida**: Factura emitida y con validez fiscal
- **Pagada**: Factura completamente pagada
- **Parcialmente pagada**: Se ha recibido un pago parcial
- **Anulada**: Factura cancelada

### Información de la factura
- **Prefijo y referencia**: Numeración automática configurable
- **Fecha de emisión**
- **Datos del cliente**: Nombre, dirección, NIF/CIF
- **Líneas de detalle**: Productos, cantidades, precios unitarios
- **Base imponible**: Importe antes de impuestos
- **Impuestos**: IVA y otros impuestos aplicables
- **IRPF**: Retención si procede
- **Total**: Importe final
- **Observaciones**: Notas adicionales

### Acciones sobre facturas
- **Enviar por email**: Enviar la factura al huésped
- **Descargar PDF**: Generar y descargar el documento
- **Vista previa**: Visualizar antes de enviar
- **Anular**: Cancelar la factura (genera nota de crédito si es necesario)

---

## Proformas

Las proformas son documentos previos a la factura que permiten:
- Mostrar al huésped el desglose de costes antes de emitir la factura
- Solicitar confirmación de los servicios
- Enviar como presupuesto o estimación

### Crear una proforma
1. En el detalle de la reserva, sección **Proformas**
2. Haz clic en **Añadir proforma**
3. Selecciona los productos/servicios
4. Confirma la creación

### Acciones
- **Enviar por email**
- **Descargar PDF**
- **Convertir a factura**: Transforma la proforma en factura definitiva

---

## Pagos

### Registrar un pago
1. En el detalle de la reserva, sección **Pagos**
2. Haz clic en **Añadir pago**
3. Selecciona el **método de pago**
4. Introduce el **importe**
5. Asocia a una factura (opcional)
6. Añade notas si es necesario
7. Confirma el pago

### Métodos de pago
- Efectivo
- Tarjeta de crédito/débito
- Transferencia bancaria
- TPV virtual
- Pasarela de pago online
- Otros métodos configurables

### Estados de pago
- **Pendiente**: Pago registrado pero no confirmado
- **Completado**: Pago recibido correctamente
- **Rechazado**: Pago rechazado por la entidad
- **Reembolsado**: Pago devuelto al huésped

### Solicitudes de pago
Se pueden enviar solicitudes de pago al huésped:
1. Selecciona el importe a cobrar
2. El sistema genera un enlace de pago seguro
3. Se envía al huésped por email o WhatsApp
4. El huésped realiza el pago online

---

## Depósitos

Los depósitos son pagos anticipados o garantías asociados a la reserva.

### Tipos de depósito
- **Señal**: Pago parcial para confirmar la reserva
- **Garantía**: Fianza de seguridad
- **Prepago**: Pago anticipado total

### Registrar un depósito
1. En el detalle de la reserva, sección **Depósitos**
2. Haz clic en **Añadir depósito**
3. Selecciona el tipo y método de pago
4. Introduce el importe
5. Confirma

---

## Descuentos

Se pueden aplicar descuentos a las reservas:
- **Porcentaje**: Descuento en porcentaje sobre el total
- **Importe fijo**: Cantidad fija de descuento
- **Código promocional**: Descuento vinculado a un código de promoción

---

## Productos y Servicios

Cada reserva puede tener productos y servicios asociados:
- **Alojamiento**: Producto principal (noches de estancia)
- **Servicios adicionales**: Parking, spa, minibar, etc.
- **Impuestos**: Tasa turística y otros impuestos adicionales
- **Productos personalizados**: Cualquier producto definido por el usuario

### Gestionar productos
1. En el detalle de la reserva, sección **Productos**
2. **Añadir producto**: Selecciona del catálogo o crea uno personalizado
3. **Editar**: Modifica cantidad, precio o fechas
4. **Eliminar**: Quita un producto de la reserva

---

## Configuración de Facturación

La configuración de facturación se gestiona desde **Configuración > Contabilidad**:
- **Datos de la empresa**: Nombre fiscal, NIF/CIF, dirección
- **Prefijos de numeración**: Para facturas, proformas y notas de crédito
- **Impuestos**: Configuración de IVA y otros impuestos
- **Campos obligatorios**: Qué datos son requeridos
- **Hora de cierre**: Hora de cierre contable diario
- **Pie de factura**: Texto que aparece en la parte inferior de las facturas
