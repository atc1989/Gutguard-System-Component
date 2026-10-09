---
title: Rank Plate
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.plate, .plate-*, .hatch, .pips, .pip, .bar)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Rank Plate

Hero progress card for the active rank. Brand-forward.

## Anatomy

- Dark brand gradient surface, radius ~18px, white type
- Optional hatch texture + watermark mark
- Eyebrow rule row (gold tick + uppercase label)
- Large uppercase title
- Subline + footer (status text + diamond **pips**)
- Progress **bar** (gold fill on translucent track)
- Note line under bar

## States

| State | Treatment |
|---|---|
| In progress | Brand blue gradient |
| Done | Green gradient (`#1a7a49` → `#0f5a35` in boss) |
| Pip done / booked / missed | gold / soft gold / clay |

## GG remap notes

- Prefer ultramarine gradient over boss `#1f5d99`
- Use muted gold carefully for pips — may need a brighter semantic “progress” token
- Done state → DS success green (extend foundations if missing)

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** hero plate in the main column (mobile max ~440px pattern). Stack metrics on very narrow widths.

## Finalize
- [ ] Decide core kit vs Academy-only
- [ ] Mark status
