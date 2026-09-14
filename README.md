# kaav-site

Source for kaav.eu.

## Local dev
Just open `public/index.html` in a browser — no build step, plain static HTML/CSS/JS.

## Deploy
Cloudflare Workers (static assets), deployed from this repo's `main` branch via
`npx wrangler deploy`. Assets directory: `public/`.

## Editing
- Pages: `public/index.html`, `public/about.html`, `public/privacy.html`
- Styles: `public/style.css` (one shared stylesheet, CSS variables at the top for colors)
- Homepage brand grid: edit `public/brands.js` — one entry per tile, see comments in the file
- Brand logo files live in `public/logos/` (see `public/logos/README.md`)
- KAAV's own mark: `public/logo.svg`, used in the nav and hero

## Status
- [x] v1 holding page (name, one-line description, contact email)
- [x] About / Contact page
- [x] Privacy Policy page
- [x] Custom domain + email verified for Apple Developer org enrollment
- [x] Warm/light redesign using the KAAV logo's colors
- [ ] Brand grid — Ass Savers and Strawbees added; still need Creatables, projection
      mapper, Föräldraplånbok, Sound memory (confirm which have a public URL vs.
      stay text-only), plus real logo files in `public/logos/`
