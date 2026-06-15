# BrickHouse

A reusable web theme kit, extracted from the **AMD Power Play League** site —
metallic look: **gunmetal / red / gold**. Build new sites fast with a consistent style.

## Files
- **`theme.css`** — the design system: colour/font/spacing tokens + reusable components
  (nav, buttons, hero, section headings, cards, tables, callouts, footer).
- **`index.html`** — a starter page that demonstrates every component. Copy it and
  replace the content to make a new page/site.

## Quick start
1. Copy this folder (or just `theme.css`) into your new project.
2. In your HTML `<head>`, load the fonts + Font Awesome + the theme:
   ```html
   <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
   <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
   <link rel="stylesheet" href="theme.css">
   ```
3. Use the markup patterns from `index.html`.

## Component cheat-sheet
| Want | Use |
|------|-----|
| Sticky top bar | `.nav` + `.nav-logo` (`.accent` on the brand word) + `.nav-links` |
| Primary / outline button | `.btn .btn-primary` / `.btn .btn-ghost` |
| Dark hero / band | add `.surface-dark` to a `.hero` or `.section` |
| Section heading | `.eyebrow` (gold chip) + `.section-title` + `.section-sub` |
| Gold emphasis word | wrap it in `<em>` inside `.section-title` / `.hero h1` |
| Red emphasis word | `<span class="red">…</span>` |
| Feature cards | `.card-grid` > `.card` (`.card-icon`, `.card-title`, `.card-body`) |
| Data table | `.table` |
| Highlight note | `.callout` (red) or `.callout.gold` |
| Footer | `.footer` > `.footer-inner` |

## Recolour
Everything keys off CSS variables at the top of `theme.css`. To re-theme a new
brand, change a few tokens — e.g. `--red` (primary), `--gold` (accent),
`--char` (dark surface) — and the whole kit follows.

## Preview
Open `index.html` in a browser, or serve the folder:
```
python -m http.server 8001
```
then visit http://127.0.0.1:8001/index.html
