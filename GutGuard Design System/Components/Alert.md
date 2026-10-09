---
title: Alert
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/styles/globals.css
  - ConfirmRegistrationModal, admin pages, Shoplet, WheelSection, PartnerPortal
---

# Alert

Inline feedback inside a page or panel (not floating — see [[Components/Toast]]).

## Variants

| Variant | Treatment |
|---|---|
| Info | Rule border; pale bone-soft ~66%; blue text / 700 |
| Error | Border `rgba(176,32,46,.28–.38)`; wash `rgba(176,32,46,.06–.07)`; title `#B0202E`; body `#8F1824` |
| Compact auth error | 3px red left border; tight padding |
| Confirm warning | `.confirm-warning` in booth modal |
| Admin | `.admin-wheel-alert` (+ `.error`) |
| Shop | `.shop-error` / `.shop-success` |

## Rules

- Square in admin; 14px radius on commerce
- Title often 10px uppercase tracked
- Never icon-only — pair with text
- Live region when the alert appears dynamically

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** — full width of the content column. Multi-line copy wraps; do not truncate error text on mobile.

## Finalize
- [ ] Collapse shop/admin/booth class names into `gg-alert` variants
- [ ] Mark **Final**
