---
title: QR Block
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - Admin doctor QR
  - PartnerPortal QR
---

# QR Block

Scannable QR presentation with actions.

## Spec

- QR modules on **pure white** (`#FFFFFF`) only — no paper texture behind modules
- Outer frame: 1px rule; commerce radius 14px; padding ~10px
- Actions: download / print / copy via [[Components/Button]] secondary or icon buttons
- Mode switch (shop vs profile): [[Components/Segmented Control]]

## Responsive

See [[Foundations/Breakpoints]].

Fixed QR art size with readable quiet zone; center in column on mobile. Mode switch ([[Components/Segmented Control]]) stacks above the QR when width is tight.

## Finalize
- [ ] Unify admin + partner QR layouts
- [ ] Mark **Final**
