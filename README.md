# anodized.github.io

Static company website for **Anodized Software, Inc.**, served via GitHub Pages
at [anodizedsoftware.com](https://anodizedsoftware.com/).

## Scope

A single landing page listing the company's products. The first product is
Tetsudoku, which links out to its own site at [tetsudoku.app](https://tetsudoku.app/).

- `index.html` — the landing page
- `styles.css` — styling (Figtree webfont, iridescent "anodized" accent, light/dark toggle)
- `assets/favicon.svg` — iridescent "A" mark, used as favicon and in the header
- `assets/tetsudoku-icon.png` — Tetsudoku app icon for its product entry,
  copied from the Tetsudoku site (`tetsudoku.github.io/icon.png`). Re-copy if the
  app icon changes.

## Design

Shares the design language of the Tetsudoku site (Figtree font, card layout,
light/dark toggle that respects the OS preference and persists a manual override
in `localStorage`). The company accent is an iridescent blue→violet→teal gradient
evoking the finish of anodized metal, distinguishing the company from individual
products.

## Adding a product

Duplicate the `.product` anchor block in `index.html` and update the icon, name,
tagline, description, and link. The product list is a responsive grid, so
additional entries flow automatically.

## Custom domain

`CNAME` contains `anodizedsoftware.com`. In repo **Settings → Pages**, set the
custom domain and enable **Enforce HTTPS**. DNS must point the apex domain to the
GitHub Pages IPs (or an `ALIAS`/`ANAME`), and `www` via a `CNAME` to
`anodized.github.io`.
