---
title: Card
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/styles/globals.css
  - Shop / Partner / Admin panels
---

# Card

Raised or ruled content surface. Prefer rules over heavy shadows.

## Variants

| Variant | Treatment | Dialect |
|---|---|---|
| Editorial panel | Bone, 1px rule, square, little/no shadow | Editorial |
| Commerce card | Paper, 1px rule, 14px radius, soft card shadow | Commerce |
| Auth card | Paper ~94% opacity, rule, **3px blue top border**, 14px radius | Commerce |
| Order panel | `.shop-order-panel` + status modifiers (`paid` / `failed` / `cancelled`) | Commerce |
| Admin panel | `.admin-wheel-panel` + panel head | Admin |
| Dark ceremonial | Ink→blue gradient, bone text, gold-soft eyebrows | Editorial special |
| Stat / trust | Centered; Fraunces value; uppercase caption | Commerce / marketing |

## Rules

- Nested blocks use bone, not a second white card
- Selectable option cards: active = blue border + inset blue line → see choice patterns in Shop
- Cards are for grouping content; interactive choices should expose selected state in text/ARIA too

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid**. In grids: 1 column < 900px, 2+ columns from desktop unless the page defines otherwise. Padding may reduce slightly on narrow screens; radius follows dialect.

## Finalize
- [ ] Name status tones for order panel
- [ ] Mark **Final**
