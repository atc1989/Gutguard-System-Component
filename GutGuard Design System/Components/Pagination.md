---
title: Pagination
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML (.admin-pagination*)
---

# Pagination

Navigate long admin tables / lists.

## Anatomy

- Meta: “Showing 1–20 of 240” in ink-3
- Controls: Prev / Next square admin buttons
- Optional page-size select (admin field skin)
- Disabled at ends; ≥44px targets where possible

## Visual

- Square dialect with tables
- No pill page numbers unless commerce surface needs them — prefer Prev/Next + page select for ops density

## Responsive

See [[Foundations/Breakpoints]].

On < 900px, show prev/next + current page; collapse excess page numbers into ellipsis. Targets ≥44px where possible.

## Finalize
- [ ] Align with [[Components/Table]]
- [ ] Mark **Final**
