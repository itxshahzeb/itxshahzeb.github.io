# itxshahzeb.github.io

Personal portfolio for **Muhammad Shahzeb** — Odoo developer, Lahore.

Static, no build step, no dependencies. `index.html` + `style.css`, served by GitHub Pages.

## Editing

| What you want to change | Where |
| --- | --- |
| Headline, lead, availability pill | the `.hero` section in `index.html` |
| The four numbers under the hero | the `<dl class="herometa">` block |
| A project | the `<article class="card">` blocks under `#work` |
| Smaller builds | the `<article class="row">` blocks under "Also shipped" |
| What you offer freelance | the `<article class="cap">` blocks under `#capabilities` |
| Skills | the `<ul>` lists inside `.stack` |
| Colours, spacing, radius | the `:root` token blocks at the top of `style.css` |
| Your photo / CV | `assets/portrait.jpg`, `assets/Muhammad-Shahzeb-CV.pdf` |

### Colours

Dark is the default palette and lives on bare `:root`. The light palette is repeated twice —
once in the `prefers-color-scheme: light` block and once in `[data-theme="light"]` — so that an
explicit toggle beats the OS setting. **Change a colour in all three places** or the themes drift
apart.

To switch the accent (for example to teal), change `--accent`, `--accent-strong`, `--accent-ink`,
`--accent-soft` and `--accent-glow` in each block.

### Marking a skill as important

Add `class="hot"` to a `<li>` in the `.stack` lists and it picks up the accent colour.

## Preview locally

```bash
python3 -m http.server 8000
# then open http://127.0.0.1:8000
```

## Checklist before pushing

- Both themes (click the toggle in the nav)
- Narrow window / phone width — the nav collapses to a menu button under 760px
- Tab through the page: the skip link, nav, buttons and links all take a visible focus ring
