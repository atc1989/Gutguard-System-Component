---
title: Spinner
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML (.spinner, .partner-spinner)
---

# Spinner

Loading indicator. Pair with text when the wait is >1s.

## Variants

| Variant | Spec |
|---|---|
| Inline | 18px ring, currentColor, on buttons |
| Block | 28–36px centered in a panel |
| Page | Centered on bone with optional “Loading…” ink-3 |

## Motion

- `.8s linear infinite` rotation
- Honor `prefers-reduced-motion` — slow pulse or static “Loading” text instead

## Color

- On bone/paper: blue or ink
- On blue/ink buttons: bone

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint. Center in the loading region; page-level spinner respects safe areas / bottom bar.

## Finalize
- [ ] One SVG/CSS recipe in portable CSS
- [ ] Mark **Final**
