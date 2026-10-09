---
title: Checkbox
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/Checkbox.tsx
example: gutguard-ui/showcase/examples/Checkbox.tsx
parts: [g-signup]
updated: 2026-10-08
---

# Checkbox

Native checkbox with a line of text that can hold links, e.g. the sign-up consent. For one-of-many choices use SegmentedControl.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| default | Consent line | Lifestyle `label.inr > input[type=checkbox]` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `children` | ReactNode | — | The text; may contain links |
| `className` | string | — | On the label |
| …input props | | | `checked`, `defaultChecked`, `onChange`, `name`, `required`… |

## States

unchecked / checked (blue accent) / focus-visible / disabled (native)

## Responsive

Same on all widths.

## Source

- Original: inline-styled label + checkbox in LifestyleLanding.jsx:751
- Found in: g-signup

## Accessibility

Native `<input type="checkbox">` inside its `<label>`, so the whole line toggles it and links inside still work.
