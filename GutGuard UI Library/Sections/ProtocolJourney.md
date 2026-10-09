---
title: ProtocolJourney
tags: [gutguard, ui-library, section]
group: Sections
status: draft
code: gutguard-ui/components/sections/ProtocolJourney.tsx
example: gutguard-ui/showcase/examples/ProtocolJourney.tsx
parts: [l-story]
updated: 2026-10-08
---

# ProtocolJourney

The top card of My Story: "Your 90-Day Protocol", the "Gut Guardian since…" chip, the heat/recovery capsule art, a big "Day 4 of 90", the journey ProgressBar split into phases, the phase chips (current one gold) and a note line (next BioScan). Use it once at the top of My Story.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | My Story protocol card | first inline-styled `div` in `.col-l` (with `.lw-id.gg`, `.ant`) |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `title` | string | — | "Your 90-Day Protocol" |
| `since` | string | — | "Gut Guardian since 26 Sep 2026" |
| `day` | number | — | Current day |
| `total` | number | — | 90 |
| `phases` | `{ name, weeks }[]` | — | Equal parts of the bar; the current phase comes from `day` |
| `note` | ReactNode | — | Bottom line; `<b>` turns ink |
| `className` | string | — | |

## States

Current phase chip: gold-pale with a gold-soft border, `aria-current="step"`. Others bone, ink-3.

## Responsive

Same on all widths (fills its column).

## Source

- Original: inline styles in components/prototype/LifestyleMember.jsx:998 (l-story, `.col-l` first div)
- Found in: l-story
- Capsule gradients #FF8A6B→#E24A22 and #4FA3DE→#1E6FB8 mapped to heat→heat-brick and recovery→recovery-deep.

## Accessibility

The bar is a `progressbar` ("Day 4 of 90"). The capsule art is `aria-hidden`.
