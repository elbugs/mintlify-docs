# Componentes de Mintlify usados en esta documentación

Esta documentación utiliza los componentes MDX de [Mintlify](https://www.mintlify.com/docs/components) para mejorar la lectura y la navegación. Los archivos `.mdx` pueden usar estos componentes; los `.md` se mantienen para Intercom y otros usos.

## Resumen por documento

| Documento | Componentes usados |
|-----------|--------------------|
| **README.mdx** | Card, Columns, Column, Tiles, Tile, Tabs, TabItem, Callout |
| **01-inicio-y-autenticacion.mdx** | Card, AccordionGroup, Accordion, Callout (info, tip, warning, check, danger), Steps, Step, Tabs, TabItem, Tooltip |
| **02-dashboard.mdx** | Card, Tabs, TabItem, Badge, Columns, Column, Tiles, Tile, Callout |
| **04-reservas.mdx** | Card, Mermaid (flowchart), Steps, Step, Tabs, TabItem, AccordionGroup, Accordion, Columns, Column, Callout |

## Referencia rápida de componentes

### Estructura y navegación
- **Card** – Enlaces destacados con icono y CTA: `title`, `icon`, `href`, `ctaText`, `horizontal`
- **Tiles / Tile** – Grid de enlaces: `title`, `description`, `href`
- **Columns / Column** – Contenido en columnas: `<Columns size="2"><Column>...</Column></Columns>`
- **Tabs / TabItem** – Pestañas: `<Tabs><TabItem value="x" label="Etiqueta">contenido</TabItem></Tabs>`
- **Steps / Step** – Pasos numerados: `<Steps><Step title="...">contenido</Step></Steps>`

### Énfasis y avisos
- **Callout** – Notas, avisos, tips: `type="note"|"info"|"tip"|"warning"|"danger"|"check"`, `title="..."`
- **Badge** – Etiquetas: `<Badge color="green">texto</Badge>` (gray, blue, green, yellow, red, etc.)
- **Tooltip** – Texto al pasar el ratón: `<Tooltip content="...">texto</Tooltip>`
- **Banner** – Configurado en `docs.json` (anuncios globales)

### Contenido expandible
- **AccordionGroup / Accordion** – Acordeones: `title`, `icon`, `defaultOpen`, contenido como hijos
- **Expandable** – Contenido colapsable (útil para API): `title`, `<ExpandableItem>`

### Código y diagramas
- **CodeGroup** – Varios bloques de código en pestañas: `<CodeGroup>` con bloques ``` dentro
- **Mermaid** – Diagramas: bloque ` ```mermaid ` con sintaxis Mermaid (flowchart, sequence, etc.)

### Otros (disponibles para usar)
- **Update** – Changelog / novedades: `label`, `tag`, `description`
- **Panel** – Contenido del panel derecho de la página
- **Frame** – Marco alrededor de imágenes
- **Fields / Response** – Parámetros y respuestas de API
- **Prompt** – Prompts de IA con copia e integración Cursor
- **View** – Contenido condicional por idioma o framework
- **Color** – Muestra de color con hex
- **Icon** – Iconos Lucide (configurado en `docs.json` con `icons.library: "lucide"`)

## Configuración en docs.json

- **banner** – Mensaje global arriba del sitio (opcional, `dismissible`)
- **styling.eyebrows** – `"breadcrumbs"` para mostrar la ruta de navegación
- **icons.library** – `"lucide"` para usar nombres de iconos de [Lucide](https://lucide.dev/icons)

## Enlaces

- [Índice de documentación Mintlify](https://www.mintlify.com/docs/llms.txt)
- [Componentes (overview)](https://www.mintlify.com/docs/components)
- [Navegación](https://www.mintlify.com/docs/navigation)
