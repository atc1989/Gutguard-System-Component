---
title: DoseRow
tags: [gutguard, ui-library, component]
group: Patterns
status: draft
code: gutguard-ui/components/patterns/DoseRow.tsx
example: gutguard-ui/showcase/examples/DoseRow.tsx
parts: [l-dose-next, l-dose-done, l-settings]
updated: 2026-10-08
---

# DoseRow

One dose (Reveille, Midday, Taps) as a row. In the day list it shows time, capsules, note, a camera button and Done or Undo. In Settings it shows a capsule Stepper and a reminder time input. Use it only for doses; for generic rows use ListRow.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `next` | The next dose: blue border, NEXT tag, filled Done | `.lw-dose.next`, `.lw-done` |
| `upcoming` | Later today: outline Done | `.lw-dose`, `.lw-done.soft` |
| `done` | Taken: pale blue, check icon, Undo | `.lw-dose.done`, `.lw-undo` |
| `settings` | Settings sheet: Stepper + time; 0 capsules = off (faded, no time) | `.lw-set`, `.lw-set.off`, `.lw-time` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `state` | `next` \| `upcoming` \| `done` \| `settings` | — | |
| `icon` | ReactNode | — | Lucide icon (Sun, Utensils, Moon); a check replaces it when done |
| `title` | string | — | |
| `time` | string | — | Day list: "7:00 AM". Settings: input value "07:00" |
| `capsules` | number | — | |
| `note` | string | — | "before meals · empty stomach" |
| `onDone` / `onUndo` / `onPhoto` | () => void | — | |
| `onCapsulesChange` | (n: number) => void | — | Settings: makes `capsules` controlled |
| `onTimeChange` | (time: string) => void | — | Settings: makes `time` controlled |
| `className` | string | — | |

## States

next / upcoming / done / settings / settings off (0 capsules). Done button presses to 97%. Focus-visible ring on all buttons and the time input.

## Responsive

Same on all widths. The original's ≤380px tightening (smaller gaps and icons) is not carried over.

## Source

- Original: `.lw-dose .ic .tag .meta .nt .lw-cam .lw-done .lw-undo .lw-set .lw-time` in components/prototype/LifestyleMember.jsx:1102
- Found in: l-dose-next, l-dose-done, l-settings

## Accessibility

Camera button is labelled "Take a photo of your <title> dose". Done reads "Done, <title>", Undo reads "Undo <title>". The Stepper is a labelled group ("<title> capsules"); the time input is labelled "<title> reminder time". The icon circle is decorative.
