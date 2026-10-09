---
title: Icon Button
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Icon Button

Square control that shows a single icon. Used for Dialog close, Accordion chevron, date-picker arrows, overflow menus.

## Spec

- Hit target **≥44×44px** (dense admin **36×36px** allowed)
- Border 1px `--rule`; fill `--paper`; radius `--r-sm` (10px) in commerce; **0** in editorial/admin when matching shell
- Icon: **Lucide-style** SVG — 24×24 viewBox, stroke `currentColor`, stroke-width **2**, round caps/joins
- In products: prefer `lucide-react` (`X`, `ChevronDown`, `ChevronLeft`, `ChevronRight`, `MoreHorizontal`)
- In Showcase / static HTML: inline the same paths

## States

| State | Treatment |
|---|---|
| Default | ink / rule border |
| Hover | border + icon → blue |
| Focus-visible | gold 3px outline offset 3px |
| Active | slight press (opacity or scale `.98`) |
| Disabled | ink-4; no hover blue |

## Canonical icons (Showcase)

| Use | Lucide name |
|---|---|
| Close / dismiss | `x` |
| Accordion | `chevron-down` (rotate 180° when open) |
| Prev / next | `chevron-left` / `chevron-right` |
| Overflow | `more-horizontal` |

## A11y

Always set `aria-label` (or visible text elsewhere). Icon-only buttons must not rely on the glyph alone.

## Related

[[Components/Dialog]] · [[Components/Accordion]] · [[Components/Button]] · [[Components/Dropdown Menu]]

## Portable CSS

`.gg-icon-btn` — see [[03 - Portable CSS Starter]]

## Showcase

`Showcase/index.html` → `#icon-button`

## Responsive

See [[Foundations/Breakpoints]].

Keep **≥44×44px** on mobile. Dense **36px** only in admin toolbars at any width. Icon SVGs stay 20px; hit target does not shrink with the glyph.

## Finalize
- [ ] Mark **Final** after second product adopts
