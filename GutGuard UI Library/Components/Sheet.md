---
title: Sheet
tags: [gutguard, ui-library, component]
group: Overlays & states
status: draft
code: gutguard-ui/components/ui/Sheet.tsx
example: gutguard-ui/showcase/examples/Sheet.tsx
parts: [s-basket, s-co, s-inside, s-done, l-plan-sheet, l-settings, l-points, l-card]
updated: 2026-10-08
---

# Sheet

A modal panel over a dark scrim, built on the native `<dialog>`: basket, checkout, what's inside, done, and the Lifestyle plan, settings and E-Points sheets. Use `placement="center"` for bare content such as the member card. For the full-screen site menu use [[MobileMenu]].

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `shop` | Shop sheets: grip, serif title, × close. Floats at the bottom right on desktop | `.sl-sheet`, `.sl-scrim`, `.sl-grip`, `.sl-sh-h` |
| `shop` + `checkout` | Checkout and done: 480px on desktop, no bottom padding, so a sticky [[BottomBar]] `sheet` sits flush | `.sl-sheet.sl-co` |
| `lifestyle` | Lifestyle sheets: grab bar, title + subtitle, "Close" pill. Centred on desktop | `.ov-c > .up`, `.grab` |
| `placement="center"` | Bare content centred over the scrim at every width (member card) | `.ov-c` (l-card) |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `open` | boolean | — | Controlled |
| `onClose` | `() => void` | — | Escape, scrim click, close button |
| `title` | string | — | Heading, and the dialog's label |
| `subtitle` | string | — | lifestyle: grey line under the title |
| `variant` | `shop` \| `lifestyle` | `shop` | |
| `placement` | `bottom` \| `center` | `bottom` | `center` drops the panel and header |
| `checkout` | boolean | — | shop: 480px desktop panel, no bottom padding |
| `children` | ReactNode | — | |

Also exports `useModal(ref, open)`, the hook that opens the dialog and locks page scroll ([[MobileMenu]] uses it).

## States

Open slides up from the bottom (centre fades and scales in). Close: × goes darker on hover; the Close pill scales to .97 when pressed.

## Responsive

Phone: bottom sheet, rounded top 24px, at most 90vh tall. shop from `md`: 440px floating panel (480px for checkout), 24px from the bottom and right, rounded 22px. lifestyle from `md`: centred, rounded 20px, at most 88vh tall.

## Source

- Original: `.sl-sheet` etc. in components/GutguardShop.jsx:488; Lifestyle overlay in components/prototype/LifestyleMember.jsx:379
- Found in: s-basket, s-co, s-inside, s-done, l-plan-sheet, l-settings, l-points, l-card
- Simplified: no closing animation (the panel disappears at once). The Lifestyle navy scrim `rgba(15,36,68,.55)` is mapped to `ink/55`, and the grab colour `#e9edf3` to `bone-soft`.

## Accessibility

Native modal `<dialog>` with `aria-label={title}`: focus moves to the first control (the close button), stays inside, and returns to the opener on close. The page behind is inert and does not scroll. Escape and a click on the scrim close it.
