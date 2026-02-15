---
title: Facturación y pagos
description: Facturas, proformas, pagos, depósitos, impuestos y métodos de pago en Hotelgest Unified.
---

# Cómo gestionar la facturación y los pagos

**Para qué sirve.** La facturación y los pagos se gestionan desde la ficha de cada reserva. Ahí puede emitir facturas y proformas, registrar los pagos que recibe del huésped y gestionar depósitos. Todo queda ligado a la reserva, así no se pierde el rastro de lo cobrado.

**Dónde está.** Abra una reserva desde el Panel de Control o desde el calendario de Planificación. Dentro de la reserva verá la sección de Facturación en la parte inferior. No puede romper nada por abrirla: solo al pulsar "Añadir factura" o "Añadir pago" y luego "Guardar" se registran cambios.

---

## Facturas

### Crear una factura

1. Abre el detalle de una reserva.
2. En la sección de **Facturas**, haz clic en **Añadir factura**.
3. Selecciona los productos/servicios a incluir.
4. Revisa los importes, impuestos y totales.
5. Confirma la creación.

### Tipos de documento

| Tipo | Descripción |
|------|-------------|
| **Factura** | Documento fiscal estándar con validez legal |
| **Proforma** | Documento previo a la factura, sin validez fiscal |
| **Nota de crédito** | Rectificación o devolución de una factura |
| **Factura de servicio** | Factura de servicios adicionales |

### Estados de factura

| Estado | Descripción |
|--------|-------------|
| **Borrador** | Factura creada pero no finalizada |
| **Emitida** | Factura emitida con validez fiscal |
| **Pagada** | Factura completamente pagada |
| **Parcialmente pagada** | Se ha recibido un pago parcial |
| **Anulada** | Factura cancelada |

### Información de la factura

Cada factura contiene:
- **Prefijo y referencia**: numeración automática configurable por propiedad. Puedes tener prefijos diferentes para facturas, proformas, servicios y notas de crédito.
- **Fecha de emisión**
- **Datos del cliente**: nombre, dirección, NIF/CIF
- **Líneas de detalle**: productos, cantidades, precios unitarios
- **Base imponible**: importe antes de impuestos
- **Impuestos**: IVA y otros impuestos aplicables
- **IRPF**: retención si procede
- **Total**: importe final
- **Observaciones**: notas adicionales

### Acciones sobre facturas

| Acción | Qué hace |
|--------|----------|
| **Enviar por email** | Envía la factura en PDF al huésped |
| **Descargar PDF** | Genera y descarga el documento |
| **Vista previa** | Visualiza antes de enviar |
| **Anular** | Cancela la factura (genera nota de crédito si es necesario) |
| **Reembolsar** | Crea una nota de crédito asociada |

---

## Proformas

Las proformas son documentos previos a la factura que permiten:
- Mostrar al huésped el desglose de costes antes de emitir la factura.
- Solicitar confirmación de los servicios.
- Enviar como presupuesto o estimación.

### Crear una proforma

1. En el detalle de la reserva, sección **Proformas**.
2. Haz clic en **Añadir proforma**.
3. Selecciona los productos/servicios.
4. Confirma la creación.

### Acciones

- **Enviar por email**: envía la proforma al huésped.
- **Descargar PDF**: genera el documento.
- **Convertir a factura**: transforma la proforma en factura definitiva.

---

## Pagos

### Registrar un pago

1. En el detalle de la reserva, sección **Pagos**.
2. Haz clic en **Añadir pago**.
3. Selecciona el **método de pago**.
4. Introduce el **importe**.
5. Asocia a una factura (opcional).
6. Añade notas si es necesario.
7. Confirma el pago.

### Métodos de pago disponibles

| Método | Descripción |
|--------|-------------|
| **Efectivo** (Cash) | Pago en efectivo |
| **Tarjeta de crédito** (Credit Card) | Pago con tarjeta estándar |
| **Transferencia bancaria** (Bank Transfer) | Transferencia desde cuenta bancaria |
| **TPV Virtual** (Virtual POS) | Pago por Redsys |
| **Monei** | Pago a través de Monei |
| **Paycomet** | Pago a través de Paycomet |
| **Stripe** | Pago a través de Stripe |
| **Bizum** | Pago por Bizum |
| **PayPal** | Pago por PayPal |
| **American Express** (Amex) | Pago con tarjeta Amex |
| **Cheque** (Paycheck) | Pago con cheque |
| **Crédito** (Credit) | Crédito a favor del huésped |
| **CashDro** | Pago por CashDro |
| **Otros** | Otros métodos |

### Tipos de pago virtual (TPV)

Al usar pasarelas de pago (Redsys, Monei, Paycomet, Stripe), hay tres modalidades:

| Tipo | Descripción |
|------|-------------|
| **Pago directo** | Cobra el importe completo en el momento |
| **Prepago** | Cobro anticipado antes de la estancia |
| **Pago parcial** | Cobra una parte del total |

### Solicitudes de pago

Puedes enviar una solicitud de pago al huésped:
1. Selecciona el importe a cobrar.
2. El sistema genera un enlace de pago seguro.
3. Se envía al huésped por email o WhatsApp.
4. El huésped realiza el pago online a través de la pasarela.

### Acciones sobre pagos

| Acción | Qué hace |
|--------|----------|
| **Enviar por email** | Envía el recibo del pago al huésped |
| **Descargar simplificado** | Descarga un recibo simplificado en PDF |
| **Reembolsar** | Devuelve el importe al huésped. Solo Monei y Paycomet permiten reembolsos automáticos por TPV |
| **Convertir a anticipo** | Convierte un pago normal en un anticipo |

