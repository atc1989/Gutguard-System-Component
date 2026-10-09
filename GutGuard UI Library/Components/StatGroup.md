---
title: StatGroup
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/StatGroup.tsx
example: gutguard-ui/showcase/examples/StatGroup.tsx
parts: [w-stats, s-stats, s-sub-stats, l-stats, l-story, l-team, w-trust, s-proof]
updated: 2026-10-08
---

# StatGroup

A row of figures, each with a short label. One component for the site's big numbers, the shop's pack figures, Lifestyle's supply/streak strip, the trust band and the "Why trust this" tiles. Not for single prices (use Price).

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `editorial` | Big serif numbers in paper cards with a heat rule | `.stat-row`, `.stat` |
| `highlight` | Shop pack/plan figures; `highlight` item gets a blue wash | `.sl-stats`, `.sl-stat.hl` |
| `boxed` | Lifestyle 3-up strip; `highlight` item turns heat red | `.lw-stats`, `.lw-stat.al` |
| `trust` | Full-width band, blue numbers (FDA, USAID, …) | `.trust`, `.trust-grid`, `.trust-item` |
| `proof` | Small 4-up tiles in the trust sheet | `.sl-proof-grid`, `.pf` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | see above | `editorial` | |
| `items` | `{ value, label, highlight? }[]` | — | `value` may contain `<small>` for a mono unit (editorial) |
| `className` | string | — | |

## States

None (static). `highlight` is per item.

## Responsive

- `editorial`: one column on phone, three from `md` (900px).
- `trust`: two columns on phone (an odd last item spans both), one row from `md`.
- Boxed looks: same on all widths (equal columns).

## Source

- Original: `.stat-row` (GutguardSite.jsx:604), `.trust-grid` (GutguardSite.jsx:337), `.sl-stats` (GutguardShop.jsx:364), `.sl-proof-grid` (GutguardShop.jsx:323), `.lw-stats` (LifestyleMember.jsx:460)
- Found in: w-stats, s-stats, s-sub-stats, l-stats, l-story, l-team, w-trust, s-proof

## Accessibility

Plain text; each figure is read before its label. The `trust` band is a `<section>`.
