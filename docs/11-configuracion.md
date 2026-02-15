---
title: Configuración y ajustes
description: Usuarios, roles, permisos, propiedad, habitaciones, impuestos, facturación y todos los ajustes de Hotelgest Unified.
---

# Configuración y ajustes

Desde Configuración puedes gestionar usuarios, roles, propiedad, habitaciones, tarifas, impuestos, facturación, integraciones y más. Solo los administradores tienen acceso completo a esta sección.

**URL:** [app.hotelgest.com/settings](https://app.hotelgest.com/settings)

---

## Secciones de configuración

| Sección | URL | Qué configura |
|---------|-----|---------------|
| Perfil | `/settings/profile` | Tu cuenta personal, contraseña, 2FA |
| Usuarios | `/settings/users` | Crear, editar y gestionar usuarios |
| Roles | `/settings/roles` | Roles y permisos personalizados |
| Suscripción | `/settings/subscription` | Plan actual y facturación del servicio |
| API Keys | `/settings/apikeys` | Claves de API para integraciones |
| Webhooks | `/settings/webhooks` | Webhooks para enviar datos a otros sistemas |
| Comunicación | `/settings/communication` | Plantillas de WhatsApp y ajustes de email |
| Auto-asignación de tareas | `/settings/auto-assign-todos` | Reglas automáticas para asignar tareas |
| Políticas de cancelación | `/settings/policies` | Políticas estándar y personalizadas |
| Alojamiento | `/settings/account` | Datos de la propiedad (nombre, dirección, logo) |
| Impuestos y tasas | `/settings/taxes` | Impuestos, tasa turística, recargo municipal |
| Facturación y contabilidad | `/settings/accounting` | Datos fiscales, numeración de facturas |
| Habitaciones | `/settings/rooms` | Tipos de habitación y habitaciones físicas |
| LOPD / RGPD | `/settings/data-privacy` | Protección de datos y períodos de conservación |
| Reservas | `/settings/bookings` | Campos obligatorios, colores, horarios |
| Recepción autónoma | `/settings/autonomous-reception` | Check-in online y web app |
| Channel Manager | `/settings/channel` | Configuración de canales de distribución |

---

## Gestión de usuarios

**URL:** [settings/users](https://app.hotelgest.com/settings/users)

### Crear un usuario

1. Haz clic en **Añadir usuario**.
2. Rellena los campos:
   - **Nombre de usuario** (único, sin espacios, en minúsculas)
   - **Contraseña**
   - **Nombre y apellidos**
   - **Email** (opcional)
   - **Rol** (selecciona uno de los roles disponibles)
3. Guarda.

### Acciones sobre un usuario

| Acción | Qué hace |
|--------|----------|
| Editar | Cambiar nombre, email, contraseña, rol |
| Bloquear | Impide que el usuario acceda al sistema |
| Desbloquear | Devuelve el acceso |
| Deshabilitar 2FA | Desactiva la autenticación en dos pasos del usuario |
| Reenviar email de verificación | Envía otro email para verificar la cuenta |
| Compartir entre propiedades | Permite que el usuario acceda a otras propiedades |
| Eliminar | Desactiva el usuario (se puede restaurar) |
| Restaurar | Reactiva un usuario eliminado |

---

## Gestión de roles y permisos

**URL:** [settings/roles](https://app.hotelgest.com/settings/roles)

### Roles predefinidos

| Rol | Descripción |
|-----|-------------|
| **Admin** | Acceso completo a todo |
| **Dirección** | Acceso amplio, similar a Admin |
| **Recepción** | Gestión de reservas, check-in/out, facturación |
| **Limpieza (Cleaner)** | Solo housekeeping |
| **Informes (Reports)** | Solo informes y reportes |
| **DPO** | Delegado de Protección de Datos |
| **VRO** | Rol VRO |

### Crear un rol personalizado

Solo disponible en el plan Unified.

1. Ve a **Configuración > Roles**.
2. Haz clic en **Crear rol**.
3. Escribe un nombre.
4. Selecciona los permisos que quieras asignar (mínimo 1).
5. Guarda.

### Módulos de permisos

Los permisos se organizan por módulos:

**Dashboard:** ver widgets, autoPricing, lista de reservas, orígenes, ocupación, housekeeping, ingresos, estado, tareas.

**Calendario:** añadir bloqueos, eliminar bloqueos.

**Reservas:** crear, editar, mover, check-in, check-out, ver precios, ver nombres, gestionar artículos, facturas, proformas, pagos, enviar email, enviar WhatsApp, abrir web app, escanear documentos, gestionar notas, gestionar tareas, gestionar limpieza, agrupar reservas, ver autoridades.

**Housekeeping:** ver datos.

**Configuración:** cuenta, comunicación, channel manager, planning, motor de reservas, facturación, contabilidad, pagos, notificaciones, logs, gestores, recepción autónoma, marketplace, teléfono, programa de referidos, LOPD, API, propietarios, chat, portabilidad.

**Menú:** controla qué secciones del menú lateral puede ver el usuario (dashboard, planning, tarifas, cada informe, motor de reservas, bandeja, mensajes, marketing, configuración, actividad, housekeeping, facturación).

---

## Configuración de la propiedad

**URL:** [settings/account](https://app.hotelgest.com/settings/account)

### Datos básicos
- Nombre de la propiedad
- Teléfono, email, web
- Tipo de propiedad
- Moneda (EUR, USD, GBP, etc.)
- Zona horaria

### Ubicación
- País, provincia, ciudad
- Dirección, número, código postal
- Coordenadas (latitud, longitud)
- Al guardar la ubicación, se genera automáticamente el widget del tiempo.

### Contenido
- Descripción (multilingüe)
- Información adicional (multilingüe): horarios, condiciones, indicaciones.
- Nota legal (multilingüe)
- Aviso de tasa turística (multilingüe)

### Logo
- Imagen del logo (máx. 1 MB, 220x220 px)
- Opción de usar el logo en los emails enviados

### Galería de imágenes
- Subir imágenes de la propiedad (máx. 2 MB, 1500x1500 px por imagen)
- Reordenar arrastrando
- Eliminar imágenes

---

## Tipos de habitación y habitaciones

**URL:** [settings/rooms](https://app.hotelgest.com/settings/rooms)

### Tipo de habitación (tipología)
Cada tipo agrupa habitaciones con las mismas características:
- Nombre y descripción (multilingüe)
- Camas, baños, tamaño (m²)
- Ocupación máxima
- Servicios incluidos
- Fotografías (con reordenación)
- Código INE (para el Instituto Nacional de Estadística)
- Coste extra de limpieza
- Visible en inventario y motor de reservas

### Habitación física
Cada habitación pertenece a un tipo:
- Número de puerta
- Piso
- Orden de visualización

---

## Impuestos y tasas

**URL:** [settings/taxes](https://app.hotelgest.com/settings/taxes)

| Campo | Descripción |
|-------|-------------|
| Impuesto local | Porcentaje del impuesto principal |
| Impuestos adicionales | Porcentaje adicional |
| Tasa turística | Número de noches, precio por adulto y por niño (impuestos excluidos) |
| Recargo municipal | Número de noches, precio por adulto y por niño |
| Programar temporadas | Tarifas específicas para períodos concretos |

---

## Configuración de reservas

**URL:** [settings/bookings](https://app.hotelgest.com/settings/bookings)

### Horarios
- Hora máxima de check-in (motor de reservas)
- Hora máxima de check-in (recepción)
- Hora máxima de check-out

### Asignación y presentación
- Asignar reservas al playground por defecto
- Ocultar tipos de habitación en planning
- Ordenar habitaciones por nombre
- Requerir pago para hacer check-out
- Colores personalizados para reservas (definir colores con nombre)

### Campos obligatorios al crear reserva
Puedes marcar como obligatorios: nombre, apellidos, teléfono, dirección, ciudad, código postal, hora de llegada, email, documento de identidad, segmento.

### Otras opciones
- Número de decimales en precios
- Notas compartidas en grupos de reservas
- Notas compartidas en reservas canceladas
- Días de limpieza por defecto
- No reemplazar titular al escanear documento
- Considerar comida como media pensión por defecto

---

## Facturación y contabilidad

**URL:** [settings/accounting](https://app.hotelgest.com/settings/accounting)

- Datos fiscales: nombre legal, NIF, dirección fiscal
- Prefijos y numeración de facturas, proformas y notas de crédito
- Preferencias de facturación
- Campos obligatorios al generar facturas
- Avisos legales y pie de factura

---

## Políticas de cancelación

**URL:** [settings/policies](https://app.hotelgest.com/settings/policies)

Tres tipos:
- **Políticas estándar**: se aplican a todas las reservas.
- **Plantillas de políticas**: textos reutilizables.
- **Políticas personalizadas**: se aplican a tipos de habitación o períodos concretos.

Cada política tiene una descripción multilingüe.

---

## Protección de datos (LOPD / RGPD)

**URL:** [settings/data-privacy](https://app.hotelgest.com/settings/data-privacy)

Configura los períodos de conservación de datos:

| Tipo de dato | Opciones |
|-------------|----------|
| Datos identificativos | No eliminar, 1-10 años |
| Documentos de identidad | No eliminar, 1-10 años |
| Imágenes | No eliminar, 1-10 años |
| Datos biométricos | No eliminar, 1-10 años |
| Datos de facturación | No eliminar, 1-10 años |
| Notas internas | No eliminar, 1-10 años |

Incluye también la configuración de la nota legal.

---

## API Keys

**URL:** [settings/apikeys](https://app.hotelgest.com/settings/apikeys)

Crea claves de API para que otros sistemas se conecten a Hotelgest:
- Crear API key con descripción.
- Ver la lista de claves activas.
- Eliminar claves.
- Acceder a la documentación de la API.

---

## Webhooks

**URL:** [settings/webhooks](https://app.hotelgest.com/settings/webhooks)

Configura webhooks para que Hotelgest envíe datos automáticamente a otros sistemas:
- URL de destino.
- Eventos que disparan el envío.
- Autenticación básica (opcional).
- Ver logs de envíos.
- Probar un webhook.