---

## Depósitos

Los depósitos son pagos anticipados o garantías asociados a la reserva.

### Tipos de depósito

| Tipo | Descripción |
|------|-------------|
| **Depósito** | Señal, fianza o prepago |
| **Reembolso** | Devolución de un depósito previo |

### Registrar un depósito

1. En el detalle de la reserva, sección **Depósitos**.
2. Haz clic en **Añadir depósito**.
3. Selecciona el tipo y método de pago.
4. Introduce el importe.
5. Confirma.

### Acciones sobre depósitos

- **Reembolsar**: devuelve el depósito al huésped.
- **Convertir a pago**: transforma el depósito en un pago definitivo asociado a una factura.

---

## Productos y Servicios

Cada reserva puede tener productos y servicios asociados:

| Tipo | Descripción |
|------|-------------|
| **Alojamiento** | Producto principal (noches de estancia) |
| **Servicios adicionales** | Parking, spa, minibar, etc. |
| **Tasa turística** | Se genera automáticamente según la configuración de impuestos |
| **Productos personalizados** | Cualquier producto definido por el usuario |

### Gestionar productos

1. En el detalle de la reserva, sección **Productos**.
2. **Añadir producto**: selecciona del catálogo o crea uno personalizado.
3. **Editar**: modifica cantidad, precio, fechas de inicio/fin o impuestos.
4. **Eliminar**: quita un producto de la reserva.
5. **Reembolsar**: crea un reembolso para el producto.

Cada producto tiene:
- Precio base
- Impuesto principal (IVA u otro)
- Impuesto secundario (si aplica)
- Descuento (porcentaje o importe fijo)
- Fechas de servicio (inicio y fin)

---

## Impuestos

### Impuesto general
Se aplica como porcentaje sobre el precio base de los productos. Se configura desde **Configuración > Impuestos**.

### Tasa turística
Se genera automáticamente en las reservas según la configuración:

| Campo | Descripción |
|-------|-------------|
| **Precio por adulto** | Importe por adulto y noche (sin impuestos) |
| **Precio por niño** | Importe por niño y noche (sin impuestos) |
| **Máximo de días** | Número máximo de noches que se cobra la tasa |
| **Sobrescritura** | Tarifas diferentes para períodos concretos (temporada alta, etc.) |

### Recargo municipal
Funciona igual que la tasa turística pero como recargo adicional.

---

## Descuentos

Se pueden aplicar descuentos a las reservas:
- **Porcentaje**: descuento en porcentaje sobre el total.
- **Importe fijo**: cantidad fija de descuento.
- **Código promocional**: descuento vinculado a un código.

---

## Firma digital de facturas

Si tienes activa la integración con **Verifactu** o **TicketBai**, las facturas se firman digitalmente de forma automática al emitirlas. Consulta [Integraciones](/docs/12-integraciones) para más detalles.

---

## Configuración de Facturación

La configuración se gestiona desde **Configuración > Contabilidad**:

| Ajuste | Descripción |
|--------|-------------|
| **Datos fiscales** | Nombre legal, NIF/CIF, dirección fiscal |
| **Prefijos de numeración** | Prefijos independientes para facturas, proformas, servicios y notas de crédito |
| **Numeración adicional** | Prefijo numérico adicional para series |
| **Impuestos** | IVA, tasa turística, recargo municipal |
| **Campos obligatorios** | Qué datos son requeridos al generar facturas |
| **Pie de factura** | Texto legal que aparece en la parte inferior |

---

## Qué puede ir mal y cómo solucionarlo

**No veo el botón de añadir factura o añadir pago.** Compruebe que está dentro de la ficha de una reserva y en la sección de Facturación. Si no la ve, su rol puede no tener permiso para facturar; pregunte a su administrador.

**He registrado un pago con un importe equivocado.** Puede editar o anular el pago desde la misma pantalla. Si el pago ya está cerrado, contacte con su administrador.

**La factura no se puede emitir (mensaje de error).** Suele faltar un dato obligatorio: NIF del cliente o dirección fiscal. Lea el mensaje en pantalla.

**No me llega el email con la factura al huésped.** Revise que el correo del huésped esté bien escrito. Pida que mire la carpeta de spam. Puede volver a enviar desde la misma pantalla.

**Recuerde.** Sus datos de facturación quedan guardados. Si se equivoca, puede pedir ayuda para corregirlo.

---

## Permisos necesarios

| Permiso | Qué permite |
|---------|-------------|
| Ver facturas | Ver la sección de facturas |
| Crear facturas | Emitir nuevas facturas |
| Editar facturas | Modificar facturas existentes |
| Eliminar facturas | Eliminar facturas |
| Reembolsar facturas | Crear notas de crédito |
| Enviar facturas | Enviar por email |
| Ver proformas | Ver la sección de proformas |
| Crear proformas | Emitir nuevas proformas |
| Enviar proformas | Enviar proformas por email |
| Ver pagos | Ver la sección de pagos |
| Crear pagos | Registrar nuevos pagos |
| Editar pagos | Modificar pagos |
| Eliminar pagos | Eliminar pagos |
| Reembolsar pagos | Procesar reembolsos |

---

## Consejos

- Antes de emitir la factura definitiva, puede enviar una **proforma** al huésped para que confirme el desglose.
- Registre los pagos en cuanto los reciba; así la reserva mostrará siempre el saldo actualizado.
- Si descarga facturas en PDF, guárdelas en su ordenador o envíelas por email.

**Ver también:** [Reservas](/docs/04-reservas), [Configuración](/docs/11-configuracion), [Integraciones](/docs/12-integraciones).
