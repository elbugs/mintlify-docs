# 03 - Planificación y Calendario

**URLs:**
- Calendario de reservas: [https://app.hotelgest.com/planning/bookings](https://app.hotelgest.com/planning/bookings)
- Vista de disponibilidad: [https://app.hotelgest.com/planning/availability](https://app.hotelgest.com/planning/availability)

El módulo de Planificación es el corazón operativo de Hotelgest Unified. Ofrece dos vistas principales: **Calendario de Reservas** y **Disponibilidad**.

---

## Calendario de Reservas

Vista de planificador con habitaciones en el eje vertical y fechas en el eje horizontal. Cada reserva aparece como una barra horizontal en la habitación correspondiente.

### Información de cada reserva
- **Logo de la OTA** de origen (Booking.com, Expedia, etc.)
- **Nombre** del huésped o del titular
- Iconos de **ocupación**: adultos, niños, bebés
- **Precio** de la reserva (opcional)
- Borde indicando el **estado de pago**
- **Tooltip** al pasar el ratón: OTA, localizador, huésped, teléfono, ocupación, empresa, régimen, fechas, noches, total, notas

### Modos de visualización
- **Modo noche**: Sin rejilla horaria, centrado en noches
- **Vista compacta**: Altura reducida de filas para ver más habitaciones
- **Niveles de zoom**: 5 niveles (del 1 al 5) para ajustar el ancho de las celdas
- **Colores dinámicos**: Colorear reservas por OTA de origen o por colores personalizados

### Opciones de visualización
- Mostrar/ocultar **ocupación** (adultos/niños/bebés) en las barras
- Mostrar/ocultar **precio** en las barras
- Mostrar **nombre** o **ID** de la reserva
- Mostrar **barras de disponibilidad** por tipo de habitación (porcentaje disponible/ocupado)

### Acciones sobre reservas
- **Hacer clic** en una reserva: Abre el detalle en una pestaña superior sin salir del calendario
- **Arrastrar y soltar (Drag & Drop)**: Mover una reserva a otra habitación (con validaciones y confirmación)
- **Redimensionar**: Cambiar las fechas arrastrando los extremos de la barra
- **Selección rectangular**: Seleccionar un rango de fechas y habitaciones para crear una nueva reserva
- **Intercambiar (Swap)**: Intercambiar las habitaciones de dos reservas

### Reservas agrupadas
- Las reservas que pertenecen a un grupo muestran enlaces visuales entre sí
- Acciones de grupo: editar, mover y gestionar todas las reservas del grupo

### Bloqueos
- Los bloqueos de habitaciones aparecen con un icono de candado
- Se pueden crear, visualizar y editar bloqueos (por mantenimiento, fuera de servicio, etc.)

### Restricciones
- Haz clic en las cabeceras de fecha para ver los días cerrados y las estancias mínimas/máximas
- Los fines de semana se muestran resaltados

### Playground
Área opcional separada para reservas sin habitación asignada (útil para gestionar overbooking).

### Navegación
- Botones **adelante/atrás** para navanzar o retroceder en el tiempo
- Botón **"Hoy"** para volver a la fecha actual
- **Selector de fecha** para saltar a una fecha específica
- **Pestañas superiores** para tener varios detalles de reserva abiertos simultáneamente

### Filtros
- **Búsqueda**: Por nombre del huésped o ID de reserva
- **Nombre de habitación**
- **Tipo de habitación**
- **OTA de origen**

### Atajos de teclado
- **Flechas**: Navegar por el calendario
- **P**: Crear nueva reserva
- **Esc**: Limpiar selección

---

## Vista de Disponibilidad

Vista centrada en la capacidad por tipo de habitación en lugar de reservas individuales.

### Contenido
- **Filas**: Tipos de habitación
- **Columnas**: Fechas
- **Celdas**: Unidades disponibles vs. total (o porcentaje de ocupación)

### Estados visuales
- **Overbooking**: Más reservas que habitaciones disponibles
- **Completo**: Todas las unidades ocupadas
- **Parcialmente ocupado**: Algunas unidades disponibles
- **Libre**: Todas las unidades disponibles

### Indicadores
- Iconos de estado: bloqueado, tentativo, confirmado
- **Fila de resumen**: Disponibilidad agregada en la parte superior

### Filtros
- Mostrar/ocultar: overbooking, completo, libre, parcial
- Alternar entre: porcentaje o cantidad
- Vista compacta

### Navegación
Mismas herramientas que el calendario de reservas: adelante/atrás, "Hoy", selector de fecha, búsqueda.
