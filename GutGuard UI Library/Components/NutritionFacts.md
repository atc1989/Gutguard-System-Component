---
title: NutritionFacts
tags: [gutguard, ui-library, component]
group: Patterns
status: draft
code: gutguard-ui/components/patterns/NutritionFacts.tsx
example: gutguard-ui/showcase/examples/NutritionFacts.tsx
parts: [s-facts, s-inside]
updated: 2026-10-08
---

# NutritionFacts

The Supplement Facts label panel, filled from data. Use it in the "What's inside" sheet or on a product page.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| default | Label panel: title, serving, actives, macros, footnote | `.fx` (`.fx-h`, `.fx-serv`, `.fx-rule`, `.fx-col`, `.fx-row`, `.fx-macros`, `.fx-foot`) |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `title` | ReactNode | "Supplement Facts" | |
| `serving` | ReactNode | — | Bold mono after "Serving size" |
| `rows` | `{ name, amount, mark? }[]` | — | `mark` is the footnote sign, e.g. `**` |
| `macros` | ReactNode | — | Mono line under the second rule |
| `footnote` | ReactNode | — | Italic fine print |

## States

None (static).

## Responsive

Same on all widths; it fills its container.

## Source

- Original: `.fx` and children (GutguardShop.jsx:309)
- Found in: s-facts, s-inside

## Accessibility

A `<section>` with an `<h3>` title; the actives are a `<dl>`. Rules are `aria-hidden`.
