---
title: Certificate
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.cert, .cert-*)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Certificate

Ceremonial rank certificate surface. **System-special** — print-optimized.

## Anatomy

- Cream card (`#FCFAF4` / `#F3EFE4`), navy outline (6px inset offset)
- Brand row, eyebrow, “hereby certifies”, italic display name
- Rank line, horizontal rule, citation, evidence list
- Signature row + QR + record fields + fine print
- Actions outside print: download / share (no-print)

## Notes

- Closest GG cousins: ceremonial panels + [[Components/QR Block]]
- Keep print CSS: hide shell/foot/toast; expand sheet

## Responsive

See [[Foundations/Breakpoints]].

Scale certificate surface to viewport width with margins; preserve print aspect. On mobile, offer download/print rather than tiny unreadable preview-only.

## Finalize
- [ ] Keep as Academy system-only unless another product needs certificates
- [ ] Mark status
