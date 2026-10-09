---
title: Drawer
tags: [gutguard, design-system, components]
updated: 2026-08-12
status: draft
sources:
  - GutGuard-Doctors-HTML/components/Shoplet.tsx
  - GutGuard-Doctors-HTML/components/GutguardSite.jsx (.sheet, .cart-drawer)
---

# Drawer

Sliding panel for basket, checkout, or mobile nav. Commerce-first.

## Anatomy

- Classes: `.shop-drawer-wrap`, `.shop-drawer-scrim`, `.shop-drawer`, `.shop-drawer-head`
- Scrim/backdrop shared with modal family
- Surface: paper, rule on exposed edge
- Inward corners **24px** on commerce
- Desktop: side drawer shadow `-22px 0 70px rgba(15,15,24,.22)`
- ≤720px: treat as bottom sheet (Shoplet behavior)

## Related

- Marketing mobile `.sheet` = full-screen menu variant of drawer/sheet
- Use [[Components/Button]] for footer CTAs

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` (and often `< 720px` in Shoplet) | **Bottom sheet** or full-height sheet for nav/basket — grab handle optional; top radius ~20–24px commerce |
| `≥ 900px` | **Side drawer** (typically right); fixed width ~280–360px; scrim + edge shadow |

Do not show a side drawer and bottom sheet for the same surface at once.

## Finalize

- [ ] Lock 720 vs 900 cut for shop basket (document product override if kept at 720)
- [ ] Mark **Final**
