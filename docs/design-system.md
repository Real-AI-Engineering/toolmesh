# ToolMesh — Design System (v0)

This repo ships a minimal static landing in `site/` with an **industrial devtools** aesthetic.

The direction is intentionally **agent-native** (machine-readable, proof-carrying, CI-first) — the UI should feel like tooling, not “marketing gradients”.

## Visual direction

- **Base:** Dark Mode (OLED-ish) + subtle depth
- **Layout:** Bento/grid cards + clear hierarchy
- **Motifs:** mesh/grid background, “evidence/receipts” artifacts, monospace highlights

## Tokens (CSS variables)

Defined in `site/styles.css` under `:root`:

- `--bg`: deep slate background
- `--surface`, `--card`: translucent panels for depth
- `--stroke`: low-contrast borders
- `--text`, `--muted`, `--muted2`: foreground ladder
- `--accent` (green): “run / pass / proof”
- `--accent2` (blue): “pipeline / infra”
- `--radius`, `--radius-lg`: rounded corners

## Typography

- **Headings / monospace:** JetBrains Mono
- **Body:** IBM Plex Sans

## Components (v0)

- Sticky topbar with brand mark + anchor navigation
- Hero with kicker + 2 CTAs + mesh diagram card
- 3-up principles grid
- “Showroom” project cards
- “Agent-to-Prod Sprint” timeline cards + CTAs

## Interaction & a11y baseline

- `:focus-visible` outline is required (keyboard nav)
- `prefers-reduced-motion` respected
- Use SVG icons (no emoji icons)
- Hover transitions: 150–300ms, subtle elevation

## Source reference (design intelligence)

This direction was sanity-checked using the local **UI/UX Pro Max** dataset (`/Users/vi/contrib/ui-ux-pro-max-skill`), which consistently recommends:

- **Dark Mode (OLED)** patterns for developer tooling
- **Bento Box Grid** for feature showcases
- **JetBrains Mono / IBM Plex Sans** pairing for technical products
