---
title: Toast
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/styles/globals.css (.admin-toast)
---

# Toast

Floating, temporary feedback.

## Spec

- Ink background, bone body text, subtle blue-translucent border
- Square; padding ~16px; shadow `0 20px 48px rgba(15,15,24,.28)`
- Title: success lime `#EAFF18` or error pink `#FFB8C2`; 12px / 800 / uppercase / `.12em`
- Body: bone 14px / 700 / 1.35
- Dismiss: translucent bone border; prefer 44px target
- Announce via `aria-live`

## Notes

Lime/pink title colors are **toast-only** — do not use as general success/error fills.

## Responsive

See [[Foundations/Breakpoints]].

Fixed position; max-width ~340px. On mobile, inset ≥16px from edges and sit **above** [[Components/Bottom Bar]] when that bar is visible.

## Finalize
- [ ] Promote beyond admin-only usage
- [ ] Mark **Final**
