# DraftEngine — Vera

UI prototype built with pure HTML, CSS, and vanilla JS. No build tools or dependencies.

---

## Live links

| | |
|---|---|
| **Dashboard** | https://vli-gemini.github.io/draftengine/app/dashboard.html |
| **Design System** | https://vli-gemini.github.io/draftengine/design-system/index.html |

---

## Run locally

```bash
cd "draftengine - vera"
python3 -m http.server 3001
```

Then open `http://localhost:3001/app/dashboard.html`

---

## File structure

```
draftengine - vera/
├── design-system/
│   ├── index.html       # Component showcase
│   ├── tokens.css       # Design tokens (light + dark)
│   └── components.css   # Component styles (.de- prefix)
└── app/
    └── dashboard.html   # Main app UI
```

## Tech

- Pure HTML/CSS/JS — no build tools
- **Font Awesome Pro** — via kit (company account required)
- **Fira Sans** — Google Fonts
- Light/dark mode via `data-theme` on `<html>`
