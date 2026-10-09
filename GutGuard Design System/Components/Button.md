---
title: Button
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/components/ActionButton.tsx
  - GutGuard-Doctors-HTML/styles/globals.css (.action, .shop-primary, .shop-secondary)
  - GutGuard-Doctors-HTML/components/GutguardSite.jsx (.btn-primary, .btn-ghost, .btn-bone)
---

# Button

Primary interactive control. One component family; dialect changes geometry and weight, not brand colors.

## Variants

### 1. Editorial primary (booth)

- Classes: `.action` (+ optional `.action-spin`, `.confirm-primary`)
- Full width; ~60–64px high; **square**
- Ink fill `#0F0F18`, bone text
- Padding `22px 28px`; gap `16px`
- Main: Inter Tight 16px / 600
- Optional sub: Fraunces italic 12px / 400 @ 70% opacity
- Optional arrow: 28×28 circle, 1px currentColor border
- Hover → blue + diagonal sheen; active scale `.99`
- Disabled → bone-soft / ink-4

### 2. Commerce primary

- Class: `.shop-primary`
- Blue fill, bone text, **14px** radius
- min-height `62px`; padding `16px 20px`
- Label weight ~900; optional `<small>` support line
- Hover → `--blue-press`
- Disabled → bone-soft / ink-4

### 3. Partner compact primary

- Blue, **9–10px** radius, min-height `48px`
- Loading: 18px spinner, retain size
- Disabled → bone-deep / ink-3 (full opacity)

### 4. Secondary outline

- Classes: `.shop-secondary`, `.confirm-secondary`
- 1px rule, paper/translucent fill, ink text
- Radius 10px commerce; square editorial/admin
- Uppercase micro label ~11–12px / 900 / `.08em`
- Hover → blue border + text

### 5. Text / link button

- Class: `.partner-auth-text-button` (and marketing text links)
- Transparent, blue, 13px / 700, underline offset 3px
- min target 44px

### 6. Marketing pill CTAs

- Classes: `.btn-primary`, `.btn-ghost`, `.btn-bone`, `.nav-cta`
- Soft / pill geometry for marketing dialect only
- Same blue / bone / ink tokens — do not invent new brand colors

### 7. Admin button

- Scoped under `.admin-wheel-shell button` / `.admin-wheel-btn`
- Square, dense, functional
- Icon-only needs 44×44 hit area + accessible name

### 8. Icon button

- 44×44 target; 1px rule; paper fill
- Hover → blue border + glyph

## Shared states

| State | Treatment |
|---|---|
| Focus-visible | 3px gold outline, 3px offset |
| Loading | Keep dimensions; spinner; block re-click |
| Disabled | Muted fill + muted text; `not-allowed` |

## Portable CSS

Map to `gg-btn` / dialect modifiers in [[03 - Portable CSS Starter]].

## Do / don’t

- Do pick one dialect per screen.
- Don’t mix booth hard `.action` with shop rounded primary on the same view.
- Don’t use purple/indigo SaaS defaults.

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** — width follows layout (full-width common on mobile CTAs). Min-height stays ≥44px; do not shrink typography to fit. Stack primary + secondary vertically when the row would wrap awkwardly below 600px.

## Finalize
- [ ] Lock marketing pill vs booth hard as named variants
- [ ] Align partner compact with commerce primary scale
- [ ] Mark **Final** when team agrees
