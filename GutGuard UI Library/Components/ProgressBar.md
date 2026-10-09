---
title: ProgressBar
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/ProgressBar.tsx
example: gutguard-ui/showcase/examples/ProgressBar.tsx
parts: [l-watch, l-story, w-hero]
updated: 2026-10-08
---

# ProgressBar

Thin bar that shows how far along something is: the 5-Night Watch, Day 4 of 90, or a Blood Scan reading. The heading or badge above it ("NIGHT 3 OF 5") belongs to the caller.

## Variants

| Tone | Use for | Replaces |
|---|---|---|
| `journey` | Lifestyle progress; heat → gold → recovery gradient, remainder in rule-soft, paper ticks between `segments` | inline bars in LifestyleMember.jsx |
| `heat` | Inflammation reading on a bone-deep track | `.bs-fill.heat` |
| `recovery` | Restored reading on a bone-deep track | `.bs-fill.rec` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `value` | number | — | |
| `max` | number | 100 | |
| `label` | string | — | Accessible name; shown on the left with `showLabel` |
| `showLabel` | boolean | — | 80px mono label column (`.bs-bar .k`) |
| `tone` | `journey` \| `heat` \| `recovery` | `journey` | |
| `segments` | number | 1 | journey only: 5 nights, 3 phases |
| `thin` | boolean | — | 6px instead of 8px |
| `className` | string | — | |

## States

Static. heat / recovery fills animate width on change (1.6s), off with reduced motion.

## Responsive

Same on all widths.

## Source

- Original: `.bs-bar`, `.bs-track`, `.bs-fill` in GutguardSite.jsx:553; inline bars in LifestyleMember.jsx:586 and :998
- Found in: l-watch, l-story, w-hero

## Accessibility

`role="progressbar"` with `aria-valuenow/min/max` and `aria-label`. The visible label is hidden from screen readers to avoid reading it twice. The site fills' off-token light ends (#ff8a6b, #7fc0ee) are approximated with token alpha.
