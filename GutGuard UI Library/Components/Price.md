---
title: Price
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/Price.tsx
example: gutguard-ui/showcase/examples/Price.tsx
parts: [w-offer, w-trialband, s-watch, l-firststep, g-first]
updated: 2026-10-08
---

# Price

A serif amount with a short caption ("Free shipping · new buyers"). Pass the amount already formatted (`₱499`).

## Variants

| Size / layout | Use for | Replaces |
|---|---|---|
| `lg` | Offer bands | `.tb-price` |
| `md` (default) | Cards and bars | `.bb-price`, Lifestyle `.ant` |
| `sm` | Option cards | `.tp` |
| `inline` | Caption beside the amount (Lifestyle) | Lifestyle first-step box |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `amount` | ReactNode | — | Formatted price |
| `caption` | ReactNode | — | |
| `inline` | boolean | — | Caption beside instead of under |
| `size` | `sm` \| `md` \| `lg` | `md` | 19 / 30 / 44px |

## States

None.

## Responsive

Same on all widths.

## Source

- Original: `.tb-price`, `.bb-price`, `.tp` in GutguardSite.css; `span.ant` in LifestyleMember.jsx
- Found in: w-offer, w-trialband, s-watch, l-firststep, g-first

## Accessibility

Plain text. Keep the currency symbol in `amount` so it is read correctly.
