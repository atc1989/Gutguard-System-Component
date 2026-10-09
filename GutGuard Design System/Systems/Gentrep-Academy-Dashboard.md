---
title: System — Gentrep Academy Dashboard
tags: [gutguard, design-system, systems, academy, gentrep]
source: d:\Users\najee\Downloads\gentrep-academy-dashboard.html
inbox: GutGuard Design System/Inbox/gentrep-academy-dashboard/
scanned: 2026-08-12
updated: 2026-08-12
---
t
# System: Gentrep Academy Dashboard

**Prototype only.** Harvest structure and component shapes; **always restyle with** [[Systems/Doctors-HTML]] (bone, ultramarine, Fraunces, Inter Tight). Boss theme `m` below is remap reference — not DS tokens.

Boss input: single-file React SPA (minified). CSS is a template string driven by theme object `m`.

Also in vault: Inbox notes + Stitch run under `Inbox/gentrep-academy-dashboard/`.

## What this product is

A **rank ladder training dashboard**: pick a rank → see progress plate → complete requirements (docs, attendance booking, demos) → earn certificate. Mobile-first; desktop adds a left sidebar.

## Screens / surfaces

| Surface | How it appears |
|---|---|
| Ladder dashboard | Primary view — mast, ladder, plate, chat CTA, requirements timeline |
| About | Sheet — levels table + rules |
| Document reader | Sheet — agreement/ethics/creed + EN/TL lang toggle |
| Video | Sheet — poster + play |
| Booking | Inline expand inside requirement card — event rows |
| Certificate | Sheet / print — cream ceremonial card + QR |
| Toast + confetti | Completion feedback |

Ranks: **BASE → TL → SL → PL → CC**.

## Theme tokens (boss — not GutGuard)

```js
m = {
  navy: "#0e2249", navyD: "#07142e",
  blue: "#2569b8", sky: "#9DB8DE",
  paper: "#eef2f7", card: "#ffffff",
  ink: "#1a2740", mute: "#5a6b82",
  gold: "#f5b716", goldD: "#8a5a00",
  line: "#e2e8f0",
  good: "#157a43", goodBg: "#E4F4EC",
  warn: "#8a5a00", warnBg: "#FDF4E0",
  clay: "#a63a20", clayBg: "#FBEAE5",
  olive: "#3f4c37", oliveLt: "#EDEFE9",
  brand: "#1f5d99", brandD: "#163f66",
  tg: "#1373a2",
}
```

Fonts: **Anton** (display) · **Sora** (UI/buttons) · **Inter** (body) · **Playfair Display** italic (brand / cert name).

> When restyling into GutGuard, remap to bone / ultramarine / Fraunces / Inter Tight — see conflict table below. Do **not** treat boss colors as new DS tokens unless the team explicitly wants an Academy dialect.

## Shell (important)

| Chrome | Mobile | Desktop ≥900px |
|---|---|---|
| [[Components/Sidebar]] `.side` | **Hidden** | Sticky **280px** left rail |
| [[Components/Top Bar]] | **No fixed top bar** — page [[Components/Masthead\|mast]] only | Mast moves into main column; brand also in sidebar |
| [[Components/Bottom Bar]] `.foot` | Fixed sticky “Next” CTA | **Hidden** (sidebar `side-next` replaces it) |
| Main column `.col` | max-width 440px | Fluid inside shell max ~1240px |

This is the first scanned system with a real **sidebar** and **bottom bar**.

## Component harvest

### Map to existing DS components

| Candidate | Boss evidence | Vault note | Action |
|---|---|---|---|
| Button | `.btn` + primary/navy/tg/outline/danger/booked/sm/wide | [[Components/Button]] | Add Academy variants; remap colors to GG |
| Badge / pill | `.pill` | [[Components/Badge]] | Compact nav/about pill |
| Card | `.req-card`, `.chat`, `.ev` | [[Components/Card]] | Active/missed/mine borders |
| Modal / sheet | `.modal` + `.sheet` (bottom sheet mobile, centered desktop) | [[Components/Modal]] / [[Components/Drawer]] | Document sheet pattern |
| Toast | `.toast` | [[Components/Toast]] | Already exists |
| Alert / outcome | `.outcome` | [[Components/Alert]] | Success/olive bands |
| Progress (bar/pips) | `.bar`, `.pips` / `.pip` | related to [[Components/Progress Rail]] | Different metaphor — new or extend |
| Section label | `.bar-title` + `.sec` | [[Components/Section Label]] | Anton uppercase + hairline |
| Empty / fine copy | `.fine`, empty booking copy | [[Components/Empty State]] | Light use |

