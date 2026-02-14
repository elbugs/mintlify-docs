# 06 - Housekeeping (Limpieza)

**URL:** [https://app.hotelgest.com/housekeeping](https://app.hotelgest.com/housekeeping)

El módulo de Housekeeping permite gestionar el estado de limpieza de las habitaciones y asignar tareas al equipo de limpieza.

---

## Vista General

La pantalla de Housekeeping tiene dos columnas principales:

### Columna izquierda: Lista de tareas

Organizada por pestañas **Hoy** y **Mañana**, con las siguientes agrupaciones:

| Grupo | Descripción |
|-------|-------------|
| **Salidas con llegada** | Habitaciones donde un huésped sale y otro llega el mismo día (prioridad alta) |
| **Llegadas** | Habitaciones con check-in previsto para hoy |
| **Salidas** | Habitaciones con check-out previsto para hoy |
| **Estancias (Stayover)** | Habitaciones con huéspedes que continúan alojados |
| **Pendientes/Olvidadas** | Habitaciones que aún necesitan limpieza de días anteriores |

Cada tarjeta de tarea muestra:
- Información del huésped (nombre)
- Ocupación: adultos, niños y bebés
- Número de noches
- Estado de check-in/check-out
- Tareas pendientes asociadas (si las hay)

### Columna derecha: Rack de habitaciones

Cuadrícula visual de todas las habitaciones agrupadas por:
- **Planta**
- **Tipo de habitación**

Cada habitación muestra:
- **Número de puerta**
- **Ocupación** actual (si hay huésped alojado)
- **Próxima fecha de limpieza** (en la parte inferior de la tarjeta)
- **Color** según el estado de limpieza

---

## Estados de Habitación

| Estado | Color | Descripción |
|--------|-------|-------------|
| **Inspeccionada (Ready)** | Verde | Habitación limpia y verificada, lista para el huésped |
| **Limpia (Clean)** | Azul | Habitación limpiada, pendiente de inspección |
| **Sucia (Dirty)** | Rojo | Habitación que necesita limpieza |
| **Revisión (Revision)** | Amarillo | Habitación en proceso de revisión |

### Cambiar el estado de una habitación
1. Haz clic en una habitación en el rack
2. Se abre un menú con las opciones de estado disponibles
3. Selecciona el nuevo estado
4. El cambio se refleja inmediatamente con el nuevo color

---

## Gestión de Limpieza por Habitación

Al hacer clic en una habitación ocupada, se abre un modal de gestión con opciones:
- **Próxima fecha de limpieza**: Cuándo debe limpiarse la habitación
- **Periodicidad**: Cada cuántos días se limpia
- **Días de la semana**: En qué días se limpia (lunes, martes, etc.)

---

## Filtros

En la cabecera de la pantalla puedes filtrar las habitaciones:
- **Mostrar/Ocultar Limpias**: Incluir o excluir habitaciones limpias
- **Mostrar/Ocultar Sucias**: Incluir o excluir habitaciones sucias
- **Mostrar/Ocultar Inspeccionadas**: Incluir o excluir habitaciones inspeccionadas
- **Mostrar/Ocultar etiquetas de tipo**: Mostrar el nombre del tipo de habitación
- **Mostrar/Ocultar etiquetas de planta**: Mostrar el número de planta

---

## Búsqueda

Puedes buscar reservas directamente desde la pantalla de Housekeeping para localizar rápidamente la habitación de un huésped.

---

## Widget de Housekeeping en el Dashboard

En el Dashboard se muestra un resumen rápido del estado de limpieza con el conteo de habitaciones por estado:
- Inspeccionadas (listas)
- Limpias
- Sucias

---

## Configuración

La periodicidad de limpieza se configura desde **Configuración > Reservas**:
- **Días de limpieza**: Número de días entre limpiezas (0 = desactivado)
- Si se establece en 0, la lista de tareas de housekeeping se desactiva

Los costes de limpieza por habitación se configuran en **Configuración > Habitaciones**.
