---
title: System — GutGuard Doctors HTML
tags: [gutguard, design-system, systems, doctors]
source: C:\Users\najee\Projects\GutGuard-Doctors-HTML
scanned: 2026-08-12
updated: 2026-08-12
---

# System: GutGuard Doctors HTML

Primary source of the GutGuard design system. Scanned 2026-08-12.

## Role

This system established the brand tokens, three dialects, and most component skins. Later systems should **consume** the vault specs rather than invent parallel classes.

## Dialects in this system

| Dialect | Where | Edge language |
|---|---|---|
| Editorial (booth) | Registration experience + sections | Hard edges, masthead, ruled fields |
| Editorial (marketing) | `GutguardSite.jsx` | Softer radius, pill CTAs, mono eyebrows |
| Commerce | Shop, order status, partner portal | `--r-sm/md/lg/pill` |
| Admin | `/admin/wheel`, `/admin/tiktok`, `/admin/orders` | Hard edges, dense ops UI |

## Shell findings

- **No left sidebar** in this system.
- Admin chrome = hero strip + **horizontal tabs**.
- Marketing / shop use **top nav** (fixed or simple).
- Booth uses **masthead + progress rail** (narrow stage, max ~520px).

## Component harvest (canonical candidates)

| Candidate | Source evidence | Vault note |
|---|---|---|
| Button | `.action`, `.shop-primary`, `.btn-primary`, admin shell buttons | [[Components/Button]] |
| Form field | `FormField.tsx`, shop fields, admin inputs, partner OTP | [[Components/Form Field]] |
| Tabs | `.admin-tabs`, `.admin-tiktok-tabs`, marketing `.sectabs` | [[Components/Tabs]] |
| Segmented control | `.shop-segment`, `.partner-qr-toggle`, `.admin-doctor-qr-toggle` | [[Components/Segmented Control]] |
| Top bar | marketing `Nav`, `.shop-site-header`, `.shop-nav` | [[Components/Top Bar]] |
| Masthead | `Header.tsx` booth | [[Components/Masthead]] |
| Progress rail | `ProgressRail.tsx` | [[Components/Progress Rail]] |
| Card / panel | shop card, admin panel, partner auth card, order panel | [[Components/Card]] |
| Modal | confirm modal, admin modal, shop modal | [[Components/Modal]] |
| Drawer | shop basket/checkout drawer | [[Components/Drawer]] |
| Alert | admin alert, confirm warning, shop error, wheel notice | [[Components/Alert]] |
| Toast | `.admin-toast` | [[Components/Toast]] |
| Badge | `.partner-badge`, marketing beta tags, status pills | [[Components/Badge]] |
| Table | admin TikTok / orders tables | [[Components/Table]] |
| Definition list | confirm rows, reveal meta, admin doctor details | [[Components/Definition List]] |
| Empty state | admin / shop / partner empties | [[Components/Empty State]] |
| QR block | admin doctor QR, partner QR | [[Components/QR Block]] |
| Admin shell | `.admin-wheel-shell` family | [[Components/Admin Shell]] |
| Section label | `SectionLabel.tsx` | [[Components/Section Label]] |
| Task item | `TaskItem.tsx` | [[Components/Task Item]] |

## Brand specials (system-specific, document lightly)

Keep out of the core kit unless another system needs them:

- Prize wheel (`WheelSection`)
- Reveal stage (`RevealSection` — currently unused in live flow)
- Congrats banner CSS (orphaned — no JSX usage found)
- Marketing science visuals (MiAge, constellation, heat/recovery seam)
- Supplement facts panel

## Fragmentation to resolve in the DS

1. **Three button systems** — booth `.action`, shop `.shop-primary`, marketing `.btn-primary` → one [[Components/Button]] with dialect variants.
2. **Three form dialects** — ruled / boxed commerce / dense admin → one [[Components/Form Field]] with variants.
3. **Duplicate QR toggles** — partner vs admin → one [[Components/Segmented Control]].
4. **Duplicate empty / alert classes** → unify under Alert / Empty State notes.

## Source map

| Area | Paths |
|---|---|
| Tokens + skins | `styles/globals.css` |
| Booth components | `components/{ActionButton,FormField,Header,ProgressRail,ConfirmRegistrationModal,TaskItem,SectionLabel}.tsx` |
| Commerce | `components/{Shoplet,OrderStatus,PartnerPortal}.tsx` |
| Marketing | `components/GutguardSite.jsx` |
| Admin | `app/admin/{wheel,tiktok,orders}/page.tsx` |
| Booth sections | `sections/*` |

## Next systems

When scanning the next product, only add components that are **new** or that **conflict** with this harvest. Update this note’s harvest table if Doctors itself gains a sidebar or new chrome.
