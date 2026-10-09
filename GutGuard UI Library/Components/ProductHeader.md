---
title: ProductHeader
tags: [gutguard, ui-library, component]
group: Patterns
status: draft
code: gutguard-ui/components/patterns/ProductHeader.tsx
example: gutguard-ui/showcase/examples/ProductHeader.tsx
parts: [s-top, s-card]
updated: 2026-10-08
---

# ProductHeader

The top of the shop: product art, name and tagline with the basket button on phone; inside the desktop buy card, a mono label with the basket. Reuses [[IconButton]] (round, with count).

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| product row (pass `name`) | Phone shop header: art + "SynBIOTIC+" + tagline + basket | `.sl-top`, `.sl-prow` (`.nm`, `.tg`), `.sl-cart` |
| card label (pass `label`) | Desktop buy card header: "Choose how to start" + basket | `.sl-top.slw-top`, `.slw-t` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `name` | ReactNode | — | Product name, rendered as `<h1>` |
| `tagline` | ReactNode | — | |
| `image` | ReactNode | — | Product art, 62px wide |
| `label` | ReactNode | — | Used when there is no `name` |
| `basketCount` | number | — | Count bubble; hidden at 0 |
| `onBasket` | () => void | — | |
| `basketHref` | string | — | Makes the basket a link |

## States

Basket button: hover blue border, focus-visible gold ring (from IconButton).

## Responsive

Same on all widths. The page chooses the product row on phone and the card label on desktop.

## Source

- Original: `.sl-top`, `.sl-prow` (GutguardShop.jsx:465); `.slw-top`, `.slw-t` (GutguardShop.jsx:464)
- Found in: s-top, s-card

## Accessibility

Basket button is labelled "Basket" or "Basket, N items". Product art should be `aria-hidden`. The basket glyph is Lucide `ShoppingBasket` (the original is a custom SVG).
