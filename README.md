# faro-demo-site

Sitio **de prueba** para FARO (Framework de Accesibilidad y Remediación Optimizada).
Contiene errores de accesibilidad **intencionales** para validar el motor de auditoría
(axe-core + Playwright) y el flujo de apertura de Issues / Pull Requests.

> ⚠️ Este repositorio **no** es un ejemplo de buenas prácticas: cada error está puesto
> a propósito y anotado con su criterio WCAG en los comentarios del HTML.

## Errores intencionales (Sprint 1)

| Criterio WCAG | Regla axe-core | Dónde |
| :-- | :-- | :-- |
| 1.1.1 | `image-alt` | Logo `<img>` sin `alt` en el header |
| 3.1.1 | `html-has-lang` | `<html>` sin atributo `lang` |
| 2.4.2 | `document-title` | Sin `<title>` en el `<head>` |
| 4.1.2 | `button-name` | Botón de ícono (SVG) sin nombre accesible |
| 2.4.1 | `bypass` | Sin skip-link ni landmarks para saltear la navegación |
| 1.3.1 | `heading-order`, `label`, `table` | Salto h1→h4, input sin label, tabla sin `th/scope` |
| 2.4.4 | `link-name` | Enlace "hacé clic acá" |
| 1.3.5 | `autocomplete-valid` | Inputs de propósito común sin `autocomplete` |
| 1.4.3 | `color-contrast` | Texto gris claro sobre blanco (~2.3:1) |
| 1.4.1 | (heurística) | Enlace distinguible solo por color |

## Uso

- Instalá la GitHub App `faro-utn` sobre este repo para probar la apertura de Issues (HU-16).
- Servido como sitio estático (ej. GitHub Pages), la URL sirve para la auditoría dinámica con Playwright.
