---
title: TextField
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/TextField.tsx
example: gutguard-ui/showcase/examples/TextField.tsx
parts: [s-mobile, s-field, s-co, g-signup, g-login]
updated: 2026-10-08
---

# TextField

Label, input and one help or error line, for any input type (text, tel, email, time…). `FieldRow` puts two fields side by side. For the 6-digit SMS code use CodeInput; for a suggestion list use Combobox (built on this).

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `shop` | Checkout: grey 12px label, mono 11px help | `.co-f`, `.fe`, `.co-f.err` |
| `lifestyle` | Sign-up / log-in: ink semibold 12.5px label, sans 11.5px help | Lifestyle `label.osw` + inline input |
| `FieldRow` | First + last name | `.co-two` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `label` | ReactNode | — | Can hold a muted " · optional" span |
| `help` | ReactNode | — | Grey line under the input |
| `error` | ReactNode | — | Replaces help, heat border + text |
| `variant` | `shop` \| `lifestyle` | `shop` | |
| `children` | ReactNode | — | Rendered under the field (Combobox list) |
| `className` | string | — | On the wrapper |
| …input props | | | `type`, `value`, `defaultValue`, `onChange`, `autoComplete`, `id`… |

## States

default / focus (blue border + faint blue ring, plus global focus ring) / error (heat-text border and text)

## Responsive

Same on all widths. FieldRow stays two-up on phones, as in the original.

## Source

- Original: `.co-f`, `.co-two`, `.fe` in GutguardShop.jsx:436, :488, :586; Lifestyle label + input in LifestyleLanding.jsx:751
- Found in: s-mobile, s-field, s-co, g-signup, g-login

## Accessibility

Real `<label for>`. Help/error linked with `aria-describedby`; error sets `aria-invalid`. Id is generated when none is passed. `.co-inline` was dropped (it only ever wraps the input). Lifestyle has no captured error state; it reuses the shop's. `.lw-time` (pill time input in settings) is not covered.