### New DS components (from this scan)

| Candidate | Classes | Vault note | Layer |
|---|---|---|---|
| **Sidebar** | `.side` `.who` `.avatar` `.side-nav` `.side-rank` `.side-btn` `.side-next` | [[Components/Sidebar]] | Shell |
| **Bottom Bar** | `.foot` `.foot-in` `.foot-title` `.eyebrow-dark` | [[Components/Bottom Bar]] | Shell |
| **Rank Ladder** | `.ladder` `.rung` `.ant` `.lock` | [[Components/Rank Ladder]] | Content |
| **Rank Plate** | `.plate` `.plate-*` `.hatch` `.pips` `.bar` | [[Components/Rank Plate]] | Brand-special |
| **Requirement Timeline** | `.reqs` `.req` `.spine` `.rail` `.node` `.req-card` | [[Components/Requirement Timeline]] | Content |
| **Event Row** | `.ev` `.datebox` `.ev-place` `.confirm` | [[Components/Event Row]] | Content |
| **Lang Toggle** | `.langs` `.lang` | [[Components/Lang Toggle]] | Content |
| **Certificate** | `.cert` `.cert-*` | [[Components/Certificate]] | Brand-special / system-only |
| **Chat CTA row** | `.chat` `.tg` | keep under Card or small “Link row” — see harvest note below | Content |

### System-only / don’t force into core kit yet

- Rank insignia metals (bronze / silver / gold seals)
- Confetti (`.cf-wrap`)
- Demo QA panel (`.demo`)
- Telegram brand tile color (`.tg`)
- Video poster (`.video` `.play`) and Doc reader (`.doc`) — simple sheet body patterns

## Anatomy snapshots

### Sidebar (desktop)

```
┌─ 280px sticky ─────────────┐
│ Gentrep (Playfair)         │
│ [avatar] Name · Team       │
│ ○ BASE                     │
│ ● TL          (on)         │
│ ○ SL  lock                 │
│ …                          │
│ [ About Academy ]          │
│ Do this next →             │
└────────────────────────────┘
```

### Mobile mast (not a Top Bar)

```
Gentrep Academy          [About]
Rey · Bravo
[ BASE ] [ TL ] [ SL ] …
```

### Bottom Bar (mobile)

```
┌────────────────────────────┐
│ DO THIS NEXT               │
│ Book Testimonial Session → │
└────────────────────────────┘
```

### Requirement row

```
(node)──┐
 rail   │  ┌ req-card ─────────────┐
        │  │ TYPE                  │
        │  │ Title                 │
        │  │ helper                │
        │  │ [ Action button ]     │
        │  │ optional .dates/.ev   │
        │  └───────────────────────┘
```

## Conflicts with GutGuard DS

| Axis | Academy boss | GutGuard | Decision needed |
|---|---|---|---|
| Canvas | cool `#eef2f7` | warm bone `#F4F1EA` | Remap to bone when implementing GG |
| Action blue | `#2569b8` | `#0608A9` | Remap |
| Brand navy | `#0e2249` fills + text | ink + ultramarine split | Don’t keep navy as primary action |
| Gold | bright `#f5b716` progress | muted `#B08D5B` accent | Need semantic “progress gold” vs premium gold |
| Fonts | Anton / Sora / Inter / Playfair | Fraunces / Inter Tight | Full remap |
| Focus ring | 3px blue | 3px gold | Follow GG (gold) |

Stitch Inbox run already used **commerce** dialect + bone — structure from this file, visuals from DS.

## Finalize priorities from this system

1. Lock [[Components/Sidebar]] + [[Components/Bottom Bar]] (new shell pieces)
2. Extend [[Components/Button]] / [[Components/Modal]] for sheet + booked/danger variants
3. Add Academy content components (Ladder, Plate, Timeline, Event Row)
4. Keep Certificate as system-special unless another product needs it
