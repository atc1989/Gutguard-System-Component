---
title: MemberCard
tags: [gutguard, ui-library, component]
group: Patterns
status: draft
code: gutguard-ui/components/patterns/MemberCard.tsx
example: gutguard-ui/showcase/examples/MemberCard.tsx
parts: [l-bigcard, l-card-desk, l-card, g-card, s-minicard]
updated: 2026-10-08
---

# MemberCard

The Gutguard Lifestyle member card: logo, rank, name, card number and E-Points on a blue gradient with the molecule watermark. The full card flips to a QR when `qr` is set. Use `mini` for the small card on the shop Done screen. The phone overlay (dark backdrop, caption, Close) is a dialog around it, not part of the card.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `full` (default) | Member page card, desktop card, phone overlay, landing preview | inline-styled card in LifestyleMember.jsx:308 and LifestyleLanding.jsx:299 |
| `full` + `placeholder` + `corner` | Landing preview ("YOUR NAME HERE", "Free membership / No fees, ever") | g-card |
| `mini` | Shop Done screen ("+1 E-Points") | `.mini-card .mc-l .mc-n .mc-p` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | `full` \| `mini` | `full` | |
| `rank` | string | — | Gold label: "LIFESTYLE MEMBER", "GUT GUARDIAN" |
| `name` | string | — | |
| `number` | string | — | Card or mobile number (full only) |
| `points` | ReactNode | — | Balance (full) or "+1" (mini) |
| `qr` | string | — | QR payload. Shows the small QR and enables the flip |
| `qrCaption` | string | "Show this at the door" | Under the big QR |
| `corner` | ReactNode | — | Bottom-right text instead of the small QR |
| `placeholder` | boolean | — | Dimmed name/number, dashed underline |
| `onPointsClick` | () => void | — | Makes E-Points a button |
| `className` | string | — | |

## States

Front / flipped (QR). Flip animates 0.6s on Y. Focus-visible ring on the QR and points buttons.

## Responsive

Same on all widths. The full card fills its container at 1.586:1; the mini card caps at 300px.

## Source

- Original: inline styles in components/prototype/LifestyleMember.jsx:308, components/prototype/LifestyleLanding.jsx:299; `.mini-card` in components/GutguardShop.jsx:703
- Found in: l-bigcard, l-card-desk, l-card, g-card, s-minicard

## Accessibility

Clicking anywhere on the card flips it (mouse). Keyboard users get real buttons: the bottom-right "Show my QR code" on the front and the whole back face ("Show the front of my card"). The hidden face is `inert`. The QR has `role="img"` "Member QR code". The QR is a placeholder pattern and does not scan yet.
