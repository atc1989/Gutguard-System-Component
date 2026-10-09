---
title: Note
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/Note.tsx
example: gutguard-ui/showcase/examples/Note.tsx
parts: [s-card, s-co, s-basket]
updated: 2026-10-08
---

# Note

A small inline info line with an icon. Use for a hint under a choice, payment fine print or the delivery estimate. Not for errors or alerts that need attention.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `info` | Grey text, blue icon: "Your 5 nights start the day your pack arrives…" | `.sl-note` |
| `fine` | Grey fine print, icon top-aligned: "You pay on Maya's secure page…" | `.co-cardnote` |
| `delivery` | Blue semibold: "Arrives in 2–6 working days…" | `.sl-eta` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | `info` \| `fine` \| `delivery` | `info` | |
| `icon` | LucideIcon | — | Required (13px; 12px for delivery) |
| `children` | ReactNode | — | The text |

## States

None (static).

## Responsive

Same on all widths.

## Source

- Original: `.sl-note` (GutguardShop.jsx:464), `.co-cardnote`, `.sl-eta` (GutguardShop.jsx:488)
- Found in: s-card, s-co, s-basket

## Accessibility

Rendered as a `<p>`; the icon is `aria-hidden`.
