---
title: AdherenceCalendar
tags: [gutguard, ui-library, component]
group: Patterns
status: draft
code: gutguard-ui/components/patterns/AdherenceCalendar.tsx
example: gutguard-ui/showcase/examples/AdherenceCalendar.tsx
parts: [l-story]
updated: 2026-10-08
---

# AdherenceCalendar

Month grid on My Story: one cell per day with a dot for how many doses were taken, a camera mark when a photo was logged, a ring on today, and a legend. Use it for dose history only.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | My Story month | `.lw-cal .wd .c .fu .td .dt .half .full .ph`, `.lw-legend` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `monthLabel` | string | — | "October 2026", shown as the heading |
| `offset` | number | — | Empty cells before day 1 (0 = Sunday) |
| `days` | `{ day, status, photo?, today? }[]` | — | status: `none` \| `half` \| `full` \| `miss` \| `future` |
| `onSelect` | (day: number) => void | — | Called when a day is tapped |
| `className` | string | — | |

## States

Day: none (no dot) / half (split dot) / full (blue dot) / miss (peach dot) / future (faded number) / today (2px blue inner ring, bold) / photo (camera mark). Focus-visible ring on each day.

## Responsive

Same on all widths; cells are square and fill the container's width.

## Source

- Original: `.lw-cal`, `.lw-legend` in components/prototype/LifestyleMember.jsx:998
- Found in: l-story

## Accessibility

Each day is a `<button>` labelled "Day 3: all doses, with photo"; today has `aria-current="date"`. Weekday letters and dots are decorative. Legend copy is fixed English for now.
