---
title: Segmented Control
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/styles/globals.css (.shop-segment)
  - GutGuard-Doctors-HTML/components/PartnerPortal.tsx (.partner-qr-toggle)
  - GutGuard-Doctors-HTML/app/admin/wheel/page.tsx (.admin-doctor-qr-toggle)
---

# Segmented Control

Mutually exclusive choices in one compact track (not page-level tabs).

## Anatomy

- Track: bone-soft fill, 1px rule, **14px** radius (commerce); square acceptable in admin
- Padding/gap ~4px
- Segments ≥ 44px high; equal height
- Label: 12px / 800 / uppercase / `.08em` / ink-3
- Active: paper fill, ink text, low shadow `0 2px 7px rgba(15,15,24,.09)`
  - Alternate active (partner/admin toggles): blue fill, bone text

## Seen in Doctors as

| Use | Class |
|---|---|
| Shop trial / protocol | `.shop-segment` |
| Partner QR mode | `.partner-qr-toggle` |
| Admin doctor QR mode | `.admin-doctor-qr-toggle` |

## Seen in prototypes (remap to this component)

| Use | Evidence |
|---|---|
| Lifestyle Health / Team / Story | `.gg-tab` |
| Academy EN / Tagalog | `.langs` / `.lang` → also [[Components/Lang Toggle]] |

These should converge to one component with an `activeTone: paper | blue` option.

## vs Tabs

- **Segmented** = filter / mode inside a panel
- **Tabs** = switching major panels or admin sections

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid**. Segments share width equally; allow horizontal scroll only if more than ~4 segments. Min segment height ≥44px on mobile.

## Finalize
- [ ] One shared class / React component
- [ ] Document paper-active vs blue-active
- [ ] Mark **Final**
