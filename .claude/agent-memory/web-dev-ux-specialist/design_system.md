---
name: Sistema de diseño Loginco
description: Paleta de colores, tipografía y tokens CSS del proyecto Loginco
type: project
---

**Paleta de colores:**
- Accent principal: `#4C50D4` (azul índigo)
- Hover/dark: `#3638B8`
- Tint claro: `#EEEEF9` (bg-accent-tint)
- Hero background: `linear-gradient(rgba(10,10,60,0.88), rgba(20,20,90,0.78))` sobre imagen Unsplash warehouse
- Sección tecnología bg: `linear-gradient(135deg, #0d0d4a 0%, #1a1b6e 100%)` — clase `.security-badge`

**Clases CSS custom (no Tailwind):**
- `.text-accent` / `.bg-accent` / `.border-accent` — color #4C50D4
- `.hover:bg-accent-dark` — color #3638B8
- `.btn-primary` — botón filled con hover lift + shadow
- `.btn-outline` — botón bordeado que rellena al hover
- `.service-card` — tarjeta con hover lift y border-color accent
- `.section-title` / `.section-title-center` — underline decorativo de 60px con pseudo-element
- `.timeline-step` — con `::after` que dibuja línea conectora horizontal (oculta en mobile)
- `.faq-item` — hover bg #f5f5fd, cursor pointer
- `.hero-bg` — background image + gradient, min-height 85vh
- `.security-badge` — fondo oscuro azul marino para sección tecnología
- `.bg-accent-tint` — fondo #EEEEF9 para iconos en cards
- `.stat-number` — font-size 2.5rem, font-weight 800, color accent

**Tipografía:** Inter (Google Fonts), pesos 300/400/500/600/700/800

**Tailwind config (en <script> del head):** Colores extendidos con `primary: '#4C50D4'`
