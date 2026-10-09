---
title: Button
tags: [gutguard, ui-library, component]
group: Primitives
status: draft
code: gutguard-ui/components/ui/Button.tsx
example: gutguard-ui/showcase/examples/Button.tsx
parts: [w-hero-actions, w-offer, w-trialband, s-bar, s-card, s-free, s-paybtn, s-done, g-cta, l-firststep, g-first]
updated: 2026-10-08
---

# Button

Every button and text link on the website, shop and Lifestyle. Use `primary` for the single main action on a screen. Renders an `<a>` when `href` is set, otherwise a `<button>`.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `primary` | Main action (blue pill) | `.btn-primary`, `.bb-cta`, `.slw-buy`, `.co-paybtn`, Lifestyle `button.tap` (blue) |
| `dark` | Top-bar call to action | `.nav-cta` |
| `light` | Action on a blue/dark band | `.tb-btn` |
| `outline` | Secondary action inside a card | Lifestyle "Manage my plan" |
| `ghost` | Secondary action next to a primary (ringed arrow) | `.btn-ghost` |
| `link` | Small text action | `.co-link`, `.sl-free`, `.bb-skip`, `.sheet-login` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | see above | `primary` | |
| `size` | `sm` \| `md` \| `lg` | `md` | `lg` = full width, 54px: phone buy bar, pay button, Lifestyle main button. Ignored by `ghost`/`link`. |
| `arrow` | boolean | — | Trailing arrow in a ring |
| `suffix` | ReactNode | — | Muted text after the label: `· ₱499` |
| `href` | string | — | Renders `<a>` |
| …rest | button / anchor attributes | | `disabled`, `onClick`, `target` … |

## States

Hover: primary darkens to `blue-press` and lifts 2px; dark turns blue. Active: back down / scale .97. Focus-visible: 3px gold ring. Disabled: 70% opacity, not clickable.

## Responsive

Same on all widths. Use `size="lg"` for the full-width phone button.

## Source

- Original: `.btn-primary`, `.btn-ghost`, `.nav-cta`, `.tb-btn` in components/GutguardSite.jsx (CSS components/GutguardSite.css); `button.tap` in components/prototype/LifestyleMember.jsx / LifestyleLanding.jsx
- Found in: w-hero-actions, w-offer, w-trialband, s-bar, s-card, s-free, s-paybtn, s-done, g-cta, l-firststep, g-first

## Accessibility

Real `<button type="button">` / `<a>`. The arrow icons are `aria-hidden`. Keep labels as words ("Start my 5 nights"), not icons.
