# Design System Specification

## Archetype: "The Modernist Architect"
**Personality:**
*   **Objective:** Presents information without decoration or bias.
*   **Functional:** Every element serves a purpose; form follows function.
*   **Timeless:** Avoids trends in favor of established typographic principles.
*   **Precise:** Aligns to the grid strictly.

**Voice & Tone:**
*   Direct, concise, and professional.
*   Avoids marketing fluff or emotional manipulation.
*   Uses sentence case for headings.

---

## Style Specification (Neo-Swiss)

### 1. Grid System
A fluid, responsive grid that adapts to the viewport.
*   **Mobile (< 768px):** 4 Columns, 12px Gutter.
*   **Tablet (≥ 768px):** 6 Columns, 16px Gutter.
*   **Desktop (≥ 1200px):** 12 Columns, 24px Gutter.
*   **Container:** Max-width 1200px, centered.

### 2. Typography
**Font Family:** `Inter` (Sans-serif).
**Scale:** Fluid typography using `clamp()`.
*   **Base Text:** `16px` - `18px`.
*   **H1:** `36px` - `64px` (Weight: 700, Tracking: -0.02em).
*   **H2:** `22px` - `28px` (Weight: 700, Tracking: -0.02em).
*   **H3:** `18px` - `22px` (Weight: 700).
*   **Line Height:** `1.45` (Body), `1.1` (Headings).

### 3. Spacing (8px Baseline)
All spacing is derived from the base unit `--space` (8px).
*   `--space-1`: 8px
*   `--space-2`: 16px
*   `--space-3`: 24px
*   `--space-4`: 32px
*   `--space-6`: 48px
*   `--space-8`: 64px

### 4. Color Palette
High contrast, monochrome foundation with a single functional accent.
*   **Background:** `#ffffff` (White)
*   **Surface:** `#fbfbfb` (Off-white for cards)
*   **Text:** `#0b0b0b` (Near Black)
*   **Muted Text:** `#575757` (Dark Gray - WCAG AA compliant)
*   **Accent:** `#0074ff` (Swiss Blue - Used for links/focus only)

### 5. Components
*   **Cards:** Flat, no shadow, subtle background distinction.
*   **Buttons:**
    *   *Primary:* Solid black, white text.
    *   *Ghost:* Transparent, borderless (or subtle border), text color.
*   **Timeline:** Vertical line with semantic `<time>` elements.
