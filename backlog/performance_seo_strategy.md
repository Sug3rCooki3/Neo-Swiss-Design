# Performance & SEO Strategy

## Performance Strategy
**Target Score:** 100/100 (Lighthouse/Core Web Vitals)

### Core Principles
1.  **Zero-Runtime Overhead:**
    *   No client-side JavaScript frameworks (React, Vue, etc.) required for initial render.
    *   Pure HTML/CSS architecture.
2.  **Asset Optimization:**
    *   **CSS:** Minified and critical CSS inline (future optimization). Currently single lightweight file.
    *   **Images:** Use modern formats (WebP/AVIF) and explicit `width`/`height` attributes to prevent Layout Shifts (CLS).
    *   **Fonts:** Preconnect to font origins (`fonts.gstatic.com`).
3.  **Rendering Metrics:**
    *   **LCP (Largest Contentful Paint):** Optimized by keeping the Hero section text-based and lightweight.
    *   **CLS (Cumulative Layout Shift):** 0.0. All dimensions are defined in CSS Grid.
    *   **FID (First Input Delay):** Near zero due to lack of blocking JS.

### Current Optimizations
*   `scroll-behavior: smooth` for better UX without heavy JS libraries.
*   CSS Variables for efficient styling without repetition.
*   `content-visibility: auto` (candidate for long pages like Timeline).

---

## SEO (Search Engine Optimization)
**Strategy:** Semantic & Content-First

### On-Page SEO
1.  **Meta Tags:**
    *   Unique `<title>` tags for every page.
    *   Unique `<meta name="description">` for every page (150-160 chars).
    *   `viewport` tag for mobile indexing.
2.  **Content Structure:**
    *   One `<h1>` per page.
    *   Semantic HTML5 tags (`<article>`, `<section>`) help crawlers understand content relevance.
3.  **Technical SEO:**
    *   **Mobile-First:** The CSS is written mobile-first (`min-width` media queries), ensuring Google's mobile-first index sees the primary content.
    *   **URL Structure:** Clean, descriptive filenames (`timeline.html`, `audit.html`).
    *   **404 Prevention:** Placeholder favicon added to prevent console errors.

### Backlog
- [ ] Generate `sitemap.xml`.
- [ ] Create `robots.txt`.
- [ ] Add Open Graph (OG) tags for social media sharing.
