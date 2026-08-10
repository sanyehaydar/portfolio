# Personal Portfolio Website

A single-page personal portfolio built with plain HTML, CSS and JavaScript — no frameworks, no build tools. It's designed to showcase education, skills, certificates and small projects, which makes it a natural home page to link from a CV, LinkedIn, or a university application.

## What it does

- **Hero section** with an animated, typewriter-style tagline (pure JavaScript, `setTimeout`-based loop — no libraries).
- **About / Skills / Certificates / Projects / Contact** sections, each reachable from a sticky navigation bar with smooth scrolling.
- **Certificates** are shown as "passport stamp" cards — a small design idea that fits the story of an international applicant.
- Fully **responsive**: the layout re-flows on mobile using CSS Grid's `auto-fit`/`minmax`.
- Respects `prefers-reduced-motion` for users who disable animations.

## How it's built

| File | Purpose |
|---|---|
| `index.html` | Page structure and content |
| `style.css` | All styling, using CSS custom properties (`:root` variables) for colors so the theme can be changed in one place |
| `script.js` | The typing animation and a small helper to auto-update the footer year |

## How to run it

No installation needed — it's static HTML/CSS/JS.

1. Download or clone the folder.
2. Open `index.html` directly in a browser, **or**
3. Serve it locally for a cleaner experience:
   ```bash
   python3 -m http.server 8000
   ```
   then visit `http://localhost:8000`.

## How to make it yours

1. ✅ Already personalized with your name, email, GitHub and LinkedIn.
3. Edit the certificate cards under `#certificates` to match your own coursework.
4. Change the accent colors in `style.css` under `:root` if you want a different palette.

## What this demonstrates

- Semantic HTML structure
- CSS Grid and Flexbox for responsive layout
- CSS custom properties for theming
- Vanilla DOM manipulation and timing functions in JavaScript
- Basic accessibility consideration (`prefers-reduced-motion`, focus-friendly links)
