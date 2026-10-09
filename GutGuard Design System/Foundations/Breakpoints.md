---
title: Breakpoints
aliases:
  - Responsive
  - Layout breakpoints
tags: [gutguard, design-system, foundations, responsive]
updated: 2026-08-14
---

# Breakpoints

Shared responsive scale for GutGuard products. Component notes reference this page under **Responsive**.

## Canonical scale

| Token | Width | Role |
|---|---:|---|
| `--bp-mobile` | `< 900px` | Default / phone / narrow |
| `--bp-desktop` | `≥ 900px` | App shell with sidebar; centered dialogs |

**Primary cut:** **900px** — matches Academy + Lifestyle (`≥900px` sidebar, hide bottom bar).

Optional denser cuts (product choice — document in that repo):

| Token | Width | When |
|---|---:|---|
| `--bp-sm` | `< 600px` | Very narrow; stack dense admin toolbars |
| `--bp-lg` | `≥ 1200px` | Wide marketing / multi-column content |

Do **not** invent a third shell breakpoint per product without updating this note.

## Shell pairing rule

| Viewport | Show | Hide |
|---|---|---|
| `< 900px` | [[Components/Bottom Bar]] (if the product uses a sticky CTA) · page [[Components/Masthead]] | [[Components/Sidebar]] |
| `≥ 900px` | [[Components/Sidebar]] | [[Components/Bottom Bar]] for the same primary CTA |

[[Components/Top Bar]] (marketing/shop) stays available at all widths; collapse nav into a sheet/menu below desktop as needed.

## Content width

| Context | Guidance |
|---|---|
| Mobile main column | max-width ~**440px** centered (Academy-style) or fluid with page padding |
| Desktop shell content | Fluid inside shell; outer shell max ~**1240–1320px** |
| Dialog / modal | max-width ~**480–560px**; see overlays |
| Form fields / buttons | Fluid width of container unless explicitly fixed |

## Touch & type

- Interactive targets **≥ 44×44px** on mobile (dense admin 36px only where already documented)
- Do not shrink type below readable Inter Tight sizes to “fit” mobile — stack or scroll instead
- Prefer stacking grids (`1fr` → `1fr 1fr`) at `--bp-desktop`, not earlier, unless the component note says otherwise

## CSS pattern

```css
/* Mobile first */
.gg-sidebar { display: none; }
.gg-bottom-bar { display: block; }

@media (min-width: 900px) {
  .gg-sidebar { display: flex; }
  .gg-bottom-bar { display: none; }
}
```

## Prefers reduced motion

Treat `prefers-reduced-motion: reduce` as a required responsive concern: shorten or remove layout transitions (drawers, accordion chevron, switch thumb). See [[01 - Visual Foundations]].

## Component notes

Every component should include a **Responsive** section that either:

1. States specific behavior at `< 900px` / `≥ 900px`, or  
2. Says **container-fluid** — no component breakpoint; inherits shell/page layout

## Related

[[Foundations/README]] · [[Foundations/Dialects]] · [[Components/Sidebar]] · [[Components/Bottom Bar]] · [[Components/Index]]
