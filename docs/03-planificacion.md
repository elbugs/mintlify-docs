---
title: Planificación y calendario
description: Calendario visual de reservas, disponibilidad, drag and drop y gestión de habitaciones en Hotelgest Unified.
---

# Planificación y calendario

El módulo de Planificación es el centro operativo de Hotelgest Unified. Desde aquí ves todas las reservas en un calendario visual, mueves reservas entre habitaciones, cambias fechas arrastrando y creas nuevas reservas con un clic.

**URLs:**
- Calendario de reservas: [app.hotelgest.com/planning/bookings](https://app.hotelgest.com/planning/bookings)
- Vista de disponibilidad: [app.hotelgest.com/planning/availability](https://app.hotelgest.com/planning/availability)

---

## Dos vistas disponibles

El módulo tiene dos vistas. Puedes cambiar entre ellas desde el menú lateral.

### Vista de reservas (Calendario)

Es la vista principal. Muestra un calendario con las habitaciones en el lateral izquierdo y las fechas en la parte superior. Cada reserva aparece como una barra horizontal en la fila de su habitación.

**Qué se ve en cada reserva:**
- Nombre del cliente (o número de reserva si no tienes permisos para ver nombres)
- Color del borde: indica el estado de pago
- Iconos: check-in realizado, check-out realizado, notas, empresa, bloqueo, tentativa
- Ocupación: adultos, niños, bebés (en vista expandida)
- Precio (en vista expandida, si tienes permisos)

### Vista de disponibilidad

Muestra un resumen por tipo de habitación y fecha. No se pueden mover reservas; es solo para consultar la ocupación.

**Qué se ve en cada celda:**
- Número de habitaciones disponibles / total (ejemplo: 5/10)
- Porcentaje de ocupación
- Color según ocupación:
  - **Verde**: todas las habitaciones libres
  - **Amarillo**: algunas habitaciones ocupadas
  - **Rojo**: todas las habitaciones ocupadas
  - **Negro**: overbooking (más reservas que habitaciones)

---

## Acciones con reservas (vista de reservas)

### Crear una reserva

1. Haz clic en una celda vacía del calendario (en la fila de la habitación y el día que quieras).
2. Se abre el formulario de nueva reserva con la habitación y fecha ya seleccionadas.
3. Rellena los datos del huésped y guarda.

También puedes seleccionar varias celdas arrastrando para crear una reserva de varias noches.

### Mover una reserva a otra habitación

1. Haz clic en la reserva y arrástrala a otra habitación.
2. Suéltala en la nueva habitación.
3. Se abre un diálogo de confirmación.

**Restricciones:**
- No puedes mover reservas al pasado.
- No puedes mover reservas bloqueadas.
- Si la reserva ya empezó (el huésped ya está alojado), solo puedes mover la parte futura.
- La reserva se mueve dentro de la misma propiedad.

### Cambiar las fechas de una reserva

1. Coloca el ratón en el borde izquierdo o derecho de la reserva (verás el cursor de redimensionar).
2. Arrastra el borde para alargar o acortar la estancia.
3. Se abre un diálogo de confirmación.

**Restricciones:**
- No puedes modificar reservas que ya terminaron.
- No puedes reducir la fecha de inicio a antes de hoy si el huésped ya está alojado.

### Menú de opciones de una reserva

Haz clic derecho en una reserva (o clic largo en móvil) para ver todas las acciones:

| Acción | Qué hace |
|--------|----------|
| **Abrir reserva** | Abre los detalles en una pestaña nueva |
| **Acciones rápidas** | Modal con las acciones más comunes |
| **Check-in / Check-out** | Cambia el estado de la reserva |
| **Cambiar estado** | Confirmar o poner como tentativa |
| **Cambiar de unidad** | Mover a otra habitación del mismo tipo |
| **Upgrade / Downgrade** | Cambiar a un tipo de habitación diferente |
| **Mover al playground** | Enviar a la zona de reservas sin asignar |
| **Autoasignar** | El sistema elige la mejor habitación (desde playground) |
| **Dividir** | Partir la reserva en una fecha concreta |
| **Intercambiar unidad** | Intercambiar habitación con otra reserva |
| **Clonar** | Crear una copia de la reserva |
| **Bloquear / Desbloquear** | Impedir que la reserva se pueda mover |
| **Cambiar color** | Asignar un color personalizado |
| **Copiar ID** | Copiar el número de reserva al portapapeles |

---

## El Playground

El Playground es una zona especial donde van las reservas que aún no tienen habitación asignada. Aparece en la parte inferior del calendario (o en un calendario separado si lo configuras así).

**Cómo funciona:**
- Cuando llega una reserva de una OTA (Booking.com, Airbnb...) sin habitación asignada, aparece aquí.
- Puedes arrastrar la reserva del Playground a una habitación concreta.
- También puedes usar **Autoasignar** para que el sistema elija la habitación automáticamente.
- Puedes enviar una reserva al Playground desde el menú de opciones si quieres desasignarla temporalmente.

---

## Filtros y opciones de visualización

### Filtros de búsqueda (barra superior)

- **Buscar**: por nombre del huésped, apellido o número de reserva.
- **Habitación**: filtrar por nombre de habitación o número de puerta.
- **Tipo de habitación**: mostrar solo ciertos tipos (doble, suite, etc.).
- **Canal / OTA**: mostrar solo reservas de un canal concreto (Booking.com, Expedia, directas...).

### Opciones de visualización

| Opción | Qué hace |
|--------|----------|
| **Vista compacta / expandida** | Compacta muestra menos datos; expandida muestra ocupación y precio |
| **Zoom** | 5 niveles: desde vista mensual hasta vista semanal detallada |
| **Color dinámico** | Colorea las reservas por OTA (cada canal un color) o usa colores personalizados |
| **Modo noche** | Vista simplificada con menos información |
| **Separar Playground** | Muestra el Playground en un calendario aparte |
| **Tooltip** | Muestra un resumen al pasar el ratón sobre una reserva |
| **Bloquear diagonal** | Restringe el arrastre a solo horizontal o vertical (no diagonal) |

---

## Grupos de reservas

Las reservas que pertenecen al mismo grupo (por ejemplo, un grupo de turistas con varias habitaciones) se muestran conectadas con líneas visuales. Puedes mostrar u ocultar el grupo completo desde el menú de opciones.

---

## Habitaciones divididas (splits)

Si una habitación física se puede dividir en unidades más pequeñas (por ejemplo, una suite que se divide en dos habitaciones), el calendario lo muestra de forma jerárquica: la habitación principal con sus subdivisiones debajo.

---

## Restricciones y cierres

En la cabecera de las fechas pueden aparecer iconos que indican:
- **Cierre temporal**: no se aceptan reservas para esa fecha.
- **Estancia mínima o máxima**: restricción de noches.

Haz clic en el icono para ver los detalles de la restricción.

---

## Atajos de teclado

| Atajo | Qué hace |
|-------|----------|
| `←` / `→` | Navegar a la fecha anterior / siguiente |
| `Esc` | Cancelar la selección o el intercambio en curso |
| `P` | Abrir una nueva pestaña de reserva |
| `Cmd/Ctrl + Clic` | Abrir la reserva en una nueva pestaña |

---

## Pestañas de reservas

Al abrir una reserva desde el calendario, se abre en una pestaña dentro de la misma pantalla (no sales del calendario). Puedes tener varias pestañas abiertas a la vez y cambiar entre ellas. La pestaña del calendario siempre permanece visible.

---

## Permisos necesarios

| Permiso | Qué permite |
|---------|-------------|
| Buscar reservas | Usar la barra de búsqueda |
| Crear reservas | Crear nuevas reservas desde el calendario |
| Editar y mover | Arrastrar, redimensionar, cambiar de habitación |
| Ver detalles | Abrir el detalle de una reserva |
| Ver precios | Ver el precio en la vista expandida |
| Ver nombre del cliente | Ver el nombre en lugar del número de reserva |
| Ver notas | Ver las notas internas y de solicitud |

Si no tienes un permiso concreto, esa funcionalidad no aparece o se muestra con información reducida.
