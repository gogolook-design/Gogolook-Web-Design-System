# Gogolook Web Design System

## Project Overview

Single-page static website documenting the Gogolook Web Design System — a comprehensive component library and design token reference for building Gogolook-branded web interfaces. Password-protected, deployed to GitHub Pages under the `gogolook-design` organization.

## Tech Stack

- Plain HTML + inline CSS (no build tools, no npm, no frameworks)
- Google Fonts CDN for Plus Jakarta Sans, Inter, JetBrains Mono
- Client-side JavaScript for password gate and navigation
- Deployed via GitHub Pages on the `main` branch

## File Structure

```
/
├── CLAUDE.md              # This file
├── README.md              # Project readme
├── index.html             # Single-page design system (all sections)
└── assets/                # Future: component screenshots, icons
```

## Design Tokens Quick Reference

### Colors

| Name            | Hex       | CSS Variable     |
|-----------------|-----------|------------------|
| Gogolook Blue   | `#0058EA` | `--gl-blue`      |
| Shadow Blue     | `#0F2647` | `--gl-shadow`    |
| Clear Horizon   | `#00C0FE` | `--gl-horizon`   |
| Neo Green       | `#01D3B8` | `--gl-green`     |
| Genuine Blue    | `#008CF4` | `--gl-genuine`   |

Each brand color has tint scale: 01 (lighter), 02 (mid), 03 (lightest).

### Typography

| Usage    | Font Family       | Source           |
|----------|-------------------|------------------|
| Headings | Plus Jakarta Sans | Google Fonts CDN |
| Body     | Inter             | Google Fonts CDN |
| Code     | JetBrains Mono    | Google Fonts CDN |

### Grid

- 12 columns, 24px gutter, 1200px max width
- Base unit: 4px
- Breakpoints: 375 / 768 / 1024 / 1440

## Password Gate

**Accepted passwords:** `gogolook2026`, `1234`

Client-side JavaScript password protection using sessionStorage for persistence.

## Sections

1. **Overview** — Quick reference, getting started
2. **Colors** — Brand palette, tint scales, neutrals, semantic colors
3. **Typography** — Type scale, font weights, specimens
4. **Spacing** — 4px-based spacing scale with visual bars
5. **Border Radius** — Token scale from sm to full
6. **Shadows** — Shadow Blue-tinted elevation levels
7. **Gradients** — Standard, duotone, blue, fresh, dark
8. **Buttons** — Primary, secondary, ghost, dark; sizes and states
9. **Cards** — Default, flat, featured variants
10. **Text Inputs** — Fields, selects, textareas, error states
11. **Selection Controls** — Checkboxes, radio buttons, switches
12. **Badges & Tags** — Color variants, interactive tags
13. **Navigation** — Light and dark nav bars
14. **Tabs** — Tab strip component
15. **Alerts** — Info, success, warning, error
16. **Avatars** — Sizes and avatar groups
17. **Dividers** — Simple and labeled dividers
18. **Progress** — Linear progress bars
19. **Tooltips** — Tooltip component
20. **Layout & Grid** — 12-column grid, breakpoints, containers
21. **Dark Mode** — Surface tokens, component adaptations
22. **Animation** — Transition tokens, entrance animations
23. **Accessibility** — WCAG AA contrast, focus states, checklist

## Deployment

1. Push changes to the `main` branch
2. GitHub Pages serves from the root of `main`
3. No build step required

## Constraints

- No build step, no npm, no package.json
- All CSS is inline in `index.html`
- Fonts loaded from Google Fonts CDN only
- Keep the site as a single `index.html` file
- All component demos are live HTML, not screenshots
