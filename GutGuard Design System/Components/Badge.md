---
title: Badge
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - PartnerPortal (.partner-badge)
  - GutguardSite (BetaFlag)
  - globals status pill patterns
---

# Badge

Compact status or proof chip.

## Variants

| Variant | Treatment |
|---|---|
| Status pill | 1px rule, pill radius, 4px 10px pad; 10px / 900 / uppercase / `.1em` / ink-3 |
| Paid / active | Border `rgba(6,8,169,.32)`, blue text (e.g. `.partner-badge.paid`) |
| Proof chip | Paper tint, rule, pill; slightly tighter pad |
| Marketing beta | `.beta-tag` / `.sec-flag` — editorial flags |

## Rules

- Always include readable status text
- Don’t color entire table rows — badge the status cell
- Pill radius token `--r-pill`

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint — inline chip. May wrap with adjacent text; do not shrink below readable 11–12px caps.

## Finalize
- [ ] Standardize paid/failed/pending/cancelled set
- [ ] Mark **Final**
