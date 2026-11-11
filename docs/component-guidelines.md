# Component Guidelines

## Visual principles
1. Premium industrial identity: charcoal, warm white, copper-orange.
2. Editorial typography: Space Grotesk for headings, Inter for interface/body copy.
3. Use whitespace and clear hierarchy; avoid dense dashboard-like layouts on public pages.
4. Cards use subtle borders and restrained shadows.
5. Copper is an accent for actions, active states, and key highlights—not large background fills.

## Page template anatomy
- Shared site header and footer.
- Breadcrumbs on interior pages.
- Eyebrow label, clear H1, concise introduction.
- Main content sections with consistent vertical rhythm.
- One primary call to action per section where appropriate.
- Mobile-first layout; no horizontal overflow.

## Motion
- Use short, subtle transitions.
- Respect `prefers-reduced-motion`.
- Avoid scroll-jacking and animations that move the reading surface.

## Separation of concerns
- CSS-ID owns visual tokens and presentation components.
- CSCID owns routes, content, API behavior, forms, and business rules.
- EDIT owns private administration and editor workflows.
- Content changes must be persisted by the editor backend/database, not by committing generated CSS or source files.

## Accessibility
- Maintain visible keyboard focus.
- Use semantic HTML and accessible labels.
- Keep contrast readable.
- All interactive controls must work with keyboard and touch.
