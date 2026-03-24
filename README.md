# CondoMaven 🏢

> Your expert guide to building and maintaining a condominium investment portfolio — from first unit to full portfolio.

CondoMaven is an informational website built with [Astro](https://astro.build) for individual investors who want to start and grow a portfolio of condominium units, beginning with zero experience.

---

## 🚀 Quick Start

### Prerequisites

- Node.js v18 or higher
- npm v9 or higher

### Install dependencies

```bash
npm install
```

### Start the development server

```bash
npm run dev
```

Visit `http://localhost:4321` in your browser.

### Build for production

```bash
npm run build
```

### Preview the production build

```bash
npm run preview
```

---

## 📁 Project Structure

```
condo-maven/
├── public/                 # Static assets (favicon, images)
│   └── favicon.svg
├── src/
│   ├── layouts/
│   │   └── Layout.astro    # Main site layout (nav, footer)
│   ├── pages/
│   │   ├── index.astro     # Home page — concept & scope
│   │   ├── roadmap.astro   # Project roadmap (6 phases)
│   │   └── faq.astro       # FAQ for new condo investors
│   └── styles/
│       └── global.css      # Global design system (variables, typography, utilities)
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

---

## 📄 Pages

| Page | Route | Purpose |
|------|--------|---------|
| Home | `/` | Explains the site concept, scope, and value proposition |
| Roadmap | `/roadmap` | 6-phase development plan with tasks and feature ideas |
| FAQ | `/faq` | Categorized Q&A for first-time condo investors |

---

## 🎨 Design System

The site uses a custom CSS design system (no external UI framework) with:

- **Color Palette**: Navy (`#0d2b45`), Gold (`#c9a84c`), Cream (`#faf8f3`)
- **Typography**: Playfair Display (headings) + Inter (body)
- **Components**: Cards, badges, callout boxes, accordion FAQ, phase roadmap
- **Responsive**: Mobile-first with breakpoints at 640px and 768px

---

## 🗺️ Development Roadmap

### Sprint 1 — Foundation ✅
- Home page with concept, scope, and CTA sections
- Roadmap page with 6 development phases
- FAQ page with 23 starter questions across 6 categories
- Global CSS design system
- Sticky navigation and footer

### Sprint 2 — Content (Planned)
- "Introduction to Condo Investing" guide article
- Condo declaration primer
- Glossary of real estate terms
- Calculator widgets (cap rate, cash-on-cash return)

### Sprint 3 — Tools & Interactivity (Planned)
- Deal analyzer tool
- Mortgage payment estimator
- Portfolio tracker template

### Sprint 4 — Community (Future)
- Newsletter integration
- Community forum / Discord
- Local market guides

---

## 💡 Developer Notes & Recommendations

### Content Structure Ideas
- Add an `/articles` collection using [Astro Content Collections](https://docs.astro.build/en/guides/content-collections/) for guide articles
- Use MDX for rich content with embedded React components (calculators, charts)
- Implement tag-based filtering for FAQ and articles

### Performance
- The site is fully static (SSG) — CDN-deployable with zero server-side overhead
- Google Fonts are loaded async; consider hosting locally to avoid external requests
- Images (when added) should use Astro's built-in `<Image>` component for optimization

### SEO
- Add `sitemap.xml` using `@astrojs/sitemap`
- Add Open Graph meta tags to the Layout for social sharing previews
- Consider `@astrojs/rss` for an article feed

### Deployment
- Works with any static host: Netlify, Vercel, Cloudflare Pages, GitHub Pages
- For Netlify/Vercel: `npm run build` → deploy `dist/` directory

### Design Enhancements
- Add a light/dark mode toggle using CSS custom properties
- Add micro-animations with CSS transitions or Motion One
- Consider adding a hero illustration or photography of urban condo buildings
- Add a progress bar or table of contents component for long guide articles

---

## ⚠️ Disclaimer

CondoMaven is for **educational and informational purposes only**. Nothing on this site constitutes financial, legal, or tax advice. Always consult qualified professionals (licensed real estate agents, CPAs, attorneys) before making investment decisions.
