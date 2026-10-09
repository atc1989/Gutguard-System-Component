---
title: BloodScanReadout
tags: [gutguard, ui-library, section]
group: Sections
status: draft
code: gutguard-ui/components/sections/BloodScanReadout.tsx
example: gutguard-ui/showcase/examples/BloodScanReadout.tsx
parts: [w-hero]
updated: 2026-10-08
---

# BloodScanReadout

The sample Blood Scan card: a title with a beta badge, three mono readings (the main one in heat), inflammation/restored bars and a caption, on paper with the heat-gold-recovery seam on top. Use as the `Hero`'s `visual`. Not for real results screens.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | One look | `.bioscan .bs-top .bs-label .bs-beta .bs-reads .bs-read(.now) .bs-bars .bs-sample` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `title` | string | — | Also the group's accessible name |
| `badge` | string | — | `Badge tone="beta"` |
| `readings` | `{ label, value, now?, word? }[]` | — | `now` = heat colour; `word` = 20px text ("High") instead of 33px |
| `bars` | `{ label, value, tone: "heat" \| "recovery" }[]` | — | Rendered with `ProgressBar showLabel` |
| `caption` | ReactNode | — | Mono line at the foot |
| `className` | string | — | Width comes from the parent (Hero sets 300px) |

## States

None.

## Responsive

Same on all widths; width is set by the parent.

## Source

- Original: `.bioscan` inside `header.hero` in components/GutguardSite.jsx:553
- Found in: w-hero

## Accessibility

`role="group"` with `aria-label={title}`. Bars are `role="progressbar"` named by their label.
