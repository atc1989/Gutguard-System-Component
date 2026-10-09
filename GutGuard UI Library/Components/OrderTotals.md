---
title: OrderTotals
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/OrderTotals.tsx
example: gutguard-ui/showcase/examples/OrderTotals.tsx
parts: [s-tots, s-basket]
updated: 2026-10-08
---

# OrderTotals

Label/value rows that end in a big serif total. Use in checkout and the basket sheet.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `checkout` | Tight rows (Items, Delivery, E-Points), total under its own rule | `.co-tots`, `.co-tots .big` |
| `basket` | Airy rows (Shipping), optional note slot, total under a rule | `.sl-ship`, `.sl-tot` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | `checkout` \| `basket` | `checkout` | |
| `rows` | `{ label, value, tone? }[]` | — | `tone`: `good` (recovery blue) or `gold` (E-Points) |
| `total` | `{ label, value }` | — | Value in 26px serif |
| `note` | ReactNode | — | Between rows and total, e.g. a delivery [[Note]] |

## States

None (static).

## Responsive

Same on all widths.

## Source

- Original: `.co-tots` (GutguardShop.jsx:670), `.sl-ship`, `.sl-tot` (GutguardShop.jsx:488)
- Found in: s-tots, s-basket, s-co

## Accessibility

Rows and total are `<dl>` lists (`dt` label, `dd` value).
