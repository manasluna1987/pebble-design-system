# Handoff Notes

## Scope as of this handoff

- Full screen sequence now exists: splash → onboarding (x3) → login → signup → home (`screens/01`–`07`). See README for the flow table.
- `screens/07-home.html` is the original Claude-exported artifact (bundled format — assets/JS packed inline, not readable as plain HTML). `screens/01`–`06` are newly authored plain HTML/CSS, built from the same design tokens.
- Onboarding headline/subtext copy is **placeholder** — no real product value proposition was available when these were built. Do not ship as-is; get real copy from product/design.
- Logo and brand guidelines are new (`assets/logos/`, `docs/brand-guidelines.md`, `docs/brand-guidelines.html`) — no prior brand identity existed, so this is a first draft pending design sign-off.
- `design-tokens/*.json` are populated, but every value was extracted from `07-home.html` alone. Treat them as "what's confirmed so far," not a complete system.
- `components/`, `charts/` are still empty placeholders — no component breakdown or chart specs exist yet.
- `docs/states.md`, `docs/interactions.md`, `docs/screen-flow.md` are empty stubs.

## Known gaps

- No dark mode colors.
- No disabled/hover/pressed/error state colors beyond what's inline in the one source screen.
- No documented interaction behavior (loading states, transitions, gestures, form validation).
- Screen flow is linear/assumed (splash → onboarding → auth → home) — not confirmed against real product IA. Password reset, social-auth success/failure states, and post-signup flows aren't designed.
- Token naming is provisional (e.g. `surfaceAlt`–`surfaceAlt4` are four near-identical off-whites pulled straight from inline styles — may need consolidating or renaming once more screens clarify intent).
- Logo is a first-pass mark with no design sign-off — expect it to change.

## Suggested next steps for engineering

1. Confirm token values/names and the logo with design before wiring them into a theme file / app icon.
2. Get real onboarding copy before building those screens for real.
3. Componentize the screens — break them into the pieces implied by `components/`.
4. Flag any missing states/colors needed as components are built, so tokens can be extended rather than improvised per-component.
