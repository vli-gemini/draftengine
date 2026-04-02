# DraftEngine Design System

Pure HTML/CSS/vanilla JS design system for the DraftEngine legal document drafting platform.

---

## Viewing the design system

### Option 1 — Open directly in your browser (no setup)

1. Clone or download this repo
2. Open `index.html` in any browser — no build step, no server needed

```bash
git clone https://github.com/vli-gemini/draftengine.git
cd draftengine
open index.html
```

### Option 2 — Run a local server (recommended for live reload)

If you have Python installed (comes with macOS):

```bash
cd draftengine
python3 -m http.server 3001
```

Then open [http://localhost:3001](http://localhost:3001) in your browser.

Or with Node.js:

```bash
npx serve . -p 3001
```

### Option 3 — Access a shared live link

If a team member has the server running and shared a public link via `ngrok` or `localtunnel`, just open that URL directly — no setup needed.

---

## File structure

```
draftengine/
├── index.html       # Design system showcase — all components
├── tokens.css       # Design tokens (primitives + light/dark semantic tokens)
└── components.css   # All component styles (.de- prefix)
```

## Tech

- **No build tools** — plain HTML, CSS, JS
- **Font Awesome Pro** — loaded via kit `32dfe1c9ba` (company account required for the full icon set)
- **Fira Sans** — loaded from Google Fonts
- **Light / Dark mode** — toggle in the top bar, driven by `data-theme` attribute on `<html>`

## Component naming

All CSS classes use the `de-` prefix (DraftEngine). Components follow MUI conventions:

| Component | Class |
|---|---|
| Button | `.de-btn--primary` `.de-btn--secondary` `.de-btn--text` `.de-btn--filled` |
| Icon Button | `.de-icon-btn--accent` `.de-icon-btn--action` `.de-icon-btn--neutral` |
| Checkbox | `.de-checkbox` + `is-checked` / `is-disabled` |
| Chip | `.de-chip--complete` `.de-chip--progress` `.de-chip--error` `.de-chip--neutral` |
| TextField | `.de-input` `.de-input--error` |
| Appbar | `.de-appbar` `.de-appbar__nav-item` |
| Sidebar | `.de-sidebar` `.de-sidebar__item` |
