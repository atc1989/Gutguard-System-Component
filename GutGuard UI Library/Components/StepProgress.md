---
title: StepProgress
tags: [gutguard, ui-library, component]
group: Patterns
status: draft
code: gutguard-ui/components/patterns/StepProgress.tsx
example: gutguard-ui/showcase/examples/StepProgress.tsx
parts: [g-signup, g-code, g-first]
updated: 2026-10-08
---

# StepProgress

Segmented progress at the top of the Lifestyle sign-up: one 4px bar per step with a numbered label ("1 · Card"). Steps up to and including the current one are blue. For a single continuous bar use ProgressBar.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | Sign-up flow (Card, Code, Start) | inline-styled segment row in LifestyleLanding.jsx:751 |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `steps` | string[] | — | Labels; numbers are added |
| `current` | number | — | 1-based step the user is on |
| `className` | string | — | |

## States

Done/current segment (blue bar, blue label) and upcoming segment (rule-soft bar, grey label).

## Responsive

Same on all widths.

## Source

- Original: inline styles in components/prototype/LifestyleLanding.jsx:751
- Found in: g-signup, g-code, g-first

## Accessibility

An `<ol>` labelled "Step 2 of 3"; the current step has `aria-current="step"`.
