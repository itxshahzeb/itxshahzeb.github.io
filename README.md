# itxshahzeb.github.io

Personal portfolio for **Muhammad Shahzeb** — Odoo developer, Lahore.

Static, no build step. `index.html` + `style.css`, served by GitHub Pages.

## Editing

| What you want to change | Where |
| --- | --- |
| Headline, summary, prose | `index.html` |
| A project entry | the `<article class="proj">` blocks in `index.html` |
| Skills | the `<ul class="chips">` lists in `index.html` |
| Colours, type, spacing | the `:root` token blocks at the top of `style.css` |

Colours are defined once as CSS custom properties in `style.css`: the light palette on
bare `:root`, the dark palette repeated in the `prefers-color-scheme` block and the
`[data-theme="dark"]` block. Change a colour in all three to keep both themes in step.

## Preview locally

```bash
python3 -m http.server 8000
# then open http://127.0.0.1:8000
```
