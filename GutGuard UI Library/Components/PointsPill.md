---
title: PointsPill
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/PointsPill.tsx
example: gutguard-ui/showcase/examples/PointsPill.tsx
parts: [l-nav, g-nav]
updated: 2026-10-08
---

# PointsPill

Small paper pill in the Lifestyle top bar. Shows the member's E-Points ("15 E-POINTS"), or a plain text pill ("Log in") on the landing page. Not for main actions; use Button.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| with `points` | Gold serif number + mono label | `.lw-pts` with `b` + `span` |
| without `points` | Plain 13px semibold text pill ("Log in") | `.lw-pts` with inline font style |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `label` | string | — | Pill text, or the mono label after the number |
| `points` | number | — | Turns on the number + label look |
| `href` | string | — | Renders a link instead of a button |
| `onClick` | () => void | — | |
| `className` | string | — | |

## States

default / active (scale .97) / focus-visible (global ring)

## Responsive

Same on all widths.

## Source

- Original: `.lw-pts` (+ `.tap`) in LifestyleMember.jsx:394, LifestyleLanding.jsx:388
- Found in: l-nav, g-nav

## Accessibility

Real `<button>` or `<a>`. With points the accessible name is "15 E-Points".
