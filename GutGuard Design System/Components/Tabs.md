---
title: Tabs
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/app/admin/wheel/page.tsx (.admin-tabs)
  - GutGuard-Doctors-HTML/app/admin/tiktok/page.tsx (.admin-tiktok-tabs)
  - GutGuard-Doctors-HTML/components/GutguardSite.jsx (.sectabs / .sectab)
---

# Tabs

Horizontal section switcher. Doctors admin uses this as **top chrome** (no sidebar).

## Variants

### 1. Admin tabs

- Classes: `.admin-tabs button` (+ `.active`); TikTok twin `.admin-tiktok-tabs`
- Track: transparent with rule-bottom
- Tab min-height ~42px; padding ~12px 18px
- Type: 11px / 800 / uppercase / `.16em`
- Inactive: ink-3, transparent 2px bottom border
- Hover + active: **blue fill**, bone text, blue bottom border
- Square corners

### 2. Marketing section tabs

- Classes: `.sectabs`, `.sectab` (+ `.on`)
- Used for in-page section jumping on the marketing site
- May use mono eyebrow styling (IBM Plex Mono in GutguardSite)
- Soften geometry only within marketing dialect

## Behavior

- One selected tab; expose `aria-current` or `aria-selected`
- Keyboard: arrow keys when used as a tablist
- Do not use tabs for primary app IA if a future system adds a sidebar — keep tabs for peer panels

## Do / don’t

- Do reuse one Admin Tabs skin across wheel / tiktok / orders
- Don’t invent a third admin tab class per page

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| < 900px | Horizontal scroll if tabs overflow; do not wrap into multiple rows |
| ≥ 900px | Full tab row in admin/marketing shell |

Active tab stays fully visible (scroll into view on change).

## Finalize
- [ ] Merge `.admin-tabs` and `.admin-tiktok-tabs` into one class name in code
- [ ] Decide whether marketing sectabs stay a Tabs variant or become “Section jump”
- [ ] Mark **Final**
