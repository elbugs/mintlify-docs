# 12 - Integraciones

**URL Marketplace (catálogo de integraciones):** [https://app.hotelgest.com/marketplace](https://app.hotelgest.com/marketplace)  
**Configuración de integraciones:** desde [Configuración](https://app.hotelgest.com/settings) y las secciones específicas de cada integración.

Hotelgest Unified se integra con múltiples servicios externos para automatizar procesos, cumplir con la legislación y ampliar las funcionalidades del PMS.

---

## Autoridades Españolas

El sistema permite el envío automático y manual de los partes de viajeros a las autoridades competentes según la comunidad autónoma.

### Ertzaintza (País Vasco)
- Envío de partes de viajeros a la Ertzaintza
- Registro de huéspedes conforme a la normativa vasca
- Envío automático al hacer check-in o manual desde la reserva

### SES (Servicio Español de Seguridad)
- Envío de partes al sistema SES
- Cumplimiento de la normativa estatal de registro de viajeros

### Mossos d'Esquadra (Cataluña)
- Envío de partes de viajeros a los Mossos d'Esquadra
- Cumplimiento de la normativa catalana

### Flujo de envío
1. Al hacer **check-in** de un huésped, los datos se preparan automáticamente
2. El sistema envía el parte a la autoridad correspondiente
3. Puedes ver el **estado del envío** en el informe de Autoridades:
   - **Enviado**: Parte enviado correctamente
   - **Error**: Fallo en el envío (con detalle del error)
   - **Pendiente de reintento**: Se reintentará automáticamente

### Envío manual
Desde el detalle de la reserva, haz clic en **Autoridades** para enviar o reenviar el parte manualmente.

---

## Firma Digital

### Verifactu
- Sistema de **facturación electrónica** conforme a la normativa española
- Firma digital de facturas para garantizar su integridad
- Generación de código QR de verificación en las facturas

### TicketBai (País Vasco)
- Sistema de facturación obligatorio en el País Vasco
- Firma y envío de facturas a la Hacienda Foral
- Cadena de facturación inalterable

---

## Channel Manager (Channex)

Integración con Channex para la distribución de habitaciones y tarifas en múltiples OTAs.

### Funcionalidades
- **Sincronización de disponibilidad**: Actualización en tiempo real del inventario en todas las OTAs
- **Sincronización de tarifas**: Precios actualizados automáticamente
- **Recepción de reservas**: Las reservas de OTAs se importan automáticamente
- **Prevención de overbooking**: Al recibir una reserva, la disponibilidad se actualiza en todos los canales

### OTAs soportadas
- Booking.com
- Expedia
- Airbnb
- Y otros canales conectados a Channex

### Configuración
Ver **Configuración > Channel Manager** para los pasos de configuración.

---

## Cerraduras Electrónicas (Doors)

Integración con sistemas de cerraduras electrónicas para acceso sin llave.

### Funcionalidades
- **Códigos de acceso**: Generación automática de códigos PIN para los huéspedes
- **Llaves digitales**: Envío de llaves electrónicas al móvil del huésped
- **Control de acceso**: Gestión de permisos de acceso por habitación y período
- **Registro de accesos**: Historial de entradas y salidas

### Acceso desde la reserva
Desde el detalle de la reserva, haz clic en **Llaves** para:
- Ver los códigos de acceso activos
- Generar nuevos códigos
- Desactivar códigos anteriores

---

## TV (Yuvod)

Integración con el sistema de TV interactiva Yuvod.

### Funcionalidades
- Personalización de la pantalla de bienvenida del televisor
- Información del huésped en la TV de la habitación
- Servicios del hotel accesibles desde la TV

---

## CRM

### Clientify
- Sincronización de datos de huéspedes con Clientify
- Seguimiento de clientes y campañas

### Pipedrive
- Integración con Pipedrive CRM
- Sincronización de contactos, negocios y organizaciones
- Webhooks para eventos de reserva

---

## Marketplace

El **Marketplace** es el catálogo de todas las integraciones disponibles en Hotelgest Unified.

### Acceso
Desde el menú lateral o inferior, haz clic en **Marketplace**.

### Funcionalidades
- **Explorar integraciones**: Ver todas las integraciones disponibles organizadas por categoría
- **Activar/Desactivar**: Conectar o desconectar integraciones
- **Configurar**: Ajustar los parámetros de cada integración
- **Estado**: Ver el estado de cada integración (activa, inactiva, error)

### Categorías de integraciones
- Autoridades y cumplimiento legal
- Firma digital y facturación
- Channel Manager y distribución
- Cerraduras y acceso
- TV y entretenimiento
- CRM y marketing
- Comunicación
- Pasarelas de pago

---

## Webhooks

Los webhooks permiten enviar datos automáticamente a sistemas externos cuando ocurren eventos en Hotelgest.

### Webhooks salientes
Envían información a URLs configuradas cuando:
- Se crea, modifica o cancela una reserva
- Se hace check-in o check-out
- Se registra un pago
- Otros eventos configurables

### Webhooks entrantes
Reciben información de sistemas externos:
- Reservas de OTAs
- Actualizaciones de disponibilidad
- Otros datos de integraciones

### Configuración
Ver **Configuración > Webhooks** para gestionar los webhooks.

---

## API Pública

Hotelgest Unified ofrece una API REST pública para integraciones personalizadas.

### Acceso
- Se requiere una **API Key** (ver Configuración > API Keys)
- La API Key se envía en la cabecera `x-api-key`

### Documentación
La documentación de la API está disponible en formato Swagger/OpenAPI.

### Casos de uso
- Integrar con software de contabilidad propio
- Sincronizar con otros sistemas del hotel
- Construir aplicaciones personalizadas sobre el PMS
