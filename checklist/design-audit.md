# Neo-Swiss Design Audit Checklist

Use this checklist to verify the design system implementation.

## Must Have
- [x] **12-column responsive grid (desktop), 4-col (mobile)**
  - Desktop (>= 1200px): 12 columns
  - Tablet (>= 768px): 6 columns
  - Mobile (< 768px): 4 columns
- [x] **Modern sans-serif typography**
  - Fonts: Inter, Helvetica, or system fonts
  - No decorative or script fonts
- [x] **Fluid typography**
  - Uses `clamp()` for responsive font sizing
  - Scales smoothly between viewports
- [x] **Minimal Color Palette**
  - Max 1-2 colors (Black/White/Grays + 1 Accent)
  - No bright/clashing colors
- [x] **Generous Whitespace**
  - Content has breathing room
  - Consistent spacing tokens (8px grid)

## Red Flags (Fix Immediately)
- [x] ❌ Fixed pixel layouts (must be responsive/fluid) - *Verified fluid*
- [x] ❌ Many bright colors (keep it minimal/monochrome) - *Verified monochrome + accent*
- [x] ❌ Decorative fonts or scripts - *Verified Inter only*
- [x] ❌ Tight spacing (increase margins/padding) - *Verified spacing tokens*
- [x] ❌ Breaking the grid system (elements must align to grid) - *Verified grid usage*

## Audit Notes
- Fixed duplicate `.grid` definition in `styles.css`.
- Fixed inconsistent "Get Started" casing in `index.html`.
- Fixed broken/weird link in `neo-swiss.html`.
- Moved inline styles in `timeline.html` to `styles.css`.

