# Pebble Brand Guidelines

No brand assets existed prior to this — logo and identity below were derived from the color/type/shape language already present in `screens/07-home.html` (see `design-tokens/`). Treat as a first draft pending design sign-off, not a finalized identity.

## Logo

Files in `assets/logos/`:

- `pebble-mark.svg` — icon only. Use for app icon, favicon, small spaces.
- `pebble-logo.svg` — mark + wordmark, ink text. Primary lockup, light backgrounds.
- `pebble-logo-dark.svg` — mark + wordmark, light text. Use on dark/brand-color backgrounds.
- `pebble-logo-mono.svg` — single-color (ink) version. Use where color isn't available (stamps, single-color print, watermarks).

**Clear space**: keep padding around the logo at least equal to the height of the mark.
**Minimum size**: don't render the mark below 20px, or the wordmark lockup below 88px wide — the wordmark stops being legible.
**Don't**: stretch, recolor outside the variants above, rotate, or add drop shadows/effects to the logo.

## Color

Full values in `design-tokens/colors.json`.

| Token | Value | Use |
|---|---|---|
| `brand.primary` | `oklch(0.68 0.19 145)` | Primary actions, brand mark |
| `brand.accent` | `oklch(0.62 0.19 35)` | Secondary CTA, highlights |
| `brand.accentAlt` | `oklch(0.72 0.18 45)` | Alt accent |
| `brand.info` | `oklch(0.62 0.17 255)` | Informational states |
| `brand.warning` | `oklch(0.75 0.16 90)` | Warning states |
| `brand.danger` | `oklch(0.6 0.2 25)` | Errors, destructive actions |
| `neutral.ink` | `#1C1B19` | Primary text |
| `neutral.textSecondary` | `#57544E` | Secondary text |
| `neutral.textTertiary` | `#6B6862` | Tertiary text |
| `neutral.textMuted` | `#8A8782` | Placeholder / muted text |
| `neutral.surface` | `#FFFFFF` | Cards, elevated surfaces |
| `neutral.surfaceAlt` – `surfaceAlt4` | `#F0EFEA`–`#EDEBE6` | Background variants (near-identical, provisional — may consolidate) |
| `neutral.background` | `#F7F5F1` | App background |

## Typography

Full scale in `design-tokens/typography.json`.

- **Font family**: `Inter`, falling back to `-apple-system, BlinkMacSystemFont, sans-serif`
- **Weights**: 400 (regular), 500 (medium), 600 (semibold), 700 (bold), 800 (extrabold)
- **Sizes**: 10px–23px, 13 steps (see token file for full scale)
- **Letter-spacing**: tighter tracking (−0.2px to −0.5px) on larger/bold text

## Spacing, radius, shadow

See `design-tokens/spacing.json`, `radii.json`, `shadows.json`. Notably: the dominant corner radius across the source screen is a sharp `2px`, with larger radii (18–30px, plus `50%` for circular elements) used selectively — not a uniform rounded style.
