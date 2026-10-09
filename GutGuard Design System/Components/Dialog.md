---
title: Dialog
tags: [gutguard, design-system, components]
updated: 2026-08-13
status: draft
---

# Dialog

Structured overlay chrome: **header · body · footer**. Prefer this for confirm/detail flows that need a title, dismiss control, and explicit actions.

Overlay surface rules (backdrop, shadow, radius dialects) live on [[Components/Modal]]. Dialog is the **inner structure** that sits on that overlay.

## Anatomy

| Region | Content |
|---|---|
| **Header** | Fraunces title (`id` for `aria-labelledby`) + trailing [[Components/Icon Button]] close (`X` SVG, `aria-label="Close"`). Bottom 1px rule. |
| **Body** | Scrollable content; ink-2; 14–16px type; padding 16–24px |
| **Footer** | Right-aligned [[Components/Button]] pair — secondary **Cancel** + primary **Confirm**. Top 1px rule. Gap 10px. |

## Geometry

- Max width ~480–560px (product choice)
- Radius: **24px** commerce/partner · **0** editorial/admin
- Shadow: `0 24px 70–80px rgba(15,15,24,.22–.28)`
- Paper/bone fill; 1px rule border
- Close control: ≥44px hit target (36px dense admin OK)

## Header / footer defaults

**Header**
- Title: Fraunces 28–32px / 400; ink
- Close: Icon Button with Lucide-style `x` (24px viewBox, 2px stroke, `currentColor`)

**Footer**
- Cancel → secondary / ghost button
- Confirm → primary matching dialect (partner blue rounded · admin square ink/blue)
- Destructive confirms may use error-tinted primary — keep copy explicit

## Variants

| Variant | Notes |
|---|---|
| Commerce dialog | 24px radius; partner primary in footer |
| Admin dialog | Square; denser header; admin primary |
| Editorial dialog | Square; booth primary if used in registration |

## A11y

- `role="dialog"` + `aria-modal="true"`
- `aria-labelledby` → header title id
- Focus trap while open; restore focus on close
- Escape dismisses (unless destructive critical — product choice)
- Backdrop click dismiss optional; document per product

## Do / don’t

- **Do** use Icon Button + SVG for close — never text `✕` / `×`
- **Do** keep actions in the footer, not only in the body
- **Don’t** mix Dialog chrome with Drawer side-sheet layout (see [[Components/Drawer]])
- **Don’t** invent a second overlay language — share Modal backdrop tokens

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` | Width `min(100% - 32px, 520px)` or bottom-sheet style; body `max-height` ~50vh with scroll; footer buttons may stack full-width if two actions won’t fit |
| `≥ 900px` | Centered; max-width ~480–560px; footer actions in a row |

Close control stays ≥44px on mobile.

## Portable CSS

`.gg-dialog` · `.gg-dialog-header` · `.gg-dialog-body` · `.gg-dialog-footer` — see [[03 - Portable CSS Starter]]

## Showcase

`Showcase/index.html` → `#dialog`

## Finalize

- [ ] Align Doctors confirm modals to this anatomy
- [ ] Mark **Final**
