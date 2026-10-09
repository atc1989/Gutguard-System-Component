---
title: Form Field
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/components/FormField.tsx
  - GutGuard-Doctors-HTML/components/Shoplet.tsx
  - GutGuard-Doctors-HTML/components/PartnerPortal.tsx
  - GutGuard-Doctors-HTML/styles/globals.css
---

# Form Field

Labeled input / select / textarea. Four visual dialects; same error grammar.

## Variants

### 1. Editorial ruled (booth)

- Classes: `.field`, `.field-label`, `.field-input`, `.field-err`
- Transparent; bottom rule only (first field also top rule)
- Label: Fraunces italic 14px, ink-3
- Input: Inter Tight 17px / 500; no radius
- Focus-within → rule + label blue
- Error → `#B0202E` rule/label + 12px message

### 2. Commerce boxed

- Class family: `.shop-field` (Doctors); large prototype `.g-bigin` (Lifestyle — remap only)
- Label: 10px / 900 / uppercase / `.14em` / ink-3
- Control: min-height ~42–48px (Lifestyle large ~60px); 1px rule; bone fill; **10–14px** radius
- Error/help: 12px / 800; error red
- Focus: blue border + pale-blue halo (Doctors grammar — not prototype royal)

### 3. Partner auth

- Labels ~12px / ~750 / ink-2 (normal case)
- Input min-height 52px; paper fill; **9px** radius; 16px text
- Focus: blue border + `0 0 0 3px rgba(6,8,169,.14)`
- Invalid: `#9D2430` border
- OTP / code: mono 24–30px / 700 / `.32em` tracking, centered

### 4. Admin dense

- Scoped under admin shell inputs
- 1px rule; translucent bone fill; **square**
- 15px / 600; padding ~12–13px
- Focus: blue border + 2px pale-blue halo
- Textarea min-height 96px

## Shared rules

- Never use placeholder as the only label
- Helper text: 11–13px, ink-3
- Checkbox: native ~18px with `accent-color: #0608A9` + clickable label
- Touch targets ≥ 44px where interactive

## Portable CSS

`gg-field`, `gg-field--ruled`, `gg-field--boxed`, `gg-field--admin`

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** — fields are 100% of the form column. On < 900px, prefer single-column forms; pair fields side-by-side only from desktop unless each field stays ≥44px tall and readable.

## Finalize
- [ ] Extract shop Field into shared React (or document as CSS-only)
- [ ] Unify error token to `--gg-error`
- [ ] Mark **Final**
