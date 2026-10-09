---
title: Definition List
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - ConfirmRegistrationModal (.confirm-row)
  - RevealSection (.reveal-meta-row)
  - Admin doctor details
---

# Definition List

Term / value rows for confirmations and detail summaries.

## Spec

- Thin rule separators between rows
- Term: Fraunces italic **or** uppercase micro-label in ink-3
- Value: Inter Tight 500–700, ink
- Long identifiers: `overflow-wrap: anywhere`
- Used in modals, reveal meta, admin detail panes, shop order meta

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid**. Stack dt above dd on narrow widths if a side-by-side row would crush labels; from desktop, two-column rows OK.

## Finalize
- [ ] Pick term style per dialect (italic editorial vs micro-label admin)
- [ ] Mark **Final**
