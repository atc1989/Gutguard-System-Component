---
title: BottomBar
tags: [gutguard, ui-library, component]
group: Shell
status: draft
code: gutguard-ui/components/shell/BottomBar.tsx
example: gutguard-ui/showcase/examples/BottomBar.tsx
parts: [w-offer, s-bar, s-paybtn]
updated: 2026-10-08
---

# BottomBar

A bar fixed to the bottom of the screen that holds the main action. The action is a [[Button]] passed as children. Use the `sheet` variant inside a [[Sheet]], where the bar is sticky rather than fixed.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `offer` | Site offer bar: tag + name, price, skip link, CTA | `.buybar`, `.buybar-inner`, `.bb-*` |
| `action` | Phone buy bar with one full-width button (460px max, centred) | `.sl-bar` |
| `sheet` | Pay button stuck to the foot of the checkout sheet, with a paper fade above | `.co-paywrap` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | `offer` \| `action` \| `sheet` | `offer` | |
| `tag` | string | — | offer: gold mono line |
| `name` | string | — | offer: product name, also the region's label |
| `price` | ReactNode | — | offer: mono amount |
| `priceNote` | string | — | offer: note under the amount |
| `secondary` | ReactNode | — | offer: `<Button variant="link">`, desktop only |
| `className` | string | — | e.g. `md:hidden` on the phone buy bar |
| `children` | ReactNode | — | The action. offer: `<Button arrow size="sm">`; action/sheet: `<Button size="lg">` |

## States

The button carries its own states. The offer bar is always shown.

## Responsive

offer: on phone, tag and name are hidden, the price sits left and the button right. From `sm` (520px; original 620px) the info shows and the price moves right. The skip link shows from `md`. action and sheet: same on all widths (the shop hides the action bar on desktop).

## Source

- Original: `.buybar` in components/GutguardSite.jsx:1297; `.sl-bar` in components/GutguardShop.jsx:482; `.co-paywrap` in components/GutguardShop.jsx:685
- Found in: w-offer, s-bar, s-paybtn
- Simplified: the original offer bar slides in after the hero scrolls away; this one is always shown.

## Accessibility

The offer bar is a `role="region"` labelled with `name`. Bottom padding respects the phone's safe area.
