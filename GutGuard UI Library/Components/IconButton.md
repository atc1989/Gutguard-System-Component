---
title: IconButton
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/IconButton.tsx
example: gutguard-ui/showcase/examples/IconButton.tsx
parts: [w-nav, s-top, l-nav, l-dose-next]
updated: 2026-10-08
---

# IconButton

A control that shows only an icon: back, menu, close, basket, Lifestyle shop / settings / camera. Use a [[Button]] when there is room for a word.

## Variants

| Shape | Use for | Replaces |
|---|---|---|
| `square` | Back button in the top bar (38px, 44px on touch) | `.nav-back` |
| `menu` | Menu and close buttons (44px) | `.burger`, `.sheet-close` |
| `round` | Basket, Lifestyle icons, camera (42px circle; resize with `className`) | `.sl-cart`, `.lw-icon`, `.lw-cam` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `label` | string | — | Required. Becomes `aria-label` |
| `shape` | `square` \| `menu` \| `round` | `round` | |
| `count` | number | — | Blue bubble (basket). Hidden at 0 |
| `href` | string | — | Renders `<a>` |
| `children` | ReactNode | — | The Lucide icon |

## States

Hover: blue border (square also gets a bone fill). Focus-visible: gold ring.

## Responsive

`square` grows to 44px on touch screens (`pointer: coarse`), as in the original.

## Source

- Original: `.nav-back`, `.burger`, `.sl-cart` (+ `.n`) in GutguardSite.css; `.lw-icon`, `.lw-cam` in LifestyleMember.jsx
- Found in: w-nav, s-top, l-nav, l-dose-next

## Accessibility

`label` is required. With `count`, the name reads "Basket, 2 items".
