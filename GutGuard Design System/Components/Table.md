---
title: Table
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/app/admin/tiktok/page.tsx
  - GutGuard-Doctors-HTML/app/admin/orders/page.tsx
---

# Table

Dense admin data display.

## Spec

- Light rule dividers; bone/paper surfaces
- Header: 10–11px / 800–900 / uppercase / wide tracking / ink-3
- Cell: 12–15px ink; supporting line ink-3
- Row actions: compact square admin buttons
- Status: [[Components/Badge]] — not full-row color fills
- Align numbers consistently; tabular numerals when available
- Wrapper: scroll container for wide tables (`.admin-tiktok-table-wrap`)

## Related

- Doctor list rows (`.admin-doctor-row`) are a list/card hybrid — keep separate unless they become a true table
- Pagination: `.admin-pagination` family lives with Table for now

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| < 900px | Horizontal scroll in a ruled wrapper **or** cardized rows (product choice — document in repo). Keep actions reachable |
| ≥ 900px | Full table; sticky header optional |

Never hide critical columns without a detail drill-in.

## Finalize
- [ ] One table class (drop per-page duplicates)
- [ ] Document compact modifier
- [ ] Mark **Final**
