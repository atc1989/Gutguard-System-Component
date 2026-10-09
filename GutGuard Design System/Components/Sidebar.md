---
title: Sidebar
tags: [gutguard, design-system, components, shell]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.side, .who, .side-nav, .side-rank, .side-next)
---

# Sidebar

Left rail for desktop app shells. **First appeared in** [[Systems/Gentrep-Academy-Dashboard]]. Also used in [[Systems/GutGuard-Lifestyle]] (`.gg-sidebar`). Doctors has none.

## Behavior

- Hidden on small screens; visible from desktop cut
- Desktop: sticky column ~**262–280px**
- Pairs with mobile [[Components/Bottom Bar]] — hide bottom bar when sidebar is visible

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` | **Hidden** — IA moves to page content / masthead / bottom CTA |
| `≥ 900px` | **Visible** sticky rail ~262–280px; do not show Bottom Bar for the same primary CTA |

Nav labels may truncate with ellipsis; do not shrink the rail below ~240px.

## Anatomy slots (GG)

1. Brand (Fraunces / Inter Tight — not prototype Playfair/Sora)
2. Primary nav rows (optional [[Components/Badge]] counts)
3. Secondary links (settings, programs)
4. Footer CTA card (supply left / reorder / “do this next”)

## Visual rules (Doctors / GG — always)

- Bone or paper surface; 1px rule separators
- Active row: pale blue wash or ink/blue text — **ultramarine**, not prototype royal
- Radius: commerce ~12–14px
- Focus-visible: gold outline per foundations

## Seen in

| System | Class | Width |
|---|---|---|
| Academy | `.side` | 280px |
| Lifestyle | `.gg-sidebar` | ~262px |

## Do / don’t

- Do use for persistent IA / rank or section switching on wide screens
- Don’t show sidebar and bottom bar at the same time for the same CTA (Academy hides `.foot` ≥900px)
- Don’t confuse with admin hero tabs ([[Components/Admin Shell]])

## Finalize

- [ ] Lock active-row treatment to GG blue/ink
- [ ] Define generic slots: brand · identity · nav · footer CTA
- [ ] Mark **Final**
