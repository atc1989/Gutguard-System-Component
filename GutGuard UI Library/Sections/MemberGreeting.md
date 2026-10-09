---
title: MemberGreeting
tags: [gutguard, ui-library, section]
group: Sections
status: draft
code: gutguard-ui/components/sections/MemberGreeting.tsx
example: gutguard-ui/showcase/examples/MemberGreeting.tsx
parts: [l-greet, l-card-desk]
updated: 2026-10-08
---

# MemberGreeting

The top of the Lifestyle My Health left column: "Kumusta, Rey.", the rank chip and date, then the member's card. On phone the card is a compact row (card thumbnail, name, rank, "CARD ›") with an E-Points tile; from md it is the full MemberCard with a caption. Use it once at the top of My Health; the trial 5-Night Watch card or Business tools go right under it.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| — (one layout, switches at md) | My Health greeting | `.lw-greet`, `.lw-greet-sub`, `.lw-id.gg`, `.lw-sc`, `.lw-scta`, `.lw-sp` + desktop MemberCard |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `greeting` | ReactNode | — | "Kumusta, Rey." |
| `name` | string | — | "Rey Aquino"; upper-cased on the full card |
| `rank` | string | — | "Gut Guardian"; upper-cased on the card |
| `date` | string | — | "Monday, October 5" |
| `points` | number | — | E-Points balance |
| `card` | `{ number?, qr?, qrCaption? }` | — | Passed to the full MemberCard |
| `cardHint` | ReactNode | — | Caption under the full card |
| `onShowCard` | () => void | — | Phone card button (open the card overlay) |
| `onPoints` | () => void | — | Phone E-Points tile and the card's E-Points figure |
| `className` | string | — | |

## States

Card button and E-Points tile: active scale(.97), focus-visible ring. Full card: front / flipped (from MemberCard).

## Responsive

Phone (base): card button row + E-Points tile. From `md` (900px): the full MemberCard (fills the column) and the caption. The original hides the thumbnail and "CARD ›" under 380px; not reproduced (base is 390).

## Source

- Original: `.lw-greet .lw-greet-sub .lw-id.gg .lw-sc .lw-scta .lw-sp` + inline styles in components/prototype/LifestyleMember.jsx:1001
- Found in: l-greet, l-card-desk

## Accessibility

Greeting is an `h1`. Card button: "Show my Lifestyle card and QR". E-Points tile: "15 E-Points". The thumbnail is decorative (`aria-hidden`); the mini QR is a QR glyph, not the member's code.
