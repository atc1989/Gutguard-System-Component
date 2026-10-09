---
title: Dialects
tags: [gutguard, design-system, foundations]
updated: 2026-08-12
---

# Dialects

One screen = one dialect. Shared colors and type hierarchy stay constant; radius and density change.

| Dialect | Character | Radius | Typical use |
|---|---|---:|---|
| Editorial (booth) | Magazine-like, ceremonial, high type contrast | Mostly `0` | Registration, verification, prize |
| Editorial (marketing) | Warm premium site, mono eyebrows, pill CTAs | Soft / pill | Marketing site nav + sections |
| Commerce / partner | Warm, friendly, softly premium | `10–24px` | Shop, checkout, partner, order status |
| Admin | Dense, functional, high clarity | Mostly `0` | Tables, management forms, tabs, alerts |

## Rules

1. Do not mix radius policies randomly on one screen.
2. Blue / bone / ink / gold tokens are shared across all dialects.
3. When a component has dialect variants, document them on that component note — not as separate unrelated components.
4. Marketing soft-pill buttons are a **variant of Button**, not a fourth brand.
