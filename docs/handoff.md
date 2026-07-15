# Handoff Notes

## Scope as of this handoff

- One reference screen: `screens/home-screen.html`. Static HTML/CSS, not built as components in any framework.
- `design-tokens/*.json` are populated, but every value was extracted from `home-screen.html` alone. Treat them as "what's confirmed so far," not a complete system.
- `components/`, `charts/`, `assets/` are empty placeholders — no component breakdown, icons, or logos exist yet.
- `docs/states.md`, `docs/interactions.md`, `docs/screen-flow.md` are empty stubs.

## Known gaps

- No dark mode colors.
- No disabled/hover/pressed/error state colors beyond what's inline in the one screen.
- No documented interaction behavior (loading states, transitions, gestures).
- No screen-to-screen flow — only one screen exists, so navigation/IA is undefined.
- Token naming is provisional (e.g. `surfaceAlt`–`surfaceAlt4` are four near-identical off-whites pulled straight from inline styles — may need consolidating or renaming once more screens clarify intent).

## Suggested next steps for engineering

1. Confirm token values/names with design before wiring them into a theme file.
2. Componentize `home-screen.html` — break it into the pieces implied by `components/`.
3. Flag any missing states/colors needed as components are built, so tokens can be extended rather than improvised per-component.
