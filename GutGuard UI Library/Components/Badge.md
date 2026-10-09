---
title: Badge
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/Badge.tsx
example: gutguard-ui/showcase/examples/Badge.tsx
parts: [w-hero, w-miage, w-doors, s-chips, s-watch, l-plan, g-offer, l-team]
updated: 2026-10-08
---

# Badge

A short mono label for a state or an offer ("Beta test", "ACTIVE", "Best rate"), plus the coloured-dot status line on My Team. Not clickable.

## Variants

| Tone | Use for | Replaces |
|---|---|---|
| `outline` | Neutral notice: "Under construction" | `.soon-badge` |
| `beta` | Features in beta (dashed gold) | `.bs-beta`, `.mh-beta` |
| `status` | Plan / offer state: "ACTIVE", "NEW BUYERS" | Lifestyle inline badges |
| `solid` | Tag on a chip: "Popular"; `active` makes it blue: "Best rate" | `.ctag` |
| `text` | Inline benefit, no box: "Free shipping" | `.tfree`, `.sl-lab .save` |
| `dot` (prop) | Member status: Drinking / Slipping / Stopped | My Team rows |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `tone` | see above | `outline` | |
| `active` | boolean | — | Blue fill for `solid` |
| `dot` | `ok` \| `warn` \| `stop` | — | Switches to a sans status line with a dot (recovery / gold / heat) |

## States

None (static).

## Responsive

Same on all widths.

## Source

- Original: `.soon-badge`, `.bs-beta`, `.mh-beta`, `.ctag`, `.tfree` in GutguardSite.css; status spans and team dots inline in LifestyleMember.jsx
- Found in: w-hero, w-miage, w-doors, s-chips, s-watch, l-plan, g-offer, l-team

## Accessibility

Plain text, so it is read out as written. The dot is `aria-hidden`; the word carries the meaning.
