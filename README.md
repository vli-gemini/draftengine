# DraftEngine — Vera

Pure HTML/CSS/vanilla JS project. No build tools, no dependencies.

---

## Viewing in your browser

### Option 1 — Run a local server (recommended)

If you have Python installed (comes with macOS):

```bash
cd "draftengine - vera"
python3 -m http.server 3001
```

Then open the links below.

Or with Node.js:

```bash
npx serve . -p 3001
```

---

### Design System

```
http://localhost:3001/design-system/index.html
```

Component library — tokens, buttons, inputs, chips, checkboxes, icons, and more.

---

### DraftEngine App

```
http://localhost:3001/app/dashboard.html
```

The main application UI — dashboard and screens built from the design system.

---

### Option 2 — Open directly (no server)

1. Clone or download this repo
2. Open `design-system/index.html` or `app/dashboard.html` directly in any browser — no setup needed

```bash
open "design-system/index.html"
open "app/dashboard.html"
```

---

## File structure

```
draftengine - vera/
├── design-system/
│   ├── index.html       # Design system showcase — all components
│   ├── tokens.css       # Design tokens (primitives + light/dark semantic tokens)
│   └── components.css   # All component styles (.de- prefix)
└── app/
    └── dashboard.html   # DraftEngine app UI
```

## Tech

- **No build tools** — plain HTML, CSS, JS
- **Font Awesome Pro** — loaded via kit (company account required for the full icon set)
- **Fira Sans** — loaded from Google Fonts
- **Light / Dark mode** — toggle in the top bar, driven by `data-theme` attribute on `<html>`

## Component naming

All CSS classes use the `de-` prefix (DraftEngine).

| Component | Class |
|---|---|
| Button | `.de-btn--primary` `.de-btn--secondary` `.de-btn--text` `.de-btn--filled` |
| Icon Button | `.de-icon-btn--accent` `.de-icon-btn--action` `.de-icon-btn--neutral` |
| Checkbox | `.de-checkbox` + `is-checked` / `is-disabled` |
| Chip | `.de-chip--complete-dark` `.de-chip--progress-dark` `.de-chip--error-dark` `.de-chip--neutral` |
| TextField | `.de-field` `.de-input` `.de-input--error` |
| Appbar | `.de-appbar` `.de-appbar__nav-item` |
| Sidebar | `.de-sidebar` `.de-sidebar__item` |
