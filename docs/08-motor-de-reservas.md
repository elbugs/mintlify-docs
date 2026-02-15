---
title: Motor de reservas
description: Configuración y funcionamiento del motor de reservas directas (Booking Engine) de Hotelgest Unified.
---

# Motor de reservas (Booking Engine)

El Motor de Reservas es la página web donde tus huéspedes pueden reservar directamente, sin comisiones de intermediarios. Cada propiedad tiene su propia URL de reservas que puedes compartir en tu web, redes sociales o emails.

**URL de configuración:** [app.hotelgest.com/booking-engine](https://app.hotelgest.com/booking-engine)
**URL del motor para huéspedes:** `https://bookings.hotelgest.com/{tu-id-de-propiedad}`

---

## Cómo lo ve el huésped

Cuando un huésped abre la URL del motor de reservas, sigue estos pasos:

### 1. Seleccionar fechas
El huésped elige la fecha de llegada y la fecha de salida.

### 2. Ver habitaciones disponibles
Se muestran los tipos de habitación disponibles para esas fechas, con:
- Fotos de la habitación (galería de imágenes)
- Descripción del tipo de habitación
- Capacidad (adultos, niños)
- Servicios y pensión (solo alojamiento, desayuno, media pensión, etc.)
- Precio por noche y precio total

### 3. Seleccionar habitación
El huésped elige el tipo de habitación que quiere.

### 4. Código promocional (opcional)
Si tienes códigos promocionales activos, el huésped puede introducir uno para obtener un descuento.

### 5. Productos y extras (opcional)
Si has configurado productos adicionales (parking, cuna, pack romántico, etc.), el huésped puede añadirlos a su reserva con la cantidad deseada.

### 6. Datos del huésped
El huésped rellena sus datos:
- Nombre y apellidos
- Email y teléfono
- Dirección, ciudad, código postal, provincia, país
- Idioma preferido
- NIF/CIF (opcional)
- Notas (opcional)

### 7. Seleccionar política de cancelación
Si hay varias políticas disponibles, el huésped elige la que prefiera.

### 8. Pagar
El huésped realiza el pago a través de la pasarela configurada (Redsys o Monei).

### 9. Confirmación
El huésped recibe un email de confirmación con los detalles de su reserva y el número de referencia.

---

## Cómo configurar el motor de reservas

### Acceder a la configuración

1. Ve al menú lateral y haz clic en **Motor de reservas**.
2. Se abre la página de configuración con un iframe que muestra cómo se ve tu motor.

### Personalización visual

Puedes personalizar el aspecto del motor:

| Opción | Qué hace |
|--------|----------|
| **Color primario** | Color principal de los botones y elementos destacados (formato hexadecimal, ejemplo: #0D9373) |
| **Color secundario** | Color de acentos y fondos (formato hexadecimal) |
| **Radio de borde del botón** | Forma de los botones: cuadrado (square), redondeado (round) o circular (full) |
| **Google Tag Manager** | ID de GTM para seguimiento (formato: GTM-XXXXXXX). Opcional |

### Información de la propiedad

La información que se muestra en el motor se toma de la configuración de la propiedad:
- Nombre de la propiedad (multilingüe)
- Descripción (multilingüe)
- Dirección, ciudad, provincia, país
- Logo
- Galería de imágenes con descripciones
- Información adicional (multilingüe)
- Firma legal (multilingüe)

---

## Políticas de cancelación

Las políticas de cancelación se configuran desde la sección de configuración de la propiedad. Hay dos tipos:

- **Políticas estándar**: aplicables a todas las reservas.
- **Políticas personalizadas**: aplicables a tipos de habitación o períodos concretos.

El huésped ve las políticas disponibles durante el proceso de reserva y elige una.

---

## Códigos promocionales

Puedes crear códigos de descuento para que los huéspedes los usen al reservar.

Cada código tiene:
- **Código**: texto que el huésped introduce (ejemplo: VERANO2026)
- **Fechas de validez**: desde y hasta cuándo se puede usar
- **Tipo de descuento**: porcentaje o importe fijo
- **Valor**: cantidad del descuento
- **Nombre**: descripción interna

---

## Productos y extras

Puedes ofrecer productos adicionales que el huésped añade a su reserva:

Cada producto tiene:
- **Nombre** (multilingüe)
- **Descripción** (multilingüe, opcional)
- **Precio**
- **Categoría** (opcional)
- **Imagen** (opcional)
- **Tipo de pago**: cómo se cobra
- **Restricciones**: puede estar limitado a ciertos tipos de habitación

---

## Pasarelas de pago

El motor de reservas soporta dos pasarelas de pago:

### Redsys
Pasarela de pago española. El huésped es redirigido a la página de Redsys para completar el pago con tarjeta.

### Monei
Pasarela de pago alternativa. El huésped es redirigido a la URL de Monei para pagar.

La pasarela se configura desde **Marketplace** en la sección de integraciones de pago.

---

## Integrar el motor en tu web

Hay tres formas de usar el motor de reservas:

### 1. Enlace directo
Comparte la URL `https://bookings.hotelgest.com/{tu-id}` en tu web, emails o redes sociales.

### 2. Iframe embebido
Incrusta el motor directamente en tu página web con un iframe:

```html
<iframe src="https://bookings.hotelgest.com/{tu-id}" width="100%" height="800px" frameborder="0"></iframe>
```

### 3. Botón de reserva
Crea un botón en tu web que enlace a la URL del motor.

---

## Impuestos y tasas

El motor puede aplicar impuestos automáticamente:

- **Tasa por adulto**: importe por adulto y noche.
- **Máximo por día**: límite máximo de tasa diaria.
- **Sobrescritura por fechas**: puedes definir tasas diferentes para períodos concretos (por ejemplo, temporada alta).

---

## Idiomas

El motor de reservas está disponible en 9 idiomas:
Español, Inglés, Italiano, Catalán, Francés, Alemán, Euskera, Ruso, Gallego.

El idioma se detecta automáticamente del navegador del huésped, pero puede cambiarse manualmente.

---

## Identificación de las reservas

Las reservas que llegan a través del motor se identifican con:
- **Canal**: "Booking Engine" / "Motor de reservas"
- **Código de canal**: 999
- **Código de referencia**: generado automáticamente

Puedes ver estas reservas en el calendario de planificación y en el informe de Reservas, filtradas por canal.

---

## Seguridad

El motor incluye protección anti-bots con reCAPTCHA en el momento de crear la reserva. Esto evita reservas fraudulentas o automáticas.

---

## Permisos necesarios

| Permiso | Qué permite |
|---------|-------------|
| **Motor de reservas (menú)** | Ver el motor de reservas en el menú |
| **Configuración del motor** | Modificar colores, GTM y opciones |
