# Gemini — Vera

UI prototypes built with pure HTML, CSS, and vanilla JS. No build tools or dependencies.

---

## Live links

| | |
|---|---|
| **DraftEngine Dashboard** | https://vli-gemini.github.io/gemini-vera/draftengine/dashboard.html |
| **Orange Screen** | https://vli-gemini.github.io/gemini-vera/orange-screen/index.html |
| **Design System** | https://vli-gemini.github.io/gemini-vera/design-system/index.html |

---

## Run locally

```bash
cd "draftengine - vera"
python3 -m http.server 3001
```

---

## File structure

```
gemini-vera/
├── design-system/
│   ├── index.html       # Component showcase
│   ├── tokens.css       # Design tokens (light + dark)
│   └── components.css   # Component styles (.de- prefix)
├── draftengine/
│   └── dashboard.html   # DraftEngine app
├── orange-screen/
│   └── index.html       # Orange Screen app
└── assets/
    └── logo.png
```

## Tech

- Pure HTML/CSS/JS — no build tools
- **Font Awesome Pro** — via kit (company account required)
- **Fira Sans** — Google Fonts
- Light/dark mode via `data-theme` on `<html>`
- Shared design system used across all apps
