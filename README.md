# Yecommerce.io — Static Site

Static site for [yecommerce.io](https://yecommerce.io), migrated from WordPress/Breakdance (June 2026).
Deployed via Netlify with GitHub auto-deploys.

## Structure
- Folder-per-page with `index.html` to preserve clean URLs (`/services/`, `/pricing/`, ...)
- `assets/css/main.css` — shared styles (nav, footer, base, buttons)
- Page-specific styles inline in each page's `<head>`
- `_redirects` — 301s from old WordPress slugs (e.g. `/pricing-2/` → `/pricing/`)

## Key wiring
- Contact form → Formspree `xqegalnd` (thank-you redirect configured in Formspree dashboard)
- Booking → calendly.com/jamesgrasty/15min
- Analytics: GA4 `G-0S82XL4HF1` + Google Ads `AW-1068863832` on all pages;
  conversion event fires on `/thank-you/` only
