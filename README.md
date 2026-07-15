# Pebble Design System

Design tokens, reference screens, and component specs for the Pebble app.

## Structure

```
design-tokens/   Color, typography, spacing, radius, and shadow values (JSON)
assets/logos/    Pebble logo files (mark, lockups, mono)
screens/         Static HTML reference screens, in flow order
components/      Component specs (empty — TBD)
charts/          Chart specs (empty — TBD)
docs/            Brand guidelines, handoff notes, states, interactions, screen flow
```

## Screen flow

| # | Screen | File |
|---|---|---|
| 1 | Splash | `screens/01-splash.html` |
| 2 | Onboarding (1/3) | `screens/02-onboarding-1.html` |
| 3 | Onboarding (2/3) | `screens/03-onboarding-2.html` |
| 4 | Onboarding (3/3) | `screens/04-onboarding-3.html` |
| 5 | Log in | `screens/05-login.html` |
| 6 | Sign up | `screens/06-signup.html` |
| 7 | Home | `screens/07-home.html` |

## Status

`screens/07-home.html` is the original Claude-exported artifact (bundled/opaque format). Screens 01–06 are newly authored, plain static HTML/CSS built from the same design tokens — no framework, not componentized.

Onboarding copy (headlines/subtext) is placeholder — the actual product value proposition wasn't available when these were built. Replace before shipping.

All five token files in `design-tokens/` are populated, but derived only from `07-home.html`. They cover what appears on that one screen — not dark mode, error/disabled states, or anything not yet designed.

Brand identity (logo, color, type) had no prior source — see [`docs/brand-guidelines.md`](docs/brand-guidelines.md) and the rendered [`docs/brand-guidelines.html`](docs/brand-guidelines.html) (open in a browser). Treat as a first draft pending sign-off.

See [`docs/handoff.md`](docs/handoff.md) for current scope and known gaps before building against this.

## Tokens

- `colors.json` — brand palette (OKLCH) + neutral text/surface/background scale
- `typography.json` — font family, size scale, weights, line-height, letter-spacing
- `spacing.json` — spacing scale (px)
- `radii.json` — corner radius scale
- `shadows.json` — elevation shadows + one colored glow variant
