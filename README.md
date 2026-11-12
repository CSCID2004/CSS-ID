# CSCID Design System — CSS-ID

Official visual system for Coconut Shell Charcoal Indonesia.

## Responsibility
This repository owns the presentation layer only:
- Design tokens: color, typography, spacing, radius, shadows, motion.
- Shared visual components and page templates.
- Responsive behavior and accessibility conventions.

It must not own business logic, authentication, content databases, or production website APIs. Those remain in the CSCID application repository.

## Brand direction
- Charcoal: `#24211E`
- Warm white: `#FAF8F5`
- Copper: `#C45E20`
- Stone: `#E7DFD6`
- Display font: Space Grotesk
- Body font: Inter

## Integration contract
The CSCID application consumes these styles/components. CSS-ID changes may update the visual layer, but must not alter application routes, data contracts, or business behavior.

## Files
- `styles/tokens.css`: brand design tokens.
- `styles/global.css`: base styles and reusable primitives.
- `docs/component-guidelines.md`: implementation rules.


## Centralized application stylesheets

All application-level CSS is maintained in this repository. Applications should load these shared files rather than maintaining independent copies.

- `styles/tokens.css`: shared design tokens.
- `styles/global.css`: shared reset, typography, and reusable primitives.
- `styles/site-production.css`: CSCID production site stylesheet, migrated from `CSCID2004/CSCID/src/app/globals.css`.
- `styles/edit-workspace.css`: EDIT workspace stylesheet, migrated from `CSCID2004/EDIT/app/globals.css`.

Keep application logic and content in their application repositories. When migrating an application, first verify the shared stylesheet loads correctly in preview before removing its local CSS implementation.
