---
title: Eyebrow
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/Eyebrow.tsx
example: gutguard-ui/showcase/examples/Eyebrow.tsx
parts: [w-hero, w-trialband, s-co, l-plan]
updated: 2026-10-08
---

# Eyebrow

Mono uppercase label above a heading, a card title, or a group of form fields. For numbered section starts use [[SectionHeading]].

## Variants

| Tone | Use for | Replaces |
|---|---|---|
| `blue` + `rule` | Hero eyebrow with a short line before it | `.eyebrow` |
| `gold` | Group and card labels ("Your first step", "Deliver to") | `.co-grp`, `.sl-lab`, Lifestyle `.g-m` |
| `light` | On blue/dark bands | `.tb-eyebrow` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `tone` | `blue` \| `gold` \| `light` | `gold` | |
| `rule` | boolean | — | Leading 26px line |
| `as` | `span` \| `div` \| `p` | `div` | |

## States

None.

## Responsive

Same on all widths.

## Source

- Original: `.eyebrow`, `.tb-eyebrow`, `.co-grp` in GutguardSite.css; `.g-m` labels inline in LifestyleMember.jsx
- Found in: w-hero, w-trialband, s-co, l-plan

## Accessibility

Decorative label only; don't use it as the only heading of a section.
