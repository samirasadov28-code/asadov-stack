# AI Product Portfolio — Portfolio Terminal

Single-page site. Drop this folder onto Netlify (Netlify Drop: https://app.netlify.com/drop)
or run `netlify deploy --dir=. --prod` after `npm install -g netlify-cli`.

## Adding logos

Place files in `assets/logos/` using these filenames:
- `uvidnova.png` — uVidNova (UVN)
- `modelup.png` — ModelUp (MUP)
- `roofsolar.png` — RoofSolar (RSL)
- `polymind.png` — PolyMind (PMD)
- `dishroll.png` — DishRoll (DSH)
- `mortwise.png` — MortWise (MWS)
- `storyroute.png` — StoryRoute (SRT)

If a logo is missing, the ticker symbol shows as a clean fallback — the site still looks good with no logos at all.

## Customization quick map

- Edit product copy, tickers, categories, accent colors: `gen_site.py` PRODUCTS list, re-run.
- Edit visual theme: CSS block in `gen_site.py` (CSS variables at top of `:root`).
- Swap fonts: change the Google Fonts link in the `<head>`.

## Iframe previews

Each card shows a live, zoomed-out iframe of the actual product. If a site blocks
embedding (X-Frame-Options / CSP), a styled fallback panel shows instead after a 5s
timeout — visitor experience stays clean either way.
