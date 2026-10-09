---
title: Lang Toggle
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.langs, .lang)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Lang Toggle

Compact language switcher (e.g. EN | Tagalog) inside document sheets.

## Spec

- Track: paper fill, 1px rule, radius 12px, padding 4px, gap 6px
- Segment: min touch 44px; `.lang.on` = selected
- Essentially a small [[Components/Segmented Control]]

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint — compact segmented control. Keep in masthead/toolbar without wrapping under 320px if possible.

## Finalize
- [ ] Merge into Segmented Control as `size: sm` variant, or keep named alias
- [ ] Mark status
