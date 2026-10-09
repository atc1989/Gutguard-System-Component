---
title: GutGuard Design System
aliases:
  - GutGuard CSS Design Reference
tags:
  - gutguard
  - design-system
  - css
  - ui
source: C:\Users\najee\Projects\GutGuard-Doctors-HTML
updated: 2026-08-12
---

# GutGuard design system

Team source of truth (Obsidian Sync). Visual language + finalized components for every GutGuard product.

> [!danger] Read-only for the team
> **Do not edit this vault** unless you are the owner. Details: [[00 - OWNER — Read only]]

> [!important] One design
> **Every component uses the GutGuard Doctors look.** Prototypes supply structure only.
> - **See it live** → open `Showcase/index.html` in a browser
> - **Building a system with Cursor?** → [[07 - Using the DS with Cursor]]
> - How the team **works** → [[05 - Playbook]]

## How we work

1. Drop or point at a system → scan for reusable UI (structure)
2. Map findings into [[Components/Index]] — skin with Doctors tokens (**owner** updates vault)
3. Finalize components family-by-family (Draft → Final)
4. **Before coding UI in Cursor:** follow [[07 - Using the DS with Cursor]]
5. Implement in the **product repo** with [[03 - Portable CSS Starter]]; Stitch via [[DESIGN]]

## Vault map

| Area | Open |
|---|---|
| **Ownership** | [[00 - OWNER — Read only]] |
| **Cursor / AGENTS adoption** | [[07 - Using the DS with Cursor]] · [[Templates/AGENTS-design-system]] |
| **Live visuals** | `Showcase/index.html` |
| Team process | [[05 - Playbook]] |
| Foundations | [[Foundations/README]] · [[01 - Visual Foundations]] · [[Foundations/Dialects]] · [[Foundations/Breakpoints]] |
| Components | [[Components/Index]] |
| Systems scanned | [[Systems/Doctors-HTML]] (truth) · [[Systems/Gentrep-Academy-Dashboard]] · [[Systems/GutGuard-Lifestyle]] |
| Stitch brief | [[DESIGN]] |
| Portable CSS | [[03 - Portable CSS Starter]] |
| Workflow | [[04 - Stitch Workflow]] |
| Boss drops | `Inbox/` |
| Templates for product repos | `Templates/` |
| **Engineering stack** | Sibling vault folder `GutGuard Tech Stack/` (hub: `00 - GutGuard Tech Stack.md`) |
| **Website SEO / search listing** | Sibling vault folder `GutGuard Website SEO/` (hub: `00 - GutGuard Website SEO.md`) |

## Brand character

Clinical interface + editorial premium-health tone:

- **Clinical** — clear hierarchy, restrained dividers, explicit form states, readable data
- **Editorial** — Fraunces headlines, italic annotations, thin rules
- **Premium** — bone canvas, ultramarine, muted gold, paper grain
- **Direct** — little decoration; registration/admin square; commerce softly rounded

## Dialects (one per screen)

See [[Foundations/Dialects]]. Short form:

| Dialect | Radius | Use |
|---|---:|---|
| Editorial booth | mostly `0` | Registration, verification, prize |
| Editorial marketing | soft / pill | Marketing site |
| Commerce / partner | `10–24px` | Shop, checkout, partner, orders |
| Admin | mostly `0` | Tables, tabs, ops forms |

## Core recognition cues

1. Warm bone `#F4F1EA` (not pure white)
2. Ultramarine `#0608A9` for actions / focus / emphasis
3. Fraunces + Inter Tight
4. Near-black ink `#0F0F18`
5. Muted gold `#B08D5B` sparingly
6. Fine warm rules + 3px paper grain
7. Uppercase micro-labels, strong weight, wide tracking

## Doctors scan snapshot

From [[Systems/Doctors-HTML]]:

- **No sidebar** in Doctors — shells are [[Components/Top Bar]] (shop/marketing), booth masthead, or admin hero + tabs
- Highest-value extractables live under `Components/`
- Prototypes (Academy, Lifestyle) supply structure only

## Adoption order

1. Fonts + tokens from [[01 - Visual Foundations]]
2. Canvas, type, paper texture
3. Pick one dialect
4. Implement only needed notes from [[Components/Index]]
5. Use [[03 - Portable CSS Starter]]
6. Verify hover, focus-visible, active, disabled, error, loading, reduced-motion

## Known caveats (from Doctors)

- Load Fraunces + Inter Tight explicitly
- Portable starter fills undeclared vars (`--paper`, etc.)
- Do **not** copy `userScalable: false` into new systems
- Global `button` resets require every variant to define appearance + focus
