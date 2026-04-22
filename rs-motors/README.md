# RS Motors — rsmotors.bg

Premium website for **RS Motors** — automotive service and cosmetic complex in Sofia, Bulgaria.

## Stack

Zero-build static site. No framework, no dependencies, no Node toolchain required.

- `index.html` — single-page site
- `assets/` — logos, favicons, OG image
- `vercel.json` — headers + caching rules
- `robots.txt`, `sitemap.xml` — SEO

## Features

- **Bilingual** — Bulgarian (default) / English toggle, persisted in localStorage
- **Mobile-first** responsive layout
- **SEO ready** — Open Graph, Twitter Cards, JSON-LD `AutomotiveBusiness` schema
- **Editorial motorsport aesthetic** — Antonio / Fraunces / JetBrains Mono type system, red accent on carbon black
- **No backend** — purely static, deploys anywhere

## Local preview

Any static server works. The simplest:

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

Or with Node:

```bash
npx serve .
```

## Deploying to Vercel

The repo is configured for a zero-config static deployment. Either:

1. **Via CLI** — `vercel` from this directory
2. **Via GitHub** — push and import the repo from the Vercel dashboard
3. **Via Claude** — the assistant can deploy directly

## Editing content

All text lives in `index.html`. Each translatable string is duplicated with `data-lang="bg"` and `data-lang="en"` attributes — edit both when changing copy.

Prices are in the **Pricing** section (`<section class="pricing">`). They match the physical price board in the cosmetic center.

## Assets to replace with real photography

When RS Motors provides real photos, swap in:

- Hero background image (currently a pure gradient)
- Gallery car cards (currently custom SVG silhouettes)
- About section — the embossed leather logo could be replaced with a real facility photo

---

© 2022 — 2026 РС Моторс ООД
