---
title: BusinessTools
tags: [gutguard, ui-library, section]
group: Sections
status: draft
code: gutguard-ui/components/sections/BusinessTools.tsx
example: gutguard-ui/showcase/examples/BusinessTools.tsx
parts: [l-tools]
updated: 2026-10-08
---

# BusinessTools

A collapsed paper box on My Health for builders: "Business tools", three small coloured tool tiles (GEMA, Academy, GG Verse) and a chevron. Tapping it opens whatever you pass as children. Only the closed state was captured, so the open panel is up to the caller.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | Builder tools under the greeting on My Health | inline box + `button[aria-expanded][aria-controls=gg-tools]` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `label` | string | — | "Business tools" |
| `tools` | `{ label, icon, className? }[]` | — | Tile icon (Lucide) and tile colour class, e.g. `bg-recovery-deep` |
| `defaultOpen` | boolean | false | |
| `children` | ReactNode | — | The open panel |
| `className` | string | — | |

## States

Closed / open (chevron turns 180°). Focus-visible ring on the toggle.

## Responsive

Same on all widths.

## Source

- Original: inline styles in components/prototype/LifestyleMember.jsx:586
- Found in: l-tools
- Tile colours in the capture (#1F5D99, #1E9E57, #0E2249) are off-token; the example uses `recovery-deep`, `recovery`, `slate-2`. There is no green token.

## Accessibility

The row is a real button with `aria-expanded` and `aria-controls` pointing at the panel. Tiles are `aria-hidden` (the label names the group).
