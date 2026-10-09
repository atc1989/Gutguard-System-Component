---
title: Switch
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Switch

Binary on/off control for settings. Prefer [[Components/Segmented Control]] when choosing among **named modes** (e.g. Trial / Protocol); use Switch for a single boolean.

## Spec

- Track: width ~44px · height ~26px · radius pill
- Thumb: ~20px circle · paper fill · subtle shadow
- Off: track `--bone-deep` / rule
- On: track `--blue`; thumb stays paper
- Focus-visible: gold ring on the control
- Optional label to the right (Inter Tight 14–15px / 600)

## A11y

- `role="switch"`
- `aria-checked="true|false"`
- Keyboard: Space / Enter toggles
- Associate with visible label via `aria-labelledby` or wrapping `<label>`

## Do / don’t

- **Do** animate thumb with short ease; respect `prefers-reduced-motion`
- **Don’t** use Switch for multi-option filters — use Segmented or checkboxes
- **Don’t** use purple/teal track fills — blue only when on

## Portable CSS

`.gg-switch` — see [[03 - Portable CSS Starter]]

## Showcase

`Showcase/index.html` → `#switch`

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint. Keep 44×26 track; pair with label in a wrapping row. Touch target for the control ≥44px height via padding if needed.

## Finalize
- [ ] Mark **Final** when used in a second product
