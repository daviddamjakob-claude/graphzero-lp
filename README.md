# ascending-lp

Static landing page for Ascending AI — "The toolbox to deploy enterprise AI".

A copy of the design-option `/5` variant of the Ascending landing page, deployed
as a plain static site.

## Structure

```
index.html                       markup for the whole page
favicon.svg                      brand mark
assets/site.css                  page-level styles
assets/site.js                   accordion / scroll behaviour
assets/design-system/
  styles.css                     entry point — import order is load-bearing
  tokens/                        fonts, colors, typography, spacing, shape, motion,
                                 semantic aliases, themes
  styles/                        base, typography, layout, components
```

No build step and no dependencies — the fonts come from Google Fonts, everything
else is served from this repo.

## Running locally

```bash
python -m http.server 8000
```

Then open http://localhost:8000.

## Deployment

Served by GitHub Pages from the `main` branch root.
