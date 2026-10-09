---
title: SuccessState
tags: [gutguard, ui-library, component]
group: Overlays & states
status: draft
code: gutguard-ui/components/ui/SuccessState.tsx
example: gutguard-ui/showcase/examples/SuccessState.tsx
parts: [s-done]
updated: 2026-10-08
---

# SuccessState

Confirmation after a completed action: blue check circle, serif title, one line, any content, then actions. The shop puts a mini `MemberCard` and a `numbered` `Timeline` in the content slot.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | Payment confirmed, sign-up done | `.co-ok` (`.ic`) |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `title` | ReactNode | — | `h3`, "Payment confirmed." |
| `description` | ReactNode | — | `<b>` inside renders in ink |
| `children` | ReactNode | — | Mini card, next steps |
| `actions` | ReactNode | — | Stacked, centred: `Button size="lg"` + `Button variant="link"` |

## States

None.

## Responsive

Same on all widths; lives inside a sheet.

## Source

- Original: `.co-ok`, `.ic` in components/GutguardShop.jsx:488
- Found in: s-done

## Accessibility

Title is an `h3` inside the sheet dialog; the check icon is `aria-hidden`. Move focus to the title or first action when the state appears.
