# Pebble Design System

Design tokens, reference screens, and component specs for the Pebble app.

## Structure

```
design-tokens/   Color, typography, spacing, radius, and shadow values (JSON)
screens/         Static HTML reference screens
components/      Component specs (empty — TBD)
charts/          Chart specs (empty — TBD)
assets/          Icons, logos, images (empty — TBD)
docs/            Handoff notes, states, interactions, screen flow
```

## Status

One reference screen exists: `screens/home-screen.html`, a static HTML/CSS mockup (not componentized, no framework).

All five token files in `design-tokens/` are populated, but derived only from `home-screen.html`. They cover what appears on that one screen — not dark mode, error/disabled states, or anything not yet designed.

See [`docs/handoff.md`](docs/handoff.md) for current scope and known gaps before building against this.

## Tokens

- `colors.json` — brand palette (OKLCH) + neutral text/surface/background scale
- `typography.json` — font family, size scale, weights, line-height, letter-spacing
- `spacing.json` — spacing scale (px)
- `radii.json` — corner radius scale
- `shadows.json` — elevation shadows + one colored glow variant
