---
title: Hero
tags: [gutguard, ui-library, section]
group: Sections
status: draft
code: gutguard-ui/components/sections/Hero.tsx
example: gutguard-ui/showcase/examples/Hero.tsx
parts: [w-hero, w-hero-actions]
updated: 2026-10-08
---

# Hero

The Home page's opening section: eyebrow, big serif headline with an italic blue accent, serif lead, buttons and a proof checklist, beside a graded portrait with a card overlapping it. Use once, at the top of a marketing page. Not for inner-page headers without a visual.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | One look; the portrait shows a warm duotone placeholder until `image` is set | `header.hero .hero-grid .hero-copy .hero-visual .portrait` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `eyebrow` | ReactNode | — | Blue `Eyebrow` with a leading rule |
| `title` | ReactNode | — | `<em>` = blue italic accent |
| `lede` | ReactNode | — | `<strong>` turns ink, weight 500 |
| `actions` | ReactNode | — | `Button` primary + ghost |
| `proof` | string[] | — | Mono list with blue dots |
| `visual` | ReactNode | — | Overlapping card, e.g. `BloodScanReadout` |
| `image` | string | — | Portrait photo; replaces the placeholder grade |
| `imageAlt` | string | `""` | Photo alt, or the placeholder's `aria-label` |
| `className` | string | — | |

## States

None of its own (buttons carry theirs).

## Responsive

Phone: one column, the card sits under the portrait at full width. From `md` (900): copy and portrait side by side (1.04fr / .96fr, gap 54px), the card overlaps the portrait's lower right (300px wide, 22px past its edge). Headline size is fluid (34–76px).

## Source

- Original: `header.hero`, `.hero-grid`, `.hero-copy`, `.hero-lede`, `.hero-actions`, `.hero-proof`, `.hero-visual`, `.portrait .grade .grain .vig .ph` in components/GutguardSite.jsx:553
- Found in: w-hero, w-hero-actions

## Accessibility

Renders a `<header>` with one `<h1>`. The placeholder portrait is `role="img"` with `imageAlt` as its label; its caption is `aria-hidden`. Proof points are a `<ul>`.
