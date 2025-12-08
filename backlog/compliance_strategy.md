# Compliance Strategy

## GDPR (General Data Protection Regulation)
**Current Status:** Compliant (Tier 1 - Static/Informational)

*   **Data Collection:** The current build is a static HTML/CSS website. It does not collect, store, or process personal data (PII).
*   **Cookies:** No cookies are set by the application code.
*   **Third-Party Scripts:**
    *   *Google Fonts:* The site loads fonts from Google. This may leak IP addresses to Google.
    *   *Mitigation:* For strict GDPR compliance, fonts should be self-hosted locally to prevent third-party requests.
*   **Action Items for Production:**
    1.  Self-host "Inter" font files.
    2.  If analytics are added later, implement a "Prior Consent" cookie banner.
    3.  Add a Privacy Policy link in the footer.

## WCAG 2.1 (Web Content Accessibility Guidelines)
**Target Level:** AA (Silver)

### Implemented Features
1.  **Semantic Structure:**
    *   Use of `<header>`, `<nav>`, `<main>`, `<article>`, and `<footer>` landmarks.
    *   Correct Heading Hierarchy (`h1` -> `h2` -> `h3`) with no skipped levels.
2.  **Keyboard Navigation:**
    *   `Skip to content` link implemented as the first focusable element.
    *   Visible focus indicators (`:focus-visible`) using the high-contrast accent color.
    *   Logical tab order follows the DOM structure.
3.  **Visual Accessibility:**
    *   **Contrast:** Text colors (`#0b0b0b`, `#575757`) against background (`#ffffff`) meet the 4.5:1 ratio for normal text.
    *   **Scaling:** Layout uses `clamp()` and relative units (`rem`, `%`), supporting browser zoom up to 200% without breaking.
4.  **Assistive Technology:**
    *   `aria-label` used on navigation and icon-only buttons (if any).
    *   Images (future) require descriptive `alt` text.

### Validation Checklist
- [x] Lighthouse Accessibility Score > 95
- [x] Keyboard-only navigation test
- [x] Screen reader announcement of page titles
