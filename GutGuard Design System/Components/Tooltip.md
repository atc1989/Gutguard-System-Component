---
title: Tooltip
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Tooltip

Short helper on hover/focus. Not for essential instructions (use field helper text).

## Spec

- Ink fill, bone text, 12–13px / 600
- Padding ~8px 10px; radius 8px commerce / 0 editorial
- Soft shadow; max-width ~220px
- Arrow optional
- Appear on focus-visible as well as hover
- Delay ~300ms; dismiss on Escape
- Never trap focus inside a tooltip

## Responsive

See [[Foundations/Breakpoints]].

Prefer tooltips on hover/focus for desktop. On touch (< 900px or coarse pointer), use tap-to-toggle or move copy into visible helper text — do not rely on hover-only.

## Finalize
- [ ] Prefer Popover for interactive content — keep Tooltip text-only
- [ ] Mark **Final**
