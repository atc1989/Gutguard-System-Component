---
title: IconRow
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/IconRow.tsx
example: gutguard-ui/showcase/examples/IconRow.tsx
parts: [g-get, l-guard, s-inside]
updated: 2026-10-08
---

# IconRow

Icon + title + a line of text. Not interactive. Stack several for a benefit or ingredient list; use `ListRow` when the row is tappable.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `benefit` (default) | "What you get" lists, divider below each row | Lifestyle landing benefit rows |
| `heading` | Panel heading with an icon: "Guard someone" | Lifestyle Guard someone header |
| `list` | Check rows in a sheet, divider above each row | `.sl-line` in "What's inside" |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | see above | `benefit` | |
| `icon` | ReactNode | — | Lucide icon; the row sizes it (19px in a 38px circle, 16px bare in `list`) |
| `title` | ReactNode | — | |
| `children` | ReactNode | — | Grey text |
| `className` | string | — | |

## States

None.

## Responsive

Same on all widths.

## Source

- Original: Lifestyle inline rows in components/prototype/LifestyleLanding.jsx:632 and LifestyleMember.jsx:586; `.sl-line` in components/GutguardShop.jsx:488
- Found in: g-get, l-guard, s-inside

## Accessibility

Icons are `aria-hidden`; the title carries the meaning.
