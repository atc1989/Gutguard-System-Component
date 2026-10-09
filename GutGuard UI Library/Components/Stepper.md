---
title: Stepper
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/Stepper.tsx
example: gutguard-ui/showcase/examples/Stepper.tsx
parts: [l-settings]
updated: 2026-10-08
---

# Stepper

Minus / value / plus pill for small counts, like capsules per dose in Lifestyle settings. Not for free numeric entry; use TextField with `type="number"`.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| default | − 2 capsules + | `.lw-step` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `label` | string | — | Group name, e.g. "Reveille capsules" |
| `value` | number | — | Controlled |
| `defaultValue` | number | 0 | Uncontrolled |
| `onChange` | (n: number) => void | — | |
| `min` | number | 0 | − disables at min |
| `max` | number | 99 | + disables at max |
| `unit` | string | — | Grey word after the number |

## States

default / active (scale .97) / focus-visible / disabled (− at min, + at max: ink-4, no fill)

## Responsive

Same on all widths.

## Source

- Original: `.lw-step` in LifestyleMember.jsx:1102 (settings sheet)
- Found in: l-settings

## Accessibility

`role="group"` with `aria-label`. Buttons are named "One less: <label>" / "One more: <label>". The number is `aria-live="polite"` so changes are read out.
