---
title: OptionCard
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/OptionCard.tsx
example: gutguard-ui/showcase/examples/OptionCard.tsx
parts: [s-watch, s-trials, s-pays]
updated: 2026-10-08
---

# OptionCard

A selectable card for choosing a trial pack or a payment method. Put them in an `OptionGroup` (two-column radiogroup); a `wide` card spans both columns. For three-up pack/goal choices use [[ChoiceChip]] instead.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `compact` | Name, caption, price stacked: Blister / Bottle | `.sl-topt` in `.sl-topts` |
| `wide` | Full row, price + tag on the right: 5-Night Watch | `.sl-topt.sl-wide-opt` (`.wr`, `.tfree`) |
| `radio` | Radio dot, bold title, small text: Maya | `.co-pay` (`.rd`) in `.co-pays` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | `compact` \| `wide` \| `radio` | `compact` | |
| `title` | ReactNode | — | Required |
| `caption` | ReactNode | — | Mono line (compact/wide), small text (radio). Can hold a `Save 15%` span |
| `price` | ReactNode | — | Rendered with `Price size="sm"` (compact/wide) |
| `tag` | ReactNode | — | Wide only: line under the price, e.g. "Free shipping" (`Badge tone="text"`) |
| `selected` | boolean | — | Controlled |
| `onSelect` | () => void | — | |
| `OptionGroup.label` | string | — | Accessible name of the radiogroup |

## States

- default: 1.5px rule border on paper
- selected: ink border (compact/wide); blue border + 1px blue ring + filled dot (radio)
- focus-visible: global gold ring

## Responsive

Same on all widths. Below 400px the wide card's tag drops to 10px.

## Source

- Original: `.sl-topt`, `.sl-wide-opt`, `.sl-topts` (GutguardShop.jsx:338, :343); `.co-pay`, `.co-pays` (GutguardShop.jsx:654)
- Found in: s-watch, s-trials, s-pays, s-card

## Accessibility

Each card is a `<button role="radio" aria-checked>` inside `OptionGroup` (`role="radiogroup"` + `aria-label`). Each card is its own tab stop (no arrow-key roving).
