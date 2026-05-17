# TechHaven | Premium Electronics Showcase

##  Project Overview
TechHaven is a fully responsive, modern e-commerce storefront built as a Week 2 software development project. This project focuses on implementing advanced CSS layouts (CSS Grid & Flexbox), fluid typography, accessible design standards, and interactive UI component structures without relying on heavy frontend frameworks.

##  Features
- **Responsive Product Grid:** Built using mobile-first CSS Grid with fluid `minmax()` mapping to handle any screen resolution dynamically.
- **Micro-interactions:** Implemented engaging CSS transitions, including scale transformations on product images and smooth lift effects on product cards during hover states.
- **Dark Mode Support:** Automatic theme switching based on the user's operating system preferences via `@media (prefers-color-scheme: dark)`.
- **Print Optimization:** Includes a print stylesheet that strips away navigation, buttons, and sidebars to present a clean, paper-friendly 2-column catalog format.
- **Accessible Design:** Maintained a strict contrast ratio exceeding 4.5:1 (WCAG AA standard) for both light and dark themes, utilizing semantic HTML elements and proper `aria-labels`.
- **E-Commerce Overlays (UI Only):** Includes structural layouts for a sliding Shopping Cart sidebar and a centralized Product Detail modal.

---

##  Design System & Architecture

### 1. Typography Hierarchy
The project uses a native system font stack to ensure instant load times and optimal readability.
- **Primary Font:** `'Segoe UI', system-ui, -apple-system, sans-serif`
- **Product Headings:** `1.5rem` (`--text-xl`) / Bold
- **Body Text / Prices:** `1.0rem` (`--text-base`)
- **Metadata / Ratings:** `0.875rem` (`--text-sm`)

### 2. Color Palette & Consistency
Managed strictly through CSS Custom Properties (`:root`) for global theme consistency.

| Element | Light Mode | Dark Mode |
| :--- | :--- | :--- |
| **Background** | `#f8fafc` (Soft White) | `#0f172a` (Deep Navy) |
| **Surface (Cards/Nav)** | `#ffffff` (Pure White) | `#1e293b` (Slate Navy) |
| **Primary Text** | `#0f172a` (Dark Slate) | `#f8fafc` (Off-White) |
| **Secondary Text** | `#475569` (Muted Blue) | `#94a3b8` (Muted Gray) |
| **Accent / CTA Button** | `#2563eb` (Royal Blue) | `#3b82f6` (Vibrant Blue) |

### 3. Spacing System
Predictable spacing is enforced using standardized custom property units:
- Small (`--space-sm`): `0.5rem`
- Medium (`--space-md`): `1rem`
- Large (`--space-lg`): `1.5rem`
- Extra Large (`--space-xl`): `2rem`

---

## Performance & Compatibility Report

### Lighthouse Target Scores
- **Performance:** 98%
- **Accessibility:** 100%
- **Best Practices:** 100%
- **SEO:** 100%

### Optimizations Applied
1. **Lazy Loading:** Native `loading="lazy"` attributes applied to images to prevent unnecessary initial bandwidth consumption.
2. **Zero Font Overheads:** Eradicated external font-fetching latencies by styling strictly with cross-platform native font configurations.
3. **Streamlined Payloads:** Organized cascading styles into a single, modular stylesheet under 5KB to completely skip rendering blocks.

### Browser Support Matrix
Tested and verified cross-platform rendering capabilities across modern engines:
- **Google Chrome / Microsoft Edge** (Chromium 115+) — Fully Functional
- **Mozilla Firefox** (Gecko 110+) — Fully Functional (Smooth transition performance)
- **Apple Safari** (WebKit 16+) — Fully Functional (Flexbox/Grid gap compliance verified)

---

## How to View Locally
1. Clone this repository to your local directory:
   ```bash
   git clone <https://github.com/Mwas1515/TechHaven.git>