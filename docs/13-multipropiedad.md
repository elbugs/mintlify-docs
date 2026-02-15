---
title: Gestión multipropiedad
description: Gestionar múltiples propiedades, cambiar de propiedad y permisos por propiedad en Hotelgest Unified.
---

# Gestión multipropiedad

Si gestionas más de un alojamiento (hotel, apartamentos, etc.), Hotelgest te permite acceder a todos desde la misma cuenta. Cada propiedad tiene su propia configuración, habitaciones, reservas e integraciones, pero los usuarios pueden ser compartidos.

---

## Cómo cambiar de propiedad

1. En el menú lateral, mira la parte superior: verás el nombre de la propiedad activa.
2. Haz clic en el nombre de la propiedad.
3. Se abre un desplegable con todas las propiedades a las que tienes acceso.
4. Selecciona la propiedad a la que quieras cambiar.
5. La interfaz se actualiza automáticamente con los datos de la nueva propiedad: reservas, habitaciones, informes, configuración, etc.

En móvil, el selector está disponible en el menú lateral.

---

## Qué es compartido y qué es independiente

### Compartido entre propiedades

| Elemento | Detalle |
|----------|---------|
| **Usuarios** | Un mismo usuario puede tener acceso a varias propiedades con roles diferentes en cada una |
| **Base de datos de clientes** | Los datos de los huéspedes se pueden compartir entre propiedades |
| **Notas compartidas** | Si está activado, las notas de reserva son visibles entre propiedades |

### Independiente por propiedad

| Elemento | Detalle |
|----------|---------|
| **Habitaciones y tipos** | Cada propiedad tiene sus propios tipos de habitación y habitaciones |
| **Tarifas y precios** | Cada propiedad define sus propias tarifas |
| **Impuestos** | Útil si las propiedades están en regiones con impuestos diferentes |
| **Facturación** | Numeración, prefijos y datos fiscales independientes |
| **Motor de reservas** | Cada propiedad tiene su propia URL y personalización |
| **Integraciones** | Cada propiedad puede tener diferentes integraciones activas |
| **Channel Manager** | Canales de distribución independientes |
| **Autoridades** | Configuración según la comunidad autónoma de la propiedad |
| **Moneda** | Cada propiedad puede usar EUR, USD, GBP, etc. |
| **Zona horaria** | Cada propiedad puede estar en una zona horaria diferente |
| **Logo y descripción** | Branding independiente |

---

## Permisos por propiedad

Un usuario puede tener roles diferentes en cada propiedad. Por ejemplo:
- **Admin** en el Hotel Principal.
- **Recepción** en los Apartamentos.
- Sin acceso a otras propiedades.

Al cambiar de propiedad, el menú y las opciones disponibles se ajustan automáticamente según el rol del usuario en esa propiedad.

### Compartir un usuario entre propiedades

1. Ve a **Configuración > Usuarios**.
2. Selecciona el usuario.
3. Haz clic en **Compartir entre propiedades**.
4. Selecciona las propiedades a las que quieras darle acceso.
5. Asigna un rol para cada propiedad.
6. Guarda.

### Compartir un rol entre propiedades

Si has creado un rol personalizado, puedes compartirlo con otras propiedades para no tener que crearlo de nuevo (requiere plan Unified).

---

## Informes multi-propiedad

Algunos informes permiten seleccionar varias propiedades a la vez para ver datos consolidados. Los totales se muestran desglosados por propiedad.

---

## Identificación de propiedades

Cada propiedad tiene un código único llamado **pcode** (property code). Este código se usa internamente en todas las operaciones y es visible en la URL cuando navegas por la aplicación.
