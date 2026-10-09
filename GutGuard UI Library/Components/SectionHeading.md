---
title: SectionHeading
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/SectionHeading.tsx
example: gutguard-ui/showcase/examples/SectionHeading.tsx
parts: [w-sechead]
updated: 2026-10-08
---

# SectionHeading

Opens a website section: a numbered mono label, a big serif `h2` with an italic blue accent, and an italic gold lead. One per section.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `light` (default) | Section opener on bone | `.sec-label` (`.num`), `h2.sec`, `.sec-sub` |
| `dark` | Section opener on a slate band (number recovery blue, accent gold) | `.measure .sec-label`, `.measure h2.sec`, `.measure .sec-sub` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `number` | string | — | "01", blue |
| `label` | ReactNode | — | "Why now" |
| `title` | ReactNode | — | Wrap the accent in `<em>` |
| `lead` | ReactNode | — | Italic gold paragraph |
| `id` | string | — | Anchor for in-page links |
| `tone` | `light` \| `dark` | `light` | `dark` on `bg-slate` bands |
| `className` | string | — | |

## States

None.

## Responsive

Heading 30→52px (`clamp(30px, 5vw, 52px)`), lead 17→20px, same as the original. Heading max 18ch, lead max 46ch.

## Source

- Original: `.sec-label`, `.num`, `h2.sec`, `.sec-sub` in components/GutguardSite.jsx:362
- Found in: w-sechead

## Accessibility

Real `h2`. The dash before the label is `aria-hidden`.
