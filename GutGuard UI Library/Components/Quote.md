---
title: Quote
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/Quote.tsx
example: gutguard-ui/showcase/examples/Quote.tsx
parts: [w-review]
updated: 2026-10-08
---

# Quote

A member's words on a dark card with the heat-gold-recovery seam on top, then avatar, name and place. Use for testimonials only, with a real consented quote.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | Testimonial | `figure.review` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `children` | ReactNode | — | The quote, with its own curly quotes |
| `name` | ReactNode | — | "[Name], 23" |
| `role` | ReactNode | — | Mono line under the name: city, membership |
| `initials` | string | `"—"` | Gold `Avatar`, 44px |

## States

None.

## Responsive

Padding (26→34px) and quote size (19→24px) scale with the viewport via `clamp()`, as in the original. Max width 62ch.

## Source

- Original: `figure.review`, `.review-q`, `.review-who`, `.review-av`, `.review-nm`, `.review-role` in components/GutguardSite.jsx:612
- Found in: w-review

## Accessibility

`figure` > `blockquote` + `figcaption`. Avatar is `aria-hidden`.
