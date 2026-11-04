# AIMSS Family Health: home page design demo

Design demo of a family medicine and pediatrics practice website (home, doctors, locations, contact and draft legal pages), built for AIMSS.

**Status:** demo. All content is sample content, all photos are stand-in photos (see `public/demo/CREDITS.txt`), the request form does not send anything, and the legal pages are placeholders pending counsel. Not a live site.

## Stack
Astro 7 + Tailwind CSS 4, static output, no third-party scripts. Node 24 LTS (see `.nvmrc`).

```bash
npm install
npm run dev      # http://localhost:4321
npm run build    # static site in dist/
npm run check    # build, then fail on any external resource or dead internal link
```

## Structure
- `src/components/`: header and sticky bar; `src/components/home/` has one component per home section.
- `src/pages/`: the 17 pages.
- `src/data/`: the single source of truth for offices, doctors and draft legal text.
- `src/styles/global.css`: design tokens (colours, type, spacing).
- `public/`: images, favicon, robots and headers. Stand-in photos are in `public/demo/`.

## Design rules
- Mobile first (390 px), then desktop (1280 px).
- Brand palette: indigo, teal, gold, cream, lavender. Buttons use a deeper teal than the brand teal so white text passes WCAG AA (5.97:1).
- Accessibility target: WCAG 2.2 AA (44 px tap targets, visible focus, skip link, no horizontal overflow).

## Before launch
- Replace the stand-in photos with real practice photos.
- Confirm facts marked as slots in `src/data/` (credentials, ratings, insurance plans, new-patient status) before showing them.
- Have counsel review the legal pages.
