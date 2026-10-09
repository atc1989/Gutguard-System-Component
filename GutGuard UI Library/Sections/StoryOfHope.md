---
title: StoryOfHope
tags: [gutguard, ui-library, section]
group: Sections
status: draft
code: gutguard-ui/components/sections/StoryOfHope.tsx
example: gutguard-ui/showcase/examples/StoryOfHope.tsx
parts: [w-soh]
updated: 2026-10-08
---

# StoryOfHope

A member's story: a dark portrait column (eyebrow, photo, one-line quote, name, meta, note) beside what they felt week by week, with a caveat. Use for consented testimonials on the Home page. For a short single quote use `Quote`.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — | One look; "Portrait" placeholder until `image` is set | `.soh .soh-portrait .soh-proof .soh-felt .soh-fr` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `eyebrow` | string | — | "Story of Hope" |
| `image` | string | — | Member photo |
| `imageAlt` | string | `"Portrait"` | Photo alt, or the placeholder label |
| `quote` | ReactNode | — | One line; quote marks added |
| `name` | ReactNode | — | |
| `meta` | ReactNode | — | Mono; `<b>` highlighted ("Age <b>34</b> · Davao City") |
| `note` | ReactNode | — | Tiny placeholder / consent note |
| `title` | ReactNode | — | `<em>` = upright semibold |
| `tether` | ReactNode | — | Mono line under the title |
| `story` | ReactNode | — | Longer italic quote; quote marks added |
| `felt` | `{ when, text, source? }[]` | — | Week rows; quote marks added |
| `caveat` | ReactNode | — | Mono small print |
| `className` | string | — | |

## States

None.

## Responsive

Phone: portrait column on top, story under it. From `md` (900): two columns (300–380px portrait, the rest story), portrait at least 540px tall.

## Source

- Original: `.soh` in components/GutguardSite.jsx:508
- Found in: w-soh

## Accessibility

Title is an `h3`; week rows are an `ol`. The photo uses `imageAlt`.
