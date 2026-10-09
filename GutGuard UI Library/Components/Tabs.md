---
title: Tabs
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/Tabs.tsx
example: gutguard-ui/showcase/examples/Tabs.tsx
parts: [w-sectabs, l-tabs]
updated: 2026-10-08
---

# Tabs

Sticky row of tabs under the top bar. Pills jump between sections of a long site page; underline switches the Lifestyle My Health / My Story / My Team views. For two or three settings choices use SegmentedControl.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `pills` | Section jump links, mono pills, seam line under the bar | `.sectabs`, `.sectab` |
| `underline` | Lifestyle views, blue underline, optional heat count badge | `.lw-tabs`, `.lw-tab`, `.bd` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `items` | `{ value: T; label: ReactNode; badge?: ReactNode }[]` | — | |
| `value` | T | — | Controlled |
| `defaultValue` | T | first item | |
| `onChange` | (v: T) => void | — | |
| `label` | string | — | aria-label of the tablist |
| `variant` | `pills` \| `underline` | `pills` | |
| `className` | string | — | On the sticky bar |

## States

default / hover (pills: blue text) / selected (pills: bone fill + rule border + blue; underline: ink + blue underline) / focus-visible

## Responsive

Row scrolls sideways when it overflows. Sticks at 73px (pills, under the site nav); underline at 53px, 55px from `md`. Underline side padding 18px → 32px from `md`.

## Source

- Original: `.sectabs` GutguardSite.jsx:1094, `.lw-tabs` LifestyleMember.jsx:994
- Found in: w-sectabs, l-tabs

## Accessibility

`role="tablist"` + `role="tab"` + `aria-selected`. Roving tabindex; Left/Right, Home/End move and select. No scroll-spy: for section tabs the caller tracks the visible section and passes `value`, and scrolls in `onChange`. The original's show-on-scroll (fixed, slides in) is not built; it is plain sticky.
