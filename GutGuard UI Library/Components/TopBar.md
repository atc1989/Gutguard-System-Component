---
title: TopBar
tags: [gutguard, ui-library, component]
group: Shell
status: draft
code: gutguard-ui/components/shell/TopBar.tsx
example: gutguard-ui/showcase/examples/TopBar.tsx
parts: [w-nav, l-nav, g-nav]
updated: 2026-10-08
---

# TopBar

The sticky bar at the top of every page. `site` is the website and shop menu; `app` is the Lifestyle bar with a slot on the right for E-Points and icon buttons. Pair `site` with [[MobileMenu]] for phones.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `site` | Website and shop pages: back button, logo, page name (phone), links, Log in, dark CTA (desktop), menu button (phone) | `.nav`, `.nav-inner`, `.nav-lead`, `.nav-back`, `.brand`, `.nav-here`, `.nav-links`, `.nav-login`, `.nav-cta`, `.burger` |
| `app` | Lifestyle member and landing pages: logo, "/ Lifestyle", links (desktop), right slot | `.lw-nav`, `.lw-nav-in`, `.lw-brand`, `.lw-here`, `.lw-links`, `.lw-right` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | `site` \| `app` | `site` | |
| `links` | `NavLink[]` (`{ label, href, current? }`) | — | `current` turns the link blue and adds the seam underline |
| `here` | string | — | Page name after the logo. Site: phone only. App: always |
| `homeHref` | string | `/` | Logo link |
| `cta` | `{ label, href }` | — | site: dark pill, desktop only |
| `login` | `{ label, href }` | — | site: "Log in" link, desktop only |
| `right` | ReactNode | — | app: E-Points pill, [[IconButton]]s, or a Log in pill |
| `onBack` | `() => void` | — | site: shows the back button |
| `onMenu` | `() => void` | — | site: shows the menu button (phone) |
| `menuOpen` | boolean | — | site: sets `aria-expanded` on the menu button |

## States

Links: hover blue; current blue with the heat-gold-recovery underline. CTA: hover blue, active scale .97. Focus-visible: gold ring.

## Responsive

Switches at `md` (900px; the original switched at 860px). Phone: site shows back, logo, page name, menu button; links, Log in and CTA are hidden. Desktop: links, Log in and CTA show and the page name hides. App: links appear from `md`; side padding grows from 18px to 32px.

## Source

- Original: `.nav*`, `.brand`, `.burger` in components/GutguardSite.jsx:261; `.lw-nav*` in components/prototype/LifestyleMember.jsx:394 and LifestyleLanding.jsx:388
- Found in: w-nav, l-nav, g-nav
- Simplified: the site bar is `sticky`, not `fixed`, so pages don't need top padding; the bottom rule that appears on scroll is left out.

## Accessibility

`<header>` with a `<nav aria-label="Primary">`. The current link gets `aria-current="page"`. Back and menu buttons have labels; the menu button has `aria-haspopup="dialog"` and `aria-expanded`. Pass `onBack`/`onMenu` only from a client component.
