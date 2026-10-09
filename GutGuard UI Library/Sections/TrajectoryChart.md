---
title: TrajectoryChart
tags: [gutguard, ui-library, section]
group: Sections
status: draft
code: gutguard-ui/components/sections/TrajectoryChart.tsx
example: gutguard-ui/showcase/examples/TrajectoryChart.tsx
parts: [w-traj]
updated: 2026-10-08
---

# TrajectoryChart

MiAge across the scans: the overall change ("− 6"), first → last values, a line chart with a dashed calendar-age line, and day labels. Data-driven, drawn as inline SVG. Made for the dark slate band.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | One look | `.traj .traj-top .traj-delta .td-main .td-flow .traj-plot .traj-svg .traj-cal .traj-pt .traj-x .traj-ex .traj-note` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `title` | ReactNode | — | Serif italic |
| `hint` | ReactNode | — | "↓ lower is better" |
| `points` | `{ label, sub?, value }[]` | — | `sub` = small blue caption under the day |
| `calendarAge` | number | — | Draws the dashed line and its label; included in the y range |
| `calendarLabel` | string | `"Calendar age"` | |
| `deltaLabel` | ReactNode | — | Mono caption beside the change |
| `deltaNote` | ReactNode | — | Line under "48 → 42" |
| `lowerIsBetter` | boolean | `true` | The change shows light blue when it moves the good way, heat otherwise |
| `example` | ReactNode | — | Italic disclaimer |
| `note` | ReactNode | — | Closing paragraph; `<b>` turns bone |
| `className` | string | — | |

The change and the first/last values are computed from `points`. Points run 5–95% across; values fill 17–77% of the plot height. Point colours fade heat → recovery along the line; the last point is filled and larger.

## States

None. (The original draws the line in on scroll; this one is static.)

## Responsive

Same layout on all widths; plot height is fluid (172–216px) and the change row wraps.

## Source

- Original: `.traj` in components/GutguardSite.jsx:426
- Found in: w-traj

## Accessibility

The SVG and dots are decorative (`aria-hidden`); the values are real text in the DOM.
