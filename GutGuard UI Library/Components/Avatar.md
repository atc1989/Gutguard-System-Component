---
title: Avatar
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/Avatar.tsx
example: gutguard-ui/showcase/examples/Avatar.tsx
parts: [w-review, l-family, g-sponsor, l-team]
updated: 2026-10-08
---

# Avatar

Initials in a circle, for people rows ([[PersonRow]]) and quotes ([[Quote]]). No photos yet.

## Variants

| Tone | Use for | Replaces |
|---|---|---|
| `bone` | Family / team members | Lifestyle family row initials |
| `ink` | Sponsor | Landing sponsor row |
| `gold` | Review quotes | `.review-av` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `initials` | string | — | 1–2 letters |
| `tone` | `bone` \| `ink` \| `gold` | `bone` | |
| `size` | number (px) | 38 | Quotes use 44 |

## States

None.

## Responsive

Same on all widths.

## Source

- Original: `.review-av` in GutguardSite.css; initials spans inline in LifestyleMember.jsx / LifestyleLanding.jsx
- Found in: w-review, l-family, g-sponsor, l-team

## Accessibility

`aria-hidden`: the person's name next to it carries the meaning.
