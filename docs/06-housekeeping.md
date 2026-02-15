---
title: Housekeeping
description: Rack de limpieza, estados de habitación, asignación de tareas y gestión de limpiezas en Hotelgest Unified.
---

# Housekeeping (limpieza)

El módulo de Housekeeping gestiona la limpieza de las habitaciones. Muestra qué habitaciones están sucias, cuáles necesitan limpieza hoy y permite cambiar el estado de cada habitación.

**URL:** [app.hotelgest.com/housekeeping](https://app.hotelgest.com/housekeeping)

---

## Pantalla principal

La pantalla se divide en dos partes:

- **Izquierda (Lista)**: lista de tareas de limpieza organizadas por tipo de movimiento (llegadas, salidas, etc.).
- **Derecha (Rack)**: vista de todas las habitaciones organizadas por planta y tipo, con su estado actual.

---

## Estados de las habitaciones

Cada habitación tiene un estado de limpieza que se muestra con un color en el rack:

| Estado | Color | Qué significa |
|--------|-------|---------------|
| **Sucia** | Rojo | Necesita limpieza. Se marca automáticamente al hacer check-out |
| **Limpia** | Verde | Ya ha sido limpiada por el personal |
| **Inspeccionada (Lista)** | Azul | Un supervisor ha revisado que la limpieza es correcta |
| **En revisión** | Amarillo | La limpieza está hecha pero necesita una segunda comprobación |

### Transiciones permitidas

No todos los cambios de estado son posibles. Estas son las transiciones válidas:

- **Sucia** → Limpia o Inspeccionada
- **Limpia** → Inspeccionada o En revisión
- **En revisión** → Limpia
- **Inspeccionada** → Sucia

Por ejemplo: no puedes pasar una habitación directamente de "Sucia" a "En revisión". Primero tiene que pasar por "Limpia".

---

## Lista de tareas (columna izquierda)

La lista muestra las habitaciones que necesitan atención, organizadas en dos pestañas:

### Pestaña "Hoy"
Habitaciones que necesitan limpieza hoy.

### Pestaña "Mañana"
Habitaciones que necesitarán limpieza mañana.

### Grupos de tareas

Las tareas se agrupan según el tipo de movimiento de la reserva:

| Grupo | Qué significa |
|-------|---------------|
| **Llegadas** (Check-in) | Habitaciones donde llega un huésped hoy |
| **Salidas con entrada** (Check-out / Check-in) | Habitaciones donde sale un huésped y entra otro el mismo día. Prioridad alta |
| **Salidas** (Check-out) | Habitaciones donde sale un huésped hoy |
| **Repaso** (Stayover) | Habitaciones donde el huésped sigue alojado y toca limpieza periódica |
| **Pendientes** | Habitaciones con limpieza pendiente de días anteriores |

Cada tarea muestra:
- Información de la reserva (nombre, fechas)
- Tareas pendientes (ToDos de llegada y salida)
- Notas internas
- Ocupación (adultos, niños)

---

## Rack de habitaciones (columna derecha)

El rack muestra todas las habitaciones de la propiedad organizadas por planta y tipo de habitación. Cada tarjeta incluye:

- Número de puerta
- Ocupación actual (si hay reserva)
- Fecha de próxima limpieza
- Color según el estado de limpieza

### Filtros del rack

Puedes filtrar las habitaciones por:
- **Estado**: Limpia, Sucia, Inspeccionada
- **Tipo de habitación**: mostrar solo ciertos tipos
- **Planta**: filtrar por piso

### Cambiar el estado de una habitación

1. Haz clic en la tarjeta de la habitación en el rack.
2. Aparece un menú con los estados disponibles (solo las transiciones válidas).
3. Selecciona el nuevo estado.
4. El cambio se guarda automáticamente.

---

## Gestionar la limpieza de una reserva

Desde el detalle de una reserva o desde la lista de housekeeping, puedes abrir el modal de gestión de limpieza.

### Periodicidad de limpieza

Puedes configurar con qué frecuencia se limpia la habitación durante la estancia del huésped:

- **Por número de noches**: limpieza cada X noches (ejemplo: cada 3 noches).
- **Por días de la semana**: limpieza en días concretos (ejemplo: lunes, miércoles y viernes).

### Cambiar la fecha de próxima limpieza

Puedes cambiar manualmente la fecha de la próxima limpieza desde el calendario del modal.

### Acciones adicionales

Desde el modal también puedes:
- Reportar una avería en la habitación.
- Registrar objetos perdidos.
- Ver el historial de limpiezas.

---

## Automatismos

### Al hacer check-out

Cuando se hace check-out de una reserva, la habitación se marca como **Sucia** automáticamente. No necesitas hacer nada; el sistema lo gestiona solo.

Si la reserva tiene configurado un estado de destino diferente (`roomStatusDestination`), se aplica ese estado en su lugar.

### Limpieza automática por periodicidad

El sistema tiene un proceso automático (cron) que revisa cada día las habitaciones y cambia el estado de limpieza según la periodicidad configurada en cada reserva. Por ejemplo, si una reserva tiene limpieza cada 3 noches, al tercer día la habitación pasa a "Sucia" automáticamente.

---

## Configuración

### Activar o desactivar housekeeping

Desde **Configuración**, se puede ajustar el número de días de limpieza por defecto (`cleanRoomDays`). Si se pone a 0, el módulo se desactiva y no se generan tareas de limpieza automáticas.

---

## Permisos necesarios

| Permiso | Qué permite |
|---------|-------------|
| **Ver datos de housekeeping** | Acceder al rack y la lista de tareas |
| **Gestionar limpieza** | Cambiar estados, modificar periodicidad y fechas |

**Roles con acceso por defecto:** Admin, Recepción, Dirección, Limpieza (Cleaner).

Los roles de Informes, VRO y DPO no tienen acceso a housekeeping por defecto.
