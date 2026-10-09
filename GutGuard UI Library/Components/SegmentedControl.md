---
title: SegmentedControl
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/SegmentedControl.tsx
example: gutguard-ui/showcase/examples/SegmentedControl.tsx
parts: [s-toggle, s-for, l-settings]
updated: 2026-10-08
---

# SegmentedControl

Two or three options in a sunken bone track; exactly one is selected and sits on a paper tile. For page sections use Tabs; for many options use OptionCard or ChoiceChip.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `toggle` | Shop plan switch: TRY FIRST · FULL PROTOCOL · SUBSCRIBE (mono uppercase) | `.sl-toggle`, `.sl-toggle.x3` |
| `choice` | Checkout questions: Me · Someone else | `.co-for` |
| `settings` | Lifestyle settings: Jingle · Chime · Silent; a `<small>` in the label becomes a mono sub-line | `.lw-seg`, `.lw-seg.x3` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `options` | `{ value: T; label: ReactNode }[]` | — | Column count follows the option count |
| `value` | T | — | Controlled |
| `defaultValue` | T | — | Uncontrolled |
| `onChange` | (v: T) => void | — | |
| `label` | string | — | aria-label of the group |
| `variant` | `toggle` \| `choice` \| `settings` | `choice` | |
| `className` | string | — | |

## States

default / selected (paper tile, ink text, soft shadow) / focus-visible

## Responsive

`toggle` uses 10px text and tighter padding on phones (the original's ≤400px rule), 11px from `sm` (520px). Others are the same on all widths.

## Source

- Original: `.sl-toggle` GutguardShop.jsx:329, `.co-for` GutguardShop.jsx:561, `.lw-seg` LifestyleMember.jsx:1102
- Found in: s-toggle, s-for, l-settings

## Accessibility

`role="radiogroup"` with `aria-label`; each option is `role="radio"` + `aria-checked`. Roving tabindex: Tab reaches the selected option, arrow keys move and select.
