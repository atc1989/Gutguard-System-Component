---
title: Modal
tags: [gutguard, design-system, components]
updated: 2026-08-12
status: draft
sources:
  - GutGuard-Doctors-HTML/components/ConfirmRegistrationModal.tsx
  - GutGuard-Doctors-HTML/app/admin/*/page.tsx
  - GutGuard-Doctors-HTML/components/Shoplet.tsx
---

# Modal

Focused overlay. Surface treatment only in DS; positioning follows implementation.

> [!important] Structured chrome
> For overlays with a **title, close icon, body, and footer actions**, prefer [[Components/Dialog]]. This note covers backdrop / shell variants (booth, admin, shop, Academy sheet).

## Anatomy

- Backdrop: `rgba(15,15,24,.58)`; optional blur 3px
- Surface: paper/bone, 1px rule
- Radius: **24px** commerce; **0** editorial/admin
- Shadow: `0 24px 70–80px rgba(15,15,24,.22–.28)`
- Header: bottom rule; Fraunces heading 28–38px
- Close: secondary control, ≥44px target
- Actions: [[Components/Button]] pair (primary + secondary)

## Variants in Doctors

| Variant | Classes |
|---|---|
| Booth confirm | `.modal-shell`, `.modal-backdrop`, `.confirm-modal` |
| Admin | `.admin-modal-backdrop`, `.admin-modal`, head/body/actions |
| Shop info | `.shop-modal-wrap`, `.shop-modal` |

## Academy sheet (from Gentrep)

| Variant | Classes | Notes |
|---|---|---|
| Bottom sheet / dialog | `.modal` + `.sheet` + `.grab` + `.sheet-head` | Mobile: align flex-end, top radius 20px; ≥900px: centered, full radius, max-width 560px |

Treat Academy `.sheet` as a Modal presentation (or shared with [[Components/Drawer]] bottom-sheet mode).

## A11y

Trap focus, restore on close, Escape to dismiss, mark page inert, label dialog.

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` | Prefer **bottom sheet** presentation when from Academy/mobile patterns (top radius ~20px, align flex-end); or full-width centered with side margins ≥16px |
| `≥ 900px` | Centered overlay; max-width ~560px; full radius per dialect (commerce 24px / admin 0) |

Structured title/close/footer chrome → [[Components/Dialog]].

## Finalize

- [ ] One modal shell API across booth/admin/shop
- [ ] Mark **Final**
