---
title: Accordion
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Accordion

Expand/collapse sections for FAQ, settings groups, long help.

## Spec

- Header row: min 48px, Inter Tight 600–700
- Trailing indicator: **SVG chevron-down** via [[Components/Icon Button]] pattern (not text `▾` / `▼`)
- Chevron rotates **180°** when the item is open; color → blue when open
- Border: 1px rule; commerce radius on outer group or per item
- Body: ink-2, padding 12–16px
- Only one open optional (product choice)
- `aria-expanded` / `aria-controls`
- Focus-visible gold on header button

## Icon

Lucide `ChevronDown` (or inline 24×24 stroke SVG, `currentColor`, stroke-width 2). See Showcase `#accordion`.

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid**. Header min-height ≥48px; chevron SVG stays trailing. Body padding can tighten slightly on narrow screens.

## Finalize
- [ ] Mark **Final** when used in a second product
