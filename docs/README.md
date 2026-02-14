# Documentación de Usuario - Hotelgest Unified (PMS)

**URL de acceso:** [https://app.hotelgest.com](https://app.hotelgest.com)

### Accesos directos

| Sección | URL |
|---------|-----|
| Login | https://app.hotelgest.com/login |
| Dashboard | https://app.hotelgest.com/dashboard |
| Planificación (reservas) | https://app.hotelgest.com/planning/bookings |
| Planificación (disponibilidad) | https://app.hotelgest.com/planning/availability |
| Housekeeping | https://app.hotelgest.com/housekeeping |
| Mensajes | https://app.hotelgest.com/messages |
| Actividad | https://app.hotelgest.com/activity |
| Notificaciones | https://app.hotelgest.com/notifications |
| Motor de reservas | https://app.hotelgest.com/booking-engine |
| Recepción automática | https://app.hotelgest.com/automatic-reception |
| Configuración | https://app.hotelgest.com/settings |
| Informes | https://app.hotelgest.com/report/bookings (y resto bajo `/report/...`) |
| Marketplace | https://app.hotelgest.com/marketplace |
| Academia | https://app.hotelgest.com/academy |
| Roadmap | https://app.hotelgest.com/roadmap |

**Hotelgest Unified** es un sistema de gestión hotelera (PMS - Property Management System) diseñado para hoteles, apartamentos turísticos y alojamientos. Permite gestionar reservas, facturación, housekeeping, comunicaciones, informes y mucho más desde una única plataforma web y móvil.

---

## Índice General

| # | Sección | Descripción |
|---|---------|-------------|
| 01 | [Inicio y Autenticación](01-inicio-y-autenticacion.md) | Login, 2FA, recuperación de contraseña, sesiones |
| 02 | [Panel de Control (Dashboard)](02-dashboard.md) | Widgets, métricas, tareas y vista general del día |
| 03 | [Planificación y Calendario](03-planificacion.md) | Calendario visual, drag & drop, disponibilidad |
| 04 | [Gestión de Reservas](04-reservas.md) | Crear, editar, check-in/out, estados, clientes |
| 05 | [Facturación y Pagos](05-facturacion-y-pagos.md) | Facturas, proformas, pagos, depósitos |
| 06 | [Housekeeping (Limpieza)](06-housekeeping.md) | Rack de limpieza, estados de habitación, tareas |
| 07 | [Informes y Reportes](07-informes.md) | Todos los informes disponibles y sus filtros |
| 08 | [Motor de Reservas](08-motor-de-reservas.md) | Reservas directas, políticas, códigos promocionales |
| 09 | [Comunicaciones](09-comunicaciones.md) | WhatsApp, email, notificaciones push |
| 10 | [Recepción Automática](10-recepcion-automatica.md) | Self check-in, web app para huéspedes |
| 11 | [Configuración y Ajustes](11-configuracion.md) | Perfil, usuarios, roles, impuestos, habitaciones |
| 12 | [Integraciones](12-integraciones.md) | Autoridades, firma digital, channel manager, cerraduras |
| 13 | [Gestión Multi-Propiedad](13-multipropiedad.md) | Múltiples propiedades, selector, permisos |
| 14 | [Actividad e Historial](14-actividad-e-historial.md) | Registro de actividad, auditoría de cambios |
| 15 | [Academia y Ayuda](15-academia-y-ayuda.md) | Recursos formativos, soporte, roadmap |
| 16 | [Aplicación Móvil](16-aplicacion-movil.md) | Navegación móvil, funciones exclusivas |
| 17 | [Administración (Super Admin)](17-administracion-super-admin.md) | Planes, pre-cuentas, mapa, IA de voz |

---

## Requisitos del Sistema

### Navegadores compatibles (Web)
- Google Chrome (recomendado)
- Mozilla Firefox
- Safari
- Microsoft Edge

### Aplicación Móvil
- iOS (iPhone y iPad)
- Android

### Idiomas disponibles
- Español
- Catalán
- Euskera
- Gallego
- Inglés
- Francés
- Alemán
- Italiano
- Portugués

---

## Acceso al Sistema

Para acceder a Hotelgest Unified necesitas:
1. Un **nombre de usuario** proporcionado por tu administrador
2. Una **contraseña** segura
3. Opcionalmente, una aplicación de **autenticación 2FA** (Google Authenticator o similar)

Consulta la sección [Inicio y Autenticación](01-inicio-y-autenticacion.md) para más detalles.

---

## Formatos de archivo en /docs

| Formato | ¿Hace falta? | Uso |
|--------|----------------|-----|
| **.md** | **Sí** (uno por artículo) | Base de cada artículo. Mintlify lo usa como página si no hay .mdx. |
| **.mdx** | Opcional | Mintlify: componentes (Card, Steps, Tabs, etc.). Si existe .mdx, Mintlify usa ese; si no, el .md. |

**Resumen:** Mantén el **.md** de cada artículo. Añade **.mdx** donde quieras componentes. La publicación es con Mintlify; ver [MINTLIFY-CONEXION.md](MINTLIFY-CONEXION.md).

---

## Publicación (Mintlify)

La documentación se publica en **Mintlify**. Ver [MINTLIFY-CONEXION.md](MINTLIFY-CONEXION.md) para conectar el repo de GitHub y sincronizar desde Bitbucket.

