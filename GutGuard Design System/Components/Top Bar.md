---
title: Top Bar
aliases:
  - Site Header
  - App Header
tags: [gutguard, design-system, components, shell]
updated: 2026-08-12
status: draft
sources:
  - GutGuard-Doctors-HTML/components/Shoplet.tsx (.shop-site-header)
  - GutGuard-Doctors-HTML/components/GutguardSite.jsx (Nav)
  - GutGuard-Doctors-HTML/components/OrderStatus.tsx / PartnerPortal.tsx (.shop-nav)
---

# Top Bar

Horizontal chrome pinned to the **top** of public / commerce screens. This is the component formerly drafted as “Site Header.”

## Where it exists in Doctors

| Surface | Has top bar? | What you see instead |
|---|---|---|
| Shop (`Shoplet`) | **Yes** — fixed `.shop-site-header` | — |
| Marketing site | **Yes** — fixed `.nav` | — |
| Order status / partner | **Yes (light)** — `.shop-nav` strip | — |
| Admin (`/admin/*`) | **No** | Page hero (`.admin-wheel-hero`) + [[Components/Tabs]] |
| Booth registration | **No** | [[Components/Masthead]] (program header, not IA nav) |
| Gentrep Academy | **No** | Page `.mast` + desktop [[Components/Sidebar]] + mobile [[Components/Bottom Bar]] |
| GutGuard Lifestyle | **No** | In-page mast + [[Components/Sidebar]] + [[Components/Bottom Bar]] + [[Components/Segmented Control]] for Health/Team/Story |

So if you were looking at **admin**, you will not see a top bar — that screen never had one.

## Canonical anatomy (shop top bar — best reference)

```
┌─────────────────────────────────────────────────────────┐
│ ▬ heat→gold→recovery accent (2px)                       │
│  Brand     · Links · Links ·     Login    [Basket]      │
└─────────────────────────────────────────────────────────┘
```

- Fixed; `z-index: 100`
- Background: bone @ ~96% + `backdrop-filter: blur(14px)`
- Bottom border: `1px solid rgba(20,16,25,.08)`
- Soft shadow: `0 5px 14px rgba(20,16,25,.04)`
- Inner: max-width ~1320px; padding `12px 32px`
- Grid: brand | links | actions
- Links: 14px / 600 / ink-2; hover + current → blue; current gets 2px blue underline
- Actions slot: login text + basket (or CTA)
- Mobile: collapse links into menu / sheet

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` | Collapse link row into menu / sheet ([[Components/Drawer]]); keep brand + primary action visible; reduce horizontal padding (~16px) |
| `≥ 900px` | Full brand \| links \| actions grid; inner max-width ~1320px; padding ~12×32 |

Optional: at `< 600px`, icon-only basket/actions if labels collide.

## Variants

### 1. Full top bar (shop / marketing)

- Shop: `.shop-site-header` …
- Marketing: `.nav` (+ `.scrolled`) …
- Slots: brand · links · actions (CTA or basket)

### 2. Simple top bar

- `.shop-nav` + `.shop-brand` + `.shop-nav-link`
- Lightweight; used on order status / partner

## Visual rules

- Bone surface, ink text, blue for current/hover
- Focus-visible: 3px gold outline, 3px offset
- CTA / basket uses [[Components/Button]] patterns
- Mobile menu → sheet ([[Components/Drawer]] family)

## Not a top bar

- [[Components/Masthead]] — booth logos + edition
- [[Components/Admin Shell]] hero — large title block, not a nav bar
- [[Components/Tabs]] — sit under admin hero; not a top bar

## Sidebar

Doctors has **no sidebar**. If a later system adds one, create `Components/Sidebar.md` — do not stretch Top Bar to cover it.

## Finalize

- [ ] Lock full vs simple variants + measurements
- [ ] Unify shop + marketing into one Top Bar with slots
- [ ] Decide whether admin should ever get a top bar (today: no)
- [ ] Mark **Final**
