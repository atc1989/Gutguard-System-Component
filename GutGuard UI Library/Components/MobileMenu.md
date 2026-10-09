---
title: MobileMenu
tags: [gutguard, ui-library, component]
group: Overlays & states
status: draft
code: gutguard-ui/components/ui/MobileMenu.tsx
example: gutguard-ui/showcase/examples/MobileMenu.tsx
parts: [w-menu]
updated: 2026-10-08
---

# MobileMenu

The full-screen phone menu that drops from the top when you tap the [[TopBar]] menu button: numbered serif links, the main button and a log-in line. It is for phones; desktop shows the links in the top bar.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| (one) | Site menu on phone | `.sheet#mobile-menu.open`, `.sheet-close`, `.sheet .nav-cta`, `.sheet-login` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `open` | boolean | — | Controlled |
| `onClose` | `() => void` | — | Escape, close button, or a link tap |
| `links` | `NavLink[]` (`{ label, href, current? }`) | — | Numbered 01, 02, … automatically; `current` is blue |
| `cta` | `{ label, href }` | — | Dark full-width pill ("Start my 5 nights · ₱499") |
| `login` | `{ label, href }` | — | Grey line at the bottom |

## States

Opens by sliding down from the top (no animation with reduced motion). Links: current page in blue. Log-in line turns blue on hover. Focus-visible: gold ring.

## Responsive

Same on all widths. Side padding grows with the screen (20–32px).

## Source

- Original: `.sheet` markup in components/GutguardSite.jsx:280
- Found in: w-menu
- Simplified: the original CTA also picks up the links' 1px bottom rule; dropped.

## Accessibility

Native modal `<dialog id="mobile-menu" aria-label="Site menu">`: focus moves to the close button and stays inside; Escape closes and focus returns to the menu button. The current link has `aria-current="page"`.
