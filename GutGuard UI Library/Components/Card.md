---
title: Card
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/Card.tsx
example: gutguard-ui/showcase/examples/Card.tsx
parts: [w-symptoms, w-about, w-phases, w-dose, w-miage, l-plan, g-offer]
updated: 2026-10-08
---

# Card

A bordered box with optional slots: eyebrow, title, aside, meta, body, footer. `CardRow` adds key/value lines and `CardGrid` lays cards out. Use it for any boxed group of content; use `OptionCard` when the box is a choice, `OfferCard` for offers.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `paper` (default) | Site cards: phases, dose plans, about | `.phase-card`, `.dose-card`, `.about-card` |
| `bone` | Symptom cards with a heat tag | `.symptom` |
| `dark` | Cards on the dark MiAge band | `.ms-card` |
| `panel` | Lifestyle panels (title + badge on the right) | My plan card, 5-Night Watch box |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | see above | `paper` | |
| `eyebrow` | ReactNode | — | Mono label above the title ("Phase 1"); heat with a dash on `bone` |
| `title` | ReactNode | — | Rendered as `h3` |
| `aside` | ReactNode | — | Beside the title: a `Badge` on panels, a mono tag on `dark` |
| `meta` | ReactNode | — | Blue line under the title |
| `footer` | ReactNode | — | Small mono grey line at the bottom |
| `children` | ReactNode | — | Body; text takes the variant's body style |
| `className` | string | — | |

`CardRow`: `label`, `value`, `className`. Bordered row on site cards; borderless "Next refill … value" line on panels.

`CardGrid`: `columns` `2 | 3` (default 3), `className`, `children`.

## States

None (static). Put a `Button` in the body for actions.

## Responsive

`CardGrid` stacks on phone and goes 2 or 3 across from `md` (900px). Cards are the same on all widths.

## Source

- Original: `.grid3 .symptom`, `.about-grid .about-card`, `.phase-cards .phase-card`, `.dose-cards .dose-card .dc-row`, `.miage-supports .ms-card` in components/GutguardSite.jsx:630, :1211, :1140, :1163, :367; Lifestyle panels in components/prototype/LifestyleMember.jsx:586 and LifestyleLanding.jsx:632
- Found in: w-symptoms, w-about, w-phases, w-dose, w-miage, l-plan, g-offer

## Accessibility

Title is an `h3`; place cards under a section `h2`. Plain `div`, no interaction of its own.
