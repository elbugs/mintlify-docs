---
title: Administración (Super Admin)
description: Panel de Super Administrador de Hotelgest Unified con gestión de planes, propiedades, usuarios globales, IA de voz y consentimientos.
---

# Administración (Super Admin)

El panel de Super Admin es exclusivo para el equipo de Hotelgest. Desde aquí se gestionan los planes de suscripción, las cuentas de nuevas propiedades, el mapa de alojamientos, la IA de voz y los consentimientos de datos. Los usuarios normales no ven esta sección.

---

## Acceso

Solo los usuarios marcados como Super Admin pueden acceder. El Super Admin tiene acceso completo a todas las propiedades del sistema sin restricciones de permisos.

**Autenticación especial:**
- Login: `/api/super-admin/auth/login`
- Verificación: `/api/super-admin/auth/verify-login`
- Login como otro usuario: permite entrar como si fueras otro usuario para depurar problemas.
- Gestión de sesiones: ver y cerrar sesiones de cualquier usuario.

---

## Secciones

### 1. Planes

**URL:** [app.hotelgest.com/manage/plans](https://app.hotelgest.com/manage/plans)

Gestión de los planes de suscripción disponibles en Hotelgest.

**Qué se puede hacer:**
- Ver todos los planes con sus características y precios.
- Configurar qué módulos incluye cada plan.
- Definir límites de uso (número de habitaciones, usuarios, etc.).
- Asignar planes a propiedades.
- Gestionar upgrades y downgrades.

---

### 2. Pre-cuentas

**URL:** [app.hotelgest.com/manage/pre-account](https://app.hotelgest.com/manage/pre-account)

Gestión de nuevas cuentas en proceso de creación.

**Qué se puede hacer:**
- Ver todas las solicitudes de nuevas cuentas.
- Seguir el estado del onboarding (solicitud recibida → en revisión → datos completados → cuenta activada).
- Crear pre-cuentas manualmente.
- Aprobar o rechazar solicitudes.

---

### 3. Mapa

**URL:** [app.hotelgest.com/manage/map](https://app.hotelgest.com/manage/map)

Vista geográfica de todas las propiedades del sistema.

**Qué se puede hacer:**
- Ver la ubicación de todas las propiedades en un mapa.
- Hacer clic en un marcador para ver información básica (nombre, logo, tipo).
- Supervisar la distribución geográfica de la red de alojamientos.

---

### 4. IA de voz (AI Voice)

**URL:** [app.hotelgest.com/manage/ai-voice](https://app.hotelgest.com/manage/ai-voice)

Gestión del asistente de voz con inteligencia artificial para recepción telefónica.

**Qué se puede hacer:**
- Configurar el asistente de voz (basado en Retell AI).
- Definir qué puede hacer el asistente:
  - Atender llamadas telefónicas automáticamente.
  - Responder preguntas frecuentes de los huéspedes.
  - Transferir llamadas complejas a recepción.
  - Registrar resúmenes de las conversaciones.
- Probar conversaciones con el asistente.
- Activar o desactivar por propiedad.

---

### 5. Consentimientos

**URL:** [app.hotelgest.com/manage/consents](https://app.hotelgest.com/manage/consents)

Gestión centralizada de los consentimientos de tratamiento de datos (RGPD).

**Qué se puede hacer:**
- Crear nuevos documentos de consentimiento (título y contenido).
- Editar borradores (los consentimientos publicados no se pueden editar).
- Publicar un consentimiento para que sea visible a los usuarios.
- Eliminar borradores.
- Ver qué usuarios han aceptado el consentimiento publicado.

**Reglas:**
- Un consentimiento publicado no se puede modificar ni eliminar.
- Solo puede haber un consentimiento publicado activo a la vez.
- Al publicar uno nuevo, sustituye al anterior.
- Los usuarios ven una pantalla de aceptación al iniciar sesión si hay un nuevo consentimiento.

---

## Gestión global de usuarios

El Super Admin puede gestionar usuarios de cualquier propiedad:

| Acción | Qué hace |
|--------|----------|
| Crear usuario | Crear un usuario en cualquier propiedad |
| Cambiar rol | Cambiar el rol de cualquier usuario |
| Bloquear / Desbloquear | Impedir o restaurar el acceso |
| Eliminar permanentemente | Borrar todos los datos del usuario (irreversible) |
| Restaurar | Recuperar un usuario eliminado |
| Añadir tester | Marcar un usuario como tester (acceso a funcionalidades beta) |
| Eliminar tester | Quitar el estado de tester |

---

## Gestión global de API Keys

El Super Admin puede ver y gestionar las API Keys de todas las propiedades:

- Ver todas las API Keys del sistema.
- Crear API Keys para cualquier propiedad.
- Habilitar o deshabilitar API Keys.
- Revocar API Keys.

---

## Configuración del sistema

| Acción | Qué hace |
|--------|----------|
| Nueva versión | Registrar una nueva versión de la aplicación |
| Mantenimiento | Poner la aplicación en modo mantenimiento |
| Producción | Enviar una versión a producción |
| Limpiar caché | Limpiar la caché del sistema |
| Contacto de soporte | Actualizar los datos de contacto del soporte |
| Configuración admin | Ver y modificar la configuración general |
