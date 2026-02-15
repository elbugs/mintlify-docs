# Gestión multipropiedad

**URL:** El selector de propiedades está en la cabecera del menú lateral una vez dentro de la aplicación ([https://app.hotelgest.com/dashboard](https://app.hotelgest.com/dashboard)).

Hotelgest Unified permite gestionar múltiples propiedades (hoteles, apartamentos, hostales, etc.) desde una única cuenta de usuario.

---

## Descripción General

Cada propiedad se identifica con un **código de propiedad (pcode)** único. Un usuario puede tener acceso a una o varias propiedades, cada una con su propia configuración, habitaciones, reservas e informes.

---

## Selector de Propiedades

### En escritorio
- En la parte superior del menú lateral se muestra el **nombre de la propiedad activa**
- Haz clic en el nombre para ver la lista de propiedades disponibles
- Selecciona otra propiedad para cambiar de contexto

### En móvil
- El selector de propiedad está disponible en el menú lateral
- Al cambiar de propiedad, toda la interfaz se actualiza con los datos de la nueva propiedad

---

## Tipos de Propiedad

El sistema soporta diferentes tipos de alojamiento:
- **Hotel**: Establecimiento hotelero tradicional
- **Apartamento turístico**: Apartamentos para uso vacacional
- **Hostal**: Alojamiento más económico
- **Casa rural**: Alojamiento en entorno rural
- **Camping**: Área de acampada
- **Otros**: Cualquier tipo de alojamiento configurable

El tipo de propiedad se configura en **Configuración > Cuenta**.

---

## Permisos por Propiedad

### Roles y acceso
- Cada usuario tiene un **rol asignado por propiedad**
- Un mismo usuario puede tener roles diferentes en distintas propiedades
- Los permisos se evalúan en función de la propiedad activa

### Ejemplo
| Usuario | Propiedad A | Propiedad B |
|---------|-------------|-------------|
| María | Administradora | Recepcionista |
| Juan | Recepcionista | Sin acceso |
| Ana | Administradora | Administradora |

---

## Configuración Independiente

Cada propiedad tiene su propia configuración independiente:
- **Habitaciones y tipologías**: Distintas para cada propiedad
- **Tarifas**: Precios y restricciones propias
- **Impuestos**: Configuración fiscal específica (útil si las propiedades están en distintas regiones)
- **Facturación**: Numeración, prefijos y datos fiscales propios
- **Motor de reservas**: Configuración independiente por propiedad
- **Integraciones**: Cada propiedad puede tener sus propias integraciones activas
- **Channel Manager**: Canales de distribución específicos
- **Autoridades**: Configuración según la comunidad autónoma correspondiente

---

## Monedas

Cada propiedad puede operar en su propia moneda:
- **EUR** (Euro)
- **USD** (Dólar estadounidense)
- **GBP** (Libra esterlina)
- Y otras monedas configurables

La moneda se configura en **Configuración > Cuenta** y afecta a todos los precios, facturas e informes de esa propiedad.

---

## Zonas Horarias

Cada propiedad puede tener su propia zona horaria, lo cual es especialmente útil para cadenas con propiedades en distintos países. La zona horaria afecta a:
- Horas de check-in y check-out
- Programación de tareas automáticas
- Envío de notificaciones
- Generación de informes

---

## Datos Compartidos entre Propiedades

Algunos datos pueden compartirse entre propiedades:
- **Usuarios**: Un mismo usuario puede acceder a múltiples propiedades
- **Notas compartidas**: Si está activado, las notas de reserva son visibles entre propiedades
- **Clientes**: La base de datos de clientes puede ser compartida

---

## Cambio Rápido de Propiedad

Al cambiar de propiedad:
1. El sistema actualiza toda la interfaz con los datos de la nueva propiedad
2. Se cargan las reservas, habitaciones e informes de la propiedad seleccionada
3. Los permisos del usuario se recalculan según su rol en la nueva propiedad
4. La configuración (moneda, zona horaria, impuestos) se ajusta automáticamente
