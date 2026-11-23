# Homepage

Personal site of **Yuheng Li** — a hand-written static page. No build step, no framework, no trackers.

**Live:** https://yu-heng-li.github.io/Homepage/ (after GitHub Pages is enabled for this repo)

## What's in here

| File | Purpose |
| --- | --- |
| `index.html` | The whole page: hero, background, focus, selected work, how I build, contact |
| `styles.css` | Minimal academic styling — paper background, hairline rules, serif headings |
| `.nojekyll` | Skips Jekyll processing so the page serves as-is |

## Bilingual

Every text node carries an `.en` and a `.zh` variant; `html[data-lang]` decides which one is visible. The `中文 / EN` button in the header toggles the attribute, updates `<html lang>`, and remembers the choice in `localStorage`. No separate translated pages.

## Run locally

```bash
python3 -m http.server 8000
# open http://127.0.0.1:8000
```

## Deploy on GitHub Pages

Settings → Pages → **Source: Deploy from a branch** → Branch `main`, folder `/ (root)` → Save.

The site uses only relative paths, so it also works on Vercel, Netlify or any subpath.

## Editing

Copy lives in `index.html`, so structure and text are in one place. Colours, type scale and spacing are CSS custom properties at the top of `styles.css`.

---

Content © Yuheng Li. If you want to reuse the layout, the CSS is yours to take.
