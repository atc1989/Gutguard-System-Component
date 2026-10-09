---
title: Component Index
aliases: [Components]
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: living
---

# Component index

Canonical GutGuard components. Each note is the team source of truth for look, variants, states, dialect rules, and **Responsive** behavior ([[Foundations/Breakpoints]]).

Harvested first from [[Systems/Doctors-HTML]]. When another system is scanned, add new notes or update variants — do not fork parallel specs.

## Shell / chrome

| Component | Status | Notes |
|---|---|---|
| [[Components/Top Bar]] | Draft | Shop / marketing fixed header (Academy has none — page mast only) |
| [[Components/Sidebar]] | Draft | **New from Academy** — desktop 280px rail (≥900px) |
| [[Components/Bottom Bar]] | Draft | **New from Academy** — mobile sticky “Next” CTA |
| [[Components/Masthead]] | Draft | Booth / Academy page mast (not a fixed top bar) |
| [[Components/Admin Shell]] | Draft | Admin hero + tabbed ops chrome |
| [[Components/Progress Rail]] | Draft | Multi-step booth progress |

## Actions & forms

| Component | Status | Notes |
|---|---|---|
| [[Components/Button]] | Draft | Editorial / commerce / marketing / admin variants |
| [[Components/Icon Button]] | Draft | Square icon control — Lucide SVG (`x`, chevrons, more) |
| [[Components/Form Field]] | Draft | Ruled / boxed / partner / admin |
| [[Components/Segmented Control]] | Draft | Trial/protocol, QR mode toggles |
| [[Components/Switch]] | Draft | Boolean on/off — blue track when on |

## Navigation

| Component | Status | Notes |
|---|---|---|
| [[Components/Tabs]] | Draft | Admin tabs + marketing section tabs |

## Surfaces

| Component | Status | Notes |
|---|---|---|
| [[Components/Card]] | Draft | Editorial panel, commerce card, auth card, admin panel |
| [[Components/Modal]] | Draft | Overlay surface variants (backdrop / shell) |
| [[Components/Dialog]] | Draft | Structured header · body · footer + SVG close |
| [[Components/Drawer]] | Draft | Shop basket / checkout |

## Feedback

| Component | Status | Notes |
|---|---|---|
| [[Components/Alert]] | Draft | Inline info / error |
| [[Components/Toast]] | Draft | Floating dark toast |
| [[Components/Badge]] | Draft | Status pills, proof chips |
| [[Components/Empty State]] | Draft | Quiet empty panels |

## Data

| Component | Status | Notes |
|---|---|---|
| [[Components/Table]] | Draft | Admin data tables |
| [[Components/Definition List]] | Draft | Confirm / detail rows |
| [[Components/QR Block]] | Draft | Printable QR surface |

## Editorial atoms

| Component | Status | Notes |
|---|---|---|
| [[Components/Section Label]] | Draft | Numbered section eyebrow |
| [[Components/Task Item]] | Draft | Verification checklist row |

## Common utilities (added)

| Component | Status | Notes |
|---|---|---|
| [[Components/File Attachment]] | Draft | Custom drop zone — **hide native file input** |
| [[Components/Avatar]] | Draft | Initials or image |
| [[Components/Tooltip]] | Draft | Short hover/focus help |
| [[Components/Pagination]] | Draft | Admin table paging |
| [[Components/Spinner]] | Draft | Inline / block / page loading |
| [[Components/Search Field]] | Draft | Filter input with icon |
| [[Components/Dropdown Menu]] | Draft | ··· overflow actions |
| [[Components/Quantity Stepper]] | Draft | − / value / + (shop & dosing) |
| [[Components/Skeleton]] | Draft | Loading placeholders |

## Extended (nice-to-have)

| Component | Status | Notes |
|---|---|---|
| [[Components/Accordion]] | Draft | FAQ / disclosure — SVG chevron-down (not text ▾) |
| [[Components/Breadcrumbs]] | Draft | Nested path nav |
| [[Components/Date Picker]] | Draft | Calendar booking |
| [[Components/Notification Bell]] | Draft | Bell + badge + panel |
| [[Components/Chat Link Row]] | Draft | External chat CTA row |

## Academy / training (from Gentrep scan)

| Component | Status | Notes |
|---|---|---|
| [[Components/Rank Ladder]] | Draft | Horizontal rank chips |
| [[Components/Rank Plate]] | Draft | Hero progress plate (brand-special) |
| [[Components/Requirement Timeline]] | Draft | Spine + requirement cards |
| [[Components/Event Row]] | Draft | Bookable session row |
| [[Components/Lang Toggle]] | Draft | EN/TL segmented switch |
| [[Components/Certificate]] | Draft | Printable cert — system-special |

## Status key

- **Draft** — extracted from Doctors; needs team finalize pass
- **Final** — locked for team use across systems
- **System-only** — brand special; see Systems notes, not core kit

## Finalize checklist (per component)

- [ ] Variants named and dialect-tagged
- [ ] Default / hover / focus-visible / active / disabled / loading / error covered
- [ ] **Responsive** section present (breakpoints or “container-fluid”) — see [[Foundations/Breakpoints]]
- [ ] Source classes + React files listed
- [ ] Portable `gg-*` mapping noted (or TODO)
- [ ] Conflicts with other systems resolved
- [ ] Status flipped to **Final**
