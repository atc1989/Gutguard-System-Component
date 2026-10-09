---
title: CodeInput
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/CodeInput.tsx
example: gutguard-ui/showcase/examples/CodeInput.tsx
parts: [g-code, g-login]
updated: 2026-10-08
---

# CodeInput

One wide input for the SMS code, with big spaced digits and a "• • • • • •" placeholder. Matches the capture (one input, not six boxes). The "Send again" link and the heading belong to the caller.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| default | 6-digit code | inline-styled code input in LifestyleLanding.jsx |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `label` | string | — | Accessible name, e.g. "6-digit code" |
| `length` | number | 6 | Sets `maxLength`, `pattern` and the placeholder |
| `className` | string | — | |
| …input props | | | `value`, `defaultValue`, `onChange`, `name`… |

## States

empty (placeholder) / filled / focus (blue border + global ring)

## Responsive

Same on all widths.

## Source

- Original: inline-styled input in LifestyleLanding.jsx:751
- Found in: g-code, g-login

## Accessibility

`aria-label`, `inputMode="numeric"`, `autoComplete="one-time-code"` (phones offer the code from the SMS), `pattern` for validation.
