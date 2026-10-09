---
title: MiAgeBlock
tags: [gutguard, ui-library, section]
group: Sections
status: draft
code: gutguard-ui/components/sections/MiAgeBlock.tsx
example: gutguard-ui/showcase/examples/MiAgeBlock.tsx
parts: [w-miage]
updated: 2026-10-08
---

# MiAgeBlock

The big MiAge figure ("48 yrs") with its explanation, beside the two readings it is built on. Made for the dark slate "How we measure" band; don't put it on bone.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | One look | `.miage-block .miage-hero .mh-label .mh-beta .mh-num .mh-desc .miage-supports .ms-card .ms-name` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `label` | ReactNode | — | Gold mono label |
| `badge` | string | — | Gold outline pill after the label ("Beta") |
| `value` | ReactNode | — | Big serif figure |
| `unit` | string | — | Mono unit after it ("yrs") |
| `supports` | `{ title, tag?, text }[]` | — | Rendered as `Card variant="dark"` |
| `children` | ReactNode | — | Explanation; `<sup><a>` footnotes turn gold |

## States

None.

## Responsive

Phone: panel, then the cards, stacked. From `md` (900): panel and cards side by side (1.05fr / .95fr), cards stretch to the panel's height. Figure is fluid (64–108px).

## Source

- Original: `.miage-block` in components/GutguardSite.jsx:367 (inside `section.measure`)
- Found in: w-miage

## Accessibility

Plain text; footnotes are links. Support titles are `h3` (from `Card`).
