---
title: Event Row
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.ev, .datebox, .ev-place, .ev-meta, .ev-seats, .confirm)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Event Row

Bookable session row inside a requirement card.

## Anatomy

- Date tile (`.datebox`) — month + day number (display type)
- Place title + meta (time, venue) + seats line
- Confirm stack — [[Components/Button]] sm (book / booked / cancel)

## States

| State | Treatment |
|---|---|
| Available | Default card border |
| Mine / booked | `.ev.mine` gold border; button `.booked` |
| Full / disabled | Disabled button |

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid**. Stack time/meta under title on narrow screens; keep booking CTA full-width or trailing ≥44px.

## Finalize
- [ ] Remap gold booked state to GG tokens
- [ ] Mark status
