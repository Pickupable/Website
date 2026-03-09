# Frontline Financial — Website Design Reference

## Colour Palette (current)

| Role | Hex |
|------|-----|
| Background | `#0d0d0f` |
| Surface (cards / boxes) | `#131c1a` / `#141c1a` |
| Footer background | `#080f0e` |
| Primary teal accent | `#047D6D` |
| Button hover / lighter teal | `#0a9e8a` |
| Links | `#1aaa96` |
| Link hover | `#2dc4ae` |
| Strapline / muted teal | `#047D6D` |
| Heading text | `#e8f2f0` |
| Body / paragraph text | `#90acaa` |
| Muted body text | `#608880` |
| Footer text | `#3d6860` |
| Footer legal | `#1e3d38` |

## Typography

- **Font**: Inter (Google Fonts) — weights 300, 400, 500, 600, 700
- **Base size**: 16px, line-height 1.7
- **Headings**: weight 600–700, letter-spacing -0.02em

## Design Language

- Inspired by Obsidian.md
- Dark near-black background with teal accent
- Cards and bordered boxes use subtle top-edge teal shimmer line (`::before` gradient)
- Hero section: dark teal radial glow, heading uses gradient text (white → `#1aaa96`)
- Buttons: teal gradient with glow box-shadow, 8px border-radius
- Header: sticky, `backdrop-filter: blur(12px)` frosted glass effect
- All borders use `rgba(4, 125, 109, 0.2–0.35)` — never solid teal

## Logo

### Files
- `images/logo-mark.svg` — mark only (used in site header), viewBox 160×64
- `images/logo-full.svg` — mark + wordmark (for external use), viewBox 160×100

### Concept
Four fading horizontal lines above a bold frontline — representing the choice of where to stand. The bottom line is THE frontline, distinguished by a hollow teal node at centre.

### Construction
- Candidate lines: `stroke="#047D6D"`, `stroke-width="1.5"`, opacity 0.15 / 0.25 / 0.38 / 0.55 (bottom to top)
- Gap between last candidate line and frontline (visual separation)
- Frontline: `stroke-width="2.8"`, full opacity
- Node: outer circle r=8 filled `#047D6D`, inner circle r=4 filled `white`

### Wordmark (logo-full only)
- "FRONTLINE": Inter 700, `fill="#047D6D"`, letter-spacing 3
- "FINANCIAL": Inter 300, `fill="#608880"`, letter-spacing 4

### Header usage
- `<img class="crest">` at `width: 160px; height: auto`
- No CSS filter (SVG renders its own colours)

## Repo

GitHub: `Pickupable/Website` — cloned locally to `/tmp/frontline-website`
