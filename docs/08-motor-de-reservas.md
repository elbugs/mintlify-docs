# Motor de reservas (Booking Engine)

**URL:** [https://app.hotelgest.com/booking-engine](https://app.hotelgest.com/booking-engine)

El Motor de Reservas permite a los huéspedes realizar reservas directas a través de tu página web, sin intermediarios ni comisiones de OTAs.

---

## Descripción General

El Booking Engine es una interfaz pública integrable en tu sitio web que permite:
- Consultar **disponibilidad** en tiempo real
- Ver **tarifas** y **tipos de habitación**
- Aplicar **códigos promocionales**
- Completar el proceso de **reserva y pago** online
- Consultar las **políticas** de cancelación

---

## Flujo de Reserva para el Huésped

### 1. Consulta de disponibilidad
- El huésped selecciona las fechas de llegada y salida
- Indica el número de huéspedes (adultos, niños, bebés)
- El sistema muestra las habitaciones disponibles con precios

### 2. Selección de habitación
- Se muestran los tipos de habitación disponibles con:
  - Fotos de la habitación
  - Descripción
  - Capacidad (personas máximas)
  - Servicios incluidos
  - Precio por noche y total
  - Régimen disponible (SA, AD, MP, PC, TI)

### 3. Datos del huésped
- Nombre y apellidos
- Email
- Teléfono
- Observaciones o peticiones especiales

### 4. Política de cancelación
- El huésped puede elegir entre las políticas configuradas:
  - **Flexible**: Cancelación gratuita hasta X días antes
  - **No reembolsable**: Precio reducido sin posibilidad de cancelación gratuita

### 5. Código promocional
- Campo opcional para introducir un código de descuento
- El sistema valida y aplica el descuento automáticamente

### 6. Pago
- El huésped completa el pago a través de la pasarela configurada
- Se confirma la reserva automáticamente

### 7. Confirmación
- El huésped recibe un email de confirmación con:
  - Detalles de la reserva
  - Número de referencia
  - Política de cancelación aplicada
  - Instrucciones de llegada

---

## Configuración del Motor de Reservas

### Acceso
Desde el menú lateral, haz clic en **Motor de Reservas**.

### Opciones configurables

#### Información general
- Activar/desactivar el motor de reservas
- URL personalizada
- Logo e imagen de marca

#### Habitaciones y tarifas
- Seleccionar qué tipos de habitación se muestran
- Configurar tarifas públicas
- Establecer restricciones (estancia mínima, cierre de ventas, etc.)

#### Políticas
- Definir políticas de cancelación disponibles
- Configurar plazos y condiciones
- Establecer política por defecto

#### Códigos promocionales
- Crear y gestionar códigos de descuento
- Establecer validez (fechas de inicio y fin)
- Definir el tipo de descuento (porcentaje o importe fijo)
- Limitar el uso (número máximo de usos)

#### Pagos
- Configurar la pasarela de pago
- Definir si se cobra el total, un porcentaje o solo una señal
- Establecer métodos de pago aceptados

#### Personalización
- Colores y estilo visual
- Textos personalizados
- Idiomas disponibles

---

## Integración en tu Web

El motor de reservas se puede integrar en tu sitio web de varias formas:
- **Enlace directo**: URL que lleva directamente al motor
- **Widget embebido**: Código HTML para insertar en tu web
- **Botón de reserva**: Botón personalizable para tu página

---

## Gestión de Reservas del Motor

Las reservas realizadas a través del motor aparecen en el sistema como cualquier otra reserva:
- Se muestran en el **calendario de planificación**
- Aparecen en los **informes de reservas**
- El origen se identifica como reserva directa del Booking Engine
- Puedes gestionarlas (editar, facturar, hacer check-in) como cualquier otra reserva
