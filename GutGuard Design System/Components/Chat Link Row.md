---
title: Chat Link Row
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.chat, .tg)
---

# Chat Link Row

CTA row to open an external chat (e.g. Telegram community).

## Spec

- Paper card, 1px rule, 14px radius
- Leading brand tile 42×42 (channel color allowed as **local** accent — e.g. Telegram teal)
- Title: Inter Tight 600; sub: ink-3
- Whole row clickable; min height ~64px
- Hover: blue border or slight shadow
- Trailing chevron or “Open” text button

## Note

Channel brand color is an exception tile only — do not recolor the whole DS.

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** row. Title/meta truncate with ellipsis; trailing action stays visible.

## Finalize
- [ ] Mark **Final** if reused beyond Academy
