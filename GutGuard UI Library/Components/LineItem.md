---
title: LineItem
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/LineItem.tsx
example: gutguard-ui/showcase/examples/LineItem.tsx
parts: [s-basket, s-co, s-done]
updated: 2026-10-08
---

# LineItem

One row in the basket or the checkout order, or a numbered next step on the done screen. Rows carry their own top rule; pass `className="border-t-0"` on the first row under a heading. Not for icon + benefit rows (that is IconRow).

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `basket` | Thumb, name, mono details, Remove, price | `.sl-line` (`.lc`, `.ln`, `.ld`, `.sl-rm`, `.sl-lp`) |
| `step` | Gold "01" number, title, grey text | `.co-next .sl-line` (`.nx`, `.ld2`) |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | `basket` \| `step` | `basket` | |
| `name` | ReactNode | — | Required |
| `description` | ReactNode | — | Mono (basket) or 12.5px text (step) |
| `price` | ReactNode | — | Basket, required |
| `thumb` | ReactNode | capsule | Basket; defaults to the red/blue capsule on bone |
| `onRemove` | () => void | — | Basket; shows the Remove link |
| `removeLabel` | string | "Remove" | Accessible name, e.g. "Remove 5-Night Watch" |
| `step` | ReactNode | — | Step, required: "01" |

## States

Remove link: focus-visible gold ring. Rows are static.

## Responsive

Same on all widths.

## Source

- Original: `.sl-line`, `.sl-rm`, `.sl-lp`, `.co-next`, `.nx`, `.ld2` (GutguardShop.jsx:488)
- Found in: s-basket, s-co, s-done

## Accessibility

Remove is a real `<button>`; give it `removeLabel` so screen readers know which item it removes.
