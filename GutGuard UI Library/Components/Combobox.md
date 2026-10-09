---
title: Combobox
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/Combobox.tsx
example: gutguard-ui/showcase/examples/Combobox.tsx
parts: [s-city]
updated: 2026-10-08
---

# Combobox

Text field that lists matching options as you type (bold name + small grey hint), like the checkout city search. Use when the list is too long for a select. Built on TextField, so it takes the same label/help/error/variant props.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| default | City or municipality search | `.co-city`, `.co-sugg[role=listbox]` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `options` | `{ value: string; label: string; hint?: string }[]` | — | Filtered by label, case-insensitive, first 8 shown |
| `value` | string | — | Typed text, controlled |
| `defaultValue` | string | "" | |
| `onChange` | (text: string) => void | — | Every keystroke and on pick |
| `onSelect` | (option) => void | — | Text becomes the option's label |
| …TextField props | | | `label`, `help`, `error`, `variant`, `placeholder`… |

## States

closed / open (list under the field) / active option (bone) / hover (bone)

## Responsive

Same on all widths.

## Source

- Original: `.co-city`, `.co-sugg` in GutguardShop.jsx:436
- Found in: s-city

## Accessibility

Input is `role="combobox"` with `aria-expanded`, `aria-controls`, `aria-autocomplete="list"` and `aria-activedescendant`. List is `role="listbox"` of `role="option"`. Arrow Up/Down move, Enter picks, Escape and blur close.
