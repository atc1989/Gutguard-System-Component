---
title: ProtocolSteps
tags: [gutguard, ui-library, section]
group: Sections
status: draft
code: gutguard-ui/components/sections/ProtocolSteps.tsx
example: gutguard-ui/showcase/examples/ProtocolSteps.tsx
parts: [w-proto]
updated: 2026-10-08
---

# ProtocolSteps

The SynBIOTIC+ illustration (heat/recovery capsule with a molecule on a blue square) beside the protocol's three roman-numeral steps. The steps are `Timeline variant="steps"`; use that on its own when there's no product art.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | One look | `.proto-grid .product .prod-cap .bottle .plus .spec` + `.steps .step-row .step-n` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `name` | string | — | Serif name on the art; label "<name> (illustration)" |
| `tagline` | string | — | Mono line under the name |
| `spec` | string | — | Mono line at the foot of the art |
| `steps` | `TimelineItem[]` | — | `{ label: "I", title, text }`; `<sup><a>` footnotes turn blue |

## States

None.

## Responsive

Phone: art on top, steps under it (gap 32px). From `md` (900): side by side (.9fr / 1.1fr, gap 48px).

## Source

- Original: `.proto-grid` in components/GutguardSite.jsx:648
- Found in: w-proto

## Accessibility

The art is `role="img"` with a label; the SVG inside is hidden. Steps are an `ol` with the numerals hidden.
