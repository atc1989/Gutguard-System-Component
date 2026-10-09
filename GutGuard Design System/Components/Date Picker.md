---
title: Date Picker
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - Academy Event Row booking
---

# Date Picker

Choose a calendar day (booking, scheduling).

## Spec

- Trigger: Form Field–styled control showing selected date
- Popover panel: paper, rule, commerce radius, card shadow
- Month nav: icon buttons 44×44
- Day grid: 40–44px cells; today = blue outline; selected = blue fill + bone text
- Disabled / past days: ink-4
- Keyboard navigable grid

## Related

- List booking UI may use [[Components/Event Row]] instead of a full calendar

## Responsive

See [[Foundations/Breakpoints]].

Calendar panel ~280px; on mobile open as centered popover or bottom sheet so month grid is fully tappable. Chevron icon buttons dense 36px OK.

## Finalize
- [ ] Prefer native `input type="date"` styled as field when enough
- [ ] Mark **Final** when custom picker ships
