---
title: Rank Ladder
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.ladder, .rung, .ant, .lock)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Rank Ladder

Horizontal, scrollable rank chips for selecting progression level.

## Anatomy

- Track: `.ladder` — flex row, gap 8px, overflow-x auto
- Chip: `.rung` — padding ~10×15, radius 12px, border
- Label: display sans uppercase (Academy: Anton `.ant`)
- Lock meta: small mute text when locked
- Active: `.rung.on` — filled (boss: navy; GG: ink or blue)

## States

`default` · `on` · `locked`

## Desktop twin

Sidebar rank rows (`.side-rank`) should share selection state with the ladder — same data, two presentations.

## Responsive

See [[Foundations/Breakpoints]].

Horizontal scroll on narrow viewports; snap chips. Desktop may show more chips without scroll if space allows ([[Components/Rank Ladder]] desktop twin).

## Finalize
- [ ] Map display type to Fraunces or keep a condensed UI chip style in Inter Tight
- [ ] Mark **Final** or system-only if unused outside Academy
