# Neo-Swiss-Design

A small demo layout combining Swiss-style clarity with modern "neo" touches (subtle depth, soft shadows, and refined micro-interactions). This README explains what you'll find in `index.html` and how `style.css` controls the visuals and behavior.

## What this project is
- A minimal single-page UI demonstrating a Neo‑Swiss visual language.
- Clean typographic hierarchy, a modular grid for content/cards, and a few interactive elements.
- Intended as a starting point or reference for building clean, modern landing pages.

## index.html — structure & intent
The HTML is organized into clear semantic sections. Look for these parts:

- Header / Nav
  - Elements: `.brand`, `.nav`, `.nav__item`, `.hamburger` (if present)
  - Purpose: site title/logo on the left and simple navigation on the right. Markup is kept simple so CSS controls layout and responsive behavior.

- Hero
  - Elements: `.hero`, `.hero__title`, `.hero__subtitle`, `.hero__cta` (primary call-to-action)
  - Purpose: main selling message with a prominent CTA. The hero uses large type, spacing, and optional visual accent (image or decorative block).

- Grid / Cards
  - Elements: `.grid`, `.card`, `.card__title`, `.card__body`, `.card__meta`
  - Purpose: modular content blocks arranged with CSS Grid or Flexbox. Cards show how components adapt across viewports.

- Footer
  - Elements: `.footer`, `.footer__links`
  - Purpose: small area for extra navigation and copyright.

- Utilities / helpers
  - Small utility classes (spacing, text-muted, visually-hidden) are used to keep HTML minimal and styles consistent.

## style.css — what to expect and how it works
The stylesheet implements the Neo‑Swiss look using a few core patterns:

- CSS custom properties (variables)
  - Typical variables: --bg, --surface, --text, --muted, --primary, --accent, --radius, --gap
  - Change these at the top of the file to quickly retheme the whole page.

- Typography
  - Clear font scale with variables or root font-size.
  - Utility classes and element rules set visual hierarchy (h1, h2, p, small).

- Layout system
  - A responsive grid: `.container` centers content; `.grid` uses CSS Grid with auto-fit/auto-fill for responsive columns.
  - Spacing is based on a consistent gap scale (e.g., var(--gap)).

- Card and surface styling
  - Cards use a neutral surface color, subtle border radius, and soft elevation (shadow or backdrop-filter for a glass effect).
  - Class examples: `.card`, `.card--highlight`, `.glass`.

- Hero and CTA
  - Hero uses larger type, wide spacing, and a prominent `.btn` or `.cta` style with hover/focus states.
  - CTAs include visible focus outlines for accessibility.

- Interactions & motion
  - Small transitions on hover/focus for buttons, links, and cards (transform, box-shadow, opacity).
  - Motion is subtle to keep the design crisp.

- Responsive breakpoints
  - Media queries adjust font sizes, grid columns, and navigation (mobile hamburger vs desktop inline nav).

## How to preview
1. Open `index.html` in a browser (double-click or use your editor's Live Server).
2. Resize the viewport to see responsive behavior (grid columns collapsing, nav switching to hamburger).

## Customization tips
- Theme: modify CSS variables at the top of `style.css` to change colors, radii, spacing.
- Typography: swap the font-face or adjust root font-size and scale variables to shift the whole rhythm.
- Layout: tweak `.grid`'s grid-template-columns or the container max-width for denser or more airy layouts.
- Accessibility: ensure color contrast for text on top of accented backgrounds; keep focus outlines visible.

## Notes for contributors
- Keep semantic HTML and small, reusable CSS classes.
- Prefer variables and utility classes for consistent spacing and color use.
- Document any new components or utility classes in this README.

## License
- Add your preferred license text or file (e.g., MIT) if you plan to distribute this template.