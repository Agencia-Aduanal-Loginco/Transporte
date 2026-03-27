# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static single-page marketing website for **Transportes KASU**, a freight and logistics company in Mexico. The entire site is one file: `index.html`.

## Running Locally

```bash
python3 -m http.server 8000
```

No build process, no package manager, no dependencies to install.

## Tech Stack

- **HTML5** with embedded CSS and JavaScript
- **Tailwind CSS** v3 via CDN (`https://cdn.tailwindcss.com`)
- **Font Awesome** 6.4.0 via CDN for icons
- **Google Fonts** — Montserrat (headings), DM Sans (body)
- All styling, layout, and behavior lives inside `index.html`

## Architecture

Single `index.html` with these ordered sections:
1. Header/sticky navbar (desktop + mobile hamburger menu)
2. Hero with background image (Unsplash CDN) and stat cards (500+ clients, 70+ units, 98% on-time)
3. About (Nosotros) — mission/vision and 4 stat cards
4. Services (Servicios) — 6 service cards (FCL, LCL, local, long-distance, corporate logistics, container storage)
5. Fleet (Flota) — 3 vehicle type cards
6. Coverage (Cobertura)
7. Contact/quote form (frontend only — no backend submission)
8. Footer

**Design tokens (CSS custom properties in `<style>` block):**
- `--primary-dark: #00018d` — deep blue, main brand color
- `--primary-mid: #3839bc` — medium indigo
- `--primary-light: #7e7fb7` — light purple
- `--accent: #08b8b5` — teal, used for CTA buttons
- `--accent-dark: #069e9b` — teal hover state
- Language: Spanish (`lang="es"`)

## Key Constraints

- **No form backend.** The contact form shows a success message on submit but sends no data anywhere. Any backend integration (email, CRM webhook) must be added.
- **All CDN dependencies.** The site requires internet access to render fonts and icons. For offline/production builds, these should be bundled locally.
- **No separate asset files.** All CSS overrides and JS are inline in `index.html`. Images are in `img/`.
