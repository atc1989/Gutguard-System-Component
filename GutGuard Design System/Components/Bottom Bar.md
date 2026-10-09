---
title: Bottom Bar
aliases:
  - Sticky Next Bar
  - Foot Bar
tags: [gutguard, design-system, components, shell]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.foot, .foot-in, .foot-title, .eyebrow-dark)
---

# Bottom Bar

Fixed mobile chrome for a primary next / order action. From prototypes [[Systems/Gentrep-Academy-Dashboard]] and [[Systems/GutGuard-Lifestyle]] — **skin with Doctors / GG**, not prototype colors.

## Behavior

- `position: fixed`; bottom 0; full width; `z-index: 40`
- Paper/bone surface; 1px top rule; soft upward shadow optional
- Inner max-width ~440px
- Safe-area padding
- **Hidden on desktop** when [[Components/Sidebar]] is shown

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` | **Visible** (when the product uses a sticky primary CTA) |
| `≥ 900px` | **Hidden** if Sidebar carries the same CTA / next action |

Reserve bottom safe-area (`env(safe-area-inset-bottom)`). Toasts sit above the bar (~96px from bottom on Academy).

## Anatomy

```
optional eyebrow
title / CTA label                 [ Button ]
```

Uses [[Components/Button]] commerce primary.

## Seen in

| System | Class | CTA |
|---|---|---|
| Academy | `.foot` | Do this next |
| Lifestyle | `.gg-foot` | Order now |

## vs Top Bar / tabs

- [[Components/Top Bar]] = navigation
- **Bottom Bar** = single persistent CTA
- Do **not** turn this into a multi-tab bar — Lifestyle tabs are [[Components/Segmented Control]]

## Finalize

- [ ] Remap to bone/paper + ink/blue
- [ ] Confirm toast sits above bar (Academy toast `bottom: 96px`)
- [ ] Mark **Final**
