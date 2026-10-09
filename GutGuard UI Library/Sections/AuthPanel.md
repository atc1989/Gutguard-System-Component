---
title: AuthPanel
tags: [gutguard, ui-library, section]
group: Sections
status: draft
code: gutguard-ui/components/sections/AuthPanel.tsx
example: gutguard-ui/showcase/examples/AuthPanel.tsx
parts: [g-signup, g-first, g-hero, g-card, g-get, g-offer, g-sponsor, g-cta]
updated: 2026-10-08
---

# AuthPanel

The two-column layout of the Lifestyle landing and sign-up: a mono intro line and the member card preview on the left, a mono group label and the form or offer on the right. Use it for the free-card landing, the sign-up details step and the first step. Do not use it for the single-box screens (Code, Log in): those are one centred 460px column.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `sticky="card"` (default) | Sign-up and first step: the card stays put while the form scrolls | `.cols.sticky-l` |
| `sticky="content"` | Landing: the offer and Get my free card stay put while the left side scrolls | `.cols.sticky-r` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `intro` | ReactNode | — | Mono 12.5px line above the card. `<b>` inside turns ink. |
| `card` | ReactNode | — | Left column under the intro: a MemberCard, or several blocks (landing). |
| `title` | string | — | Mono uppercase label over the right column, rendered as `<h2>`. |
| `sticky` | `"card" \| "content"` | `"card"` | Which column is sticky from md. |
| `children` | ReactNode | — | Right column content. |
| `className` | string | — | On the grid. |

## States

None of its own; the form inside carries the states.

## Responsive

Phone: stacked, the right-column label has 30px above it. From `md` (900px): grid `400px | 1fr`, 32px gap, top-aligned, one column `position: sticky` at 88px (under the top bar). From `xl` (1440px; original 1400px): `440px | 1fr`, 44px gap. The page container (`.gg-main`, 460 → 560 → 1040 → 1160px) stays in the screen, not in AuthPanel.

## Source

- Original: `.cols .sticky-l .sticky-r .col-l .col-r` plus inline intro/label styles in LifestyleLanding.jsx:632 (landing) and :751 (sign-up screens)
- Found in: g-signup, g-first, and the landing column layout around g-hero … g-cta

## Accessibility

The right-column label is a real `<h2>`. Sticky columns don't change reading order: left column first, then right.
