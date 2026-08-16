# HVC Internationals — Website

Marketing website for **HVC Internationals**, a global import-export company specializing in Makhana (Fox Nuts) and quality agri-products.

## Pages

| File | Description |
|---|---|
| `index.html` | Home page — hero banner, about, services, portfolio, blog, contact |
| `products.html` | Product catalog / listings |
| `services.html` | Detailed services offered |
| `certifications.html` | Company certifications |
| `terms.html` | Terms & conditions |

## Project Structure

```
HVC-International-main/
├── index.html
├── products.html
├── services.html
├── certifications.html
├── terms.html
├── assets/
│   ├── css/          # Stylesheets (see below)
│   ├── js/            # JavaScript (animations, carousel, tabs, etc.)
│   ├── images/         # Site images, icons, backgrounds
│   └── fonts/           # Icon fonts (Font Awesome, Flaticon, Slick, etc.)
└── vendor/
    ├── bootstrap/       # Bootstrap CSS/JS framework
    └── jquery/          # jQuery library
```

## Stylesheets (`assets/css/`)

**Shared / vendor styles** — loaded on every page, in this order:

| File | Purpose |
|---|---|
| `fontawesome.css` | Font Awesome icon library — powers all icon glyphs across the site (social icons, service icons, arrows, checkmarks, etc.) |
| `templatemo-space-dynamic.css` | Core theme stylesheet — header/nav, section layouts, typography, footer, buttons, grid spacing. The visual foundation of the whole site |
| `animated.css` | Animate.css — scroll/load animations (`fadeInUp`, etc.) |
| `owl.css` | Owl Carousel plugin styles — sliders and carousels (dots, arrows, slide positioning) |

**Page-specific styles** — one file per page, containing only the custom CSS unique to that page:

| File | Used by | Purpose |
|---|---|---|
| `index.css` | `index.html` | Anchor-scroll offsets, full-height sections, CTA button hover color, disabling clicks on placeholder blog cards |
| `products.css` | `products.html` | Product grid/card layout |
| `services.css` | `services.html` | HVC brand color variables (navy/gold), services hero, section headings, service card styling |
| `certifications.css` | `certifications.html` | Nav-link color override for this page's header |
| `terms.css` | `terms.html` | Nav-link color override for this page's header |

Each page loads the shared vendor stylesheets first, then its own page-specific stylesheet last, so page-specific rules can override the theme defaults.

## JavaScript (`assets/js/`)

| File | Purpose |
|---|---|
| `animation.js` | Scroll-triggered animations |
| `imagesloaded.js` | Detects when images have finished loading (used by Isotope) |
| `isotope.js` | Filterable/sortable grid layouts |
| `owl-carousel.js` | Image/content carousel |
| `tabs.js` | Tabbed content sections |

## Vendor Libraries (`vendor/`)

- **Bootstrap** — grid system and base components
- **jQuery** — required by Bootstrap and the various plugins above
