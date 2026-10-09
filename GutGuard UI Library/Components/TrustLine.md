---
title: TrustLine
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/TrustLine.tsx
example: gutguard-ui/showcase/examples/TrustLine.tsx
parts: [s-trustline, s-basket]
updated: 2026-10-08
---

# TrustLine

A centred, wrapping row of small icon + text reassurances under a choice or a pay button. For a single explanatory line use [[Note]].

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `choice` | 11px, under the pack choice: Secure · FDA-registered · Free shipping | `.sl-trustline` |
| `checkout` | 12px, under basket / pay buttons, with an optional link | `.sl-trust2` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | `choice` \| `checkout` | `choice` | |
| `items` | `{ icon: LucideIcon; label }[]` | — | Icons render 12px in recovery blue |
| `link` | `{ href, label }` | — | Trailing underlined blue link, e.g. Refund policy |

## States

Link: default underline; focus-visible gold ring.

## Responsive

Same on all widths; items wrap.

## Source

- Original: `.sl-trustline` (GutguardShop.jsx:392), `.sl-trust2` (GutguardShop.jsx:488)
- Found in: s-trustline, s-basket, s-co, s-card

## Accessibility

Icons are `aria-hidden`; the text carries the meaning. The link is a real `<a>`.
