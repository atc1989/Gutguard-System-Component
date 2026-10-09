---
title: ChoiceChip
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/ChoiceChip.tsx
example: gutguard-ui/showcase/examples/ChoiceChip.tsx
parts: [s-chips, s-sub]
updated: 2026-10-08
---

# ChoiceChip

A centred chip for picking one of three packs (Start / Grow / Peak) or goals (Keep healthy / Feel better / Full recovery). Use `ChoiceChips` as the three-up row. For cards with a price on the side use [[OptionCard]].

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| default | Pack chips: name, saving, duration | `.sl-chip` (`.cn`, `.cpc.sv`, `.cd`) |
| `best` | Saving shown as a filled blue pill | `.cpc.svp` |
| `long` | Two-word names at 15px | `.cn.sm` |
| `tag` | Top-edge tag: "Popular", "Best rate" (blue when selected) | `.ctag` (uses `Badge tone="solid"`) |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `name` | ReactNode | — | Required |
| `detail` | ReactNode | — | Mono blue line: "Save 11%", "2 a day" |
| `duration` | ReactNode | — | Mono grey line: "15-day", "6 blisters" |
| `tag` | ReactNode | — | |
| `best` | boolean | — | |
| `long` | boolean | — | |
| `selected` | boolean | — | Controlled |
| `onSelect` | () => void | — | |
| `ChoiceChips.label` | string | — | Accessible name of the radiogroup |

## States

- default: rule border, paper
- selected: blue border, faint blue wash, soft blue shadow, check mark top-right, tag turns blue
- focus-visible: global gold ring

## Responsive

Same on all widths (always three columns, gap 8px).

## Source

- Original: `.sl-chips`, `.sl-chip`, `.ctag`, `.cmk`, `.cn`, `.cpc`, `.svp`, `.cd` (GutguardShop.jsx:355)
- Found in: s-chips, s-sub

## Accessibility

`<button role="radio" aria-checked>` inside `ChoiceChips` (`role="radiogroup"` + `aria-label`). The check mark is `aria-hidden`. Each chip is its own tab stop.
