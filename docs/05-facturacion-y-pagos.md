# Cómo gestionar la facturación y los pagos

**Para qué sirve.** La facturación y los pagos se gestionan desde la ficha de cada reserva. Ahí puede emitir facturas y proformas, registrar los pagos que recibe del huésped (efectivo, tarjeta, transferencia) y ver depósitos. Todo queda ligado a la reserva, así no se pierde el rastro de lo cobrado.

**Dónde está.** Abra una reserva desde el Panel de Control o desde el calendario de Planificación. Dentro de la reserva verá varias **pestañas** (solapas); una de ellas es Facturación (o Facturas / Pagos). Al pulsar en esa pestaña verá la lista de facturas, proformas y pagos de esa reserva. No puede romper nada por abrir la pestaña: solo al pulsar "Añadir factura" o "Añadir pago" y luego "Guardar" se registran cambios.

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

---

## Qué puede ir mal y cómo solucionarlo

**No veo el botón de añadir factura o añadir pago.** Compruebe que está dentro de la ficha de una reserva y en la pestaña de Facturación o Pagos. Si no ve esa pestaña, su perfil (rol) puede no tener permiso para facturar; pregunte a su administrador.

**He registrado un pago con un importe equivocado.** Si acaba de guardar, en algunas pantallas puede haber una opción para editar o anular el pago. Si no la ve o el pago ya está cerrado, contacte con su administrador o con soporte; suelen poder corregirlo.

**La factura no se puede emitir (mensaje de error).** Suele faltar un dato obligatorio: por ejemplo el NIF del cliente o la dirección fiscal. Lea el mensaje que aparece en pantalla; indicará qué campo completar. Complete el dato y vuelva a intentar. Mientras no pulse Emitir o Guardar, la factura no se registra.

**No me llega el email con la factura al huésped.** Revise que el correo del huésped esté bien escrito en la reserva. Pida al huésped que mire la carpeta de spam. Puede volver a enviar la factura desde la misma pantalla (botón Enviar por email).

**Recuerde.** Sus datos de facturación y pagos quedan guardados. Si se equivoca al introducir un pago o una factura, no se pierde nada por pedir ayuda para corregirlo. Para dudas sobre impuestos o numeración, el administrador o la configuración de Contabilidad son la referencia.

---

## Consejos

- Antes de emitir la factura definitiva, puede enviar una **proforma** al huésped para que confirme el desglose.
- Registre los pagos en cuanto los reciba; así la reserva mostrará siempre el saldo actualizado.
- Si descarga facturas en PDF, guárdelas en una carpeta de su ordenador o envíelas por email al cliente para tener copia.

**Ver también:** [Reservas](/docs/04-reservas), [Configuración](/docs/11-configuracion), [Resolución de problemas](/docs/18-resolucion-problemas).
