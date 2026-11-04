# Family First Medical — 1:1 Live Replica

Exact 100% 1:1 local mirror of the production website [https://www.familyfirstmedicalny.com/](https://www.familyfirstmedicalny.com/).

This codebase is isolated in this standalone repository so your existing Astro project (`family-first-medical-ny`) remains 100% untouched.

---

## Quick Start (Review in Localhost)

To run the local server:

```bash
npm run dev
```

or directly:

```bash
node server.js
```

Open your browser to:
**[http://localhost:3000](http://localhost:3000)**

To run on a different port (e.g. 8080):
```bash
PORT=8080 npm run dev
```

---

## What is Included

1. **`index.html`**
   - Exact markup, meta tags, and open graph tags from `familyfirstmedicalny.com`
   - Complete embedded CSS design tokens, typography, and responsive styles
   - Bilingual / Trilingual client-side switcher (`EN` · `中文` · `Español`)
   - Interactive sections:
     - Intro splash overlay (auto-dismiss and click/key dismiss)
     - Call Sheet bottom drawer for Elmhurst & Hicksville
     - Service tabs filtering (All · Pediatrics · Family Medicine)
     - IV therapy carousel and accordions
     - FAQ accordions
     - Mobile navigation drawer
   - Full Schema.org structured data (`MedicalClinic`, `FAQPage`, `MedicalWebPage`, `WebSite`, `Physician`)

2. **`404.html`**
   - Exact custom 404 error page from the live site

3. **`images/` (67 assets)**
   - All high-resolution doctor photos (`dr-qikai.jpg`, `dr-liyan.jpg`, transparent cutouts)
   - Clinic interior & exterior photography (Elmhurst & Hicksville locations)
   - SVG & PNG icons, badges, and background graphics
   - Web manifest icons (`icon-192.png`, `icon-512.png`, `favicon.svg`, `favicon-32.png`, `favicon.ico`)

4. **SEO & Discovery Assets**
   - `robots.txt`
   - `sitemap.xml`
   - `site.webmanifest`
   - `llms.txt` (AI agent discovery summary)
   - `agents.json` (Structured clinic schema for AI assistants)

5. **Local Dev Server (`server.js`)**
   - Zero-dependency Node.js HTTP server
   - Correct MIME types for all images, SVGs, webmanifest, and HTML
   - Clean 404 fallback handling

---

## Practice Information Reference

- **Practice**: Family First Medical (Family Medicine & Pediatrics)
- **Physicians**:
  - Dr. Qikai Yao, MD (Pediatrics & Adolescent Care)
  - Dr. Liyan Yao, MD (Family Medicine & Adult Care)
- **Offices**:
  - **Elmhurst, Queens**: 45-02 82nd Street, Elmhurst, NY 11373 · Phone: (718) 779-2248 · Open 7 Days
  - **Hicksville, Long Island**: 101 Jerusalem Avenue, Hicksville, NY 11801 · Phone: (516) 681-0681 · Mon/Tue/Fri 9-6, Sat/Sun 9-4
