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
