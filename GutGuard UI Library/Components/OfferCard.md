---
title: OfferCard
tags: [gutguard, ui-library, component]
group: Patterns
status: draft
code: gutguard-ui/components/patterns/OfferCard.tsx
example: gutguard-ui/showcase/examples/OfferCard.tsx
parts: [w-trialband, g-hero, g-offer, l-firststep]
updated: 2026-10-08
---

# OfferCard

The 5-Night Watch and "Join the movement" offer. The band is the dark site band with the price and button on the side; the box is the Lifestyle paper box used on the landing and for the member's first step. Body text goes in as children, buttons in `actions`.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `band` | Site pages, the ₱499 offer band | `.trialband .tb-eyebrow .tb-h .tb-line .tb-creed .tb-sign .tb-small .tb-side .tb-price` |
| `box` (default) | Lifestyle landing join box, 5-Night Watch box, member "Your first step" | inline-styled boxes in LifestyleLanding.jsx:632 and LifestyleMember.jsx:586 |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | `band` \| `box` | `box` | |
| `eyebrow` | string | — | |
| `title` | ReactNode | — | Wrap the accent in `<em>` (gold italic in the band) |
| `badge` | ReactNode | — | Beside the title in a box, e.g. `<Badge tone="status">New buyers</Badge>` |
| `price` | ReactNode | — | "₱499" |
| `priceCaption` | ReactNode | — | |
| `creed` | string[] | — | The three "Guard …" pills |
| `sign` | string | — | "We Gut You." |
| `note` | ReactNode | — | Small print under the sign-off |
| `actions` | ReactNode | — | Band: beside the price. Box: stacked at the bottom |
| `children` | ReactNode | — | Body text |
| `className` | string | — | |

## States

None of its own; buttons passed in carry their own states.

## Responsive

Band: one column on phone, the button full width; from `md` (900px) the price and button sit in a right column, right-aligned. Title and price scale fluidly (24→36px, 40→60px). Box: same on all widths.

## Source

- Original: `.trialband` and children in components/GutguardSite.jsx:1111; boxes in components/prototype/LifestyleLanding.jsx:632 and components/prototype/LifestyleMember.jsx:586
- Found in: w-trialband, g-hero, g-offer, l-firststep

## Accessibility

Band title is an `h2`, box title an `h3`. Pass real links or buttons in `actions` (`Button variant="light"` in the band).
