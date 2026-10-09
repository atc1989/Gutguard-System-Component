---
title: Timeline
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/Timeline.tsx
example: gutguard-ui/showcase/examples/Timeline.tsx
parts: [w-timeline, w-proto, s-done]
updated: 2026-10-08
---

# Timeline

An ordered list of steps in three looks. Use for anything that happens in order; not for sign-up progress (use `StepProgress`).

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `checkpoints` (default) | BioScan Day 30 / 60 / 90 | `.timeline .tl-item .tl-day .tl-txt` |
| `steps` | Protocol steps with roman numerals | `.steps .step-row .step-n .step-tx` |
| `numbered` | Compact "01 02 03" next steps in a sheet | `.co-next .sl-line .nx` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | see above | `checkpoints` | |
| `items` | `{ label, title?, text? }[]` | — | `label` = "Day 30", "I", "01" |
| `className` | string | — | |

## States

None.

## Responsive

`checkpoints`: stacked on phone, 3 across from `md`. Other variants are the same on all widths.

## Source

- Original: `.timeline` in components/GutguardSite.jsx:1179; `.steps` in components/GutguardSite.jsx:648; `.co-next` in components/GutguardShop.jsx:488
- Found in: w-timeline, w-proto, s-done

## Accessibility

`ol` / `li`. Numerals in `steps` and `numbered` are `aria-hidden` (the list order carries them); checkpoint labels are read.
