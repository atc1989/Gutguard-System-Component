---
title: EmptyState
tags: [gutguard, ui-library, component]
group: Overlays & states
status: draft
code: gutguard-ui/components/ui/EmptyState.tsx
example: gutguard-ui/showcase/examples/EmptyState.tsx
parts: [s-basket, w-doors]
updated: 2026-10-08
---

# EmptyState

What to show when there is nothing yet: one centred line inside a sheet, or a dashed coming-soon box for a section that is not open.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `inline` (default) | "Your basket is empty." | `.sl-empty` |
| `soon` | Section not open yet | `.doors-soon` + `.soon-badge` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | see above | `inline` | |
| `badge` | ReactNode | — | `soon`: outline `Badge` text |
| `title` | ReactNode | — | `soon`: `h3` |
| `children` | ReactNode | — | The line of text |

## States

None.

## Responsive

Same on all widths.

## Source

- Original: `.sl-empty` in components/GutguardShop.jsx:488; `.doors-soon`, `.soon-badge` in components/GutguardSite.jsx:676
- Found in: s-basket, w-doors

## Accessibility

Plain text. If the empty line appears after a user action (removing the last item), announce it from the parent with `aria-live`.
