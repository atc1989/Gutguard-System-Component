---
title: GutGuard Design System Playbook
aliases:
  - Playbook
  - DS Playbook
tags: [gutguard, design-system, playbook, team]
updated: 2026-08-12
---

# GutGuard Design System — Playbook

One visual language for every product. One vault for the whole team (Obsidian Sync).

> Looking for **how components look**? → open `Showcase/index.html`
> **Using Cursor on a new system?** → [[07 - Using the DS with Cursor]]
> **Who may edit this vault?** → [[00 - OWNER — Read only]]
> This note is the **team operating playbook** (process, remap, QA).

---

## The rule (read this first)

**Yes — every component uses the GutGuard Doctors design.**

| Layer | Source of truth | What prototypes are for |
|---|---|---|
| Look & feel | [[Systems/Doctors-HTML]] + [[01 - Visual Foundations]] | **Not** the look |
| Component skins | [[Components/Index]] + [[03 - Portable CSS Starter]] | Structure / IA / flows only |
| Compact Stitch brief | [[DESIGN]] | Generate on-brand screens |

Academy, Lifestyle, and future boss HTML files are **prototypes**. Extract *what* the UI needs (sidebar, bottom bar, sheets, cards). Never copy their cool paper, royal blue, Anton/Sora/Playfair, or bright amber into the DS.

If a screen could be mistaken for a different brand after removing the logo, it is wrong.

---

## Non-negotiable recognition cues

Carry these into every system:

1. Warm bone `#F4F1EA` canvas (not pure white, not cool grey paper)
2. Ultramarine `#0608A9` for actions, focus, emphasis
3. Fraunces (display) + Inter Tight (UI)
4. Near-black ink `#0F0F18`
5. Muted gold `#B08D5B` sparingly
6. Fine warm rules + subtle 3px paper grain
7. Uppercase micro-labels, strong weight, wide tracking

Full tokens: [[01 - Visual Foundations]]. Dialects: [[Foundations/Dialects]].

---

## Dialects (one per screen)

| Dialect | Radius | Use |
|---|---:|---|
| Editorial booth | mostly `0` | Registration, verification, prize |
| Editorial marketing | soft / pill | Marketing site |
| Commerce / partner | `10–24px` | Shop, member apps, Lifestyle, Academy restyles |
| Admin | mostly `0` | Ops tables, admin tabs, dense forms |

Do not mix radius policies on one screen. Colors and type hierarchy stay shared.

---

## How the team uses this vault

```
Prototype / boss HTML
        │
        ▼
   Scan → Systems/<Name>.md   (structure harvest)
        │
        ▼
   Map → Components/*         (existing note or new candidate)
        │
        ▼
   Skin → Doctors tokens      (always)
        │
        ▼
   Ship → gg-* CSS / Stitch / product code
```

### Roles

| Who | Does |
|---|---|
| Anyone dropping a prototype | Put file in `Inbox/` or paste path in Cursor |
| Agent / designer | Run harvest → update Systems + Components |
| Implementer | Read component note + foundations; use portable CSS |
| Stitch | Upload [[DESIGN]]; dialect stated in prompt |

---

## Playbook steps

### A. New prototype arrives

1. Confirm it is **structure only** (not a new brand).
2. Scan screens, shell, and repeating UI.
3. Write / update `Systems/<Product>.md` with:
   - Shell table (Top Bar / Sidebar / Bottom Bar — yes/no)
   - Harvest table mapping → existing [[Components/Index]] notes
   - Product-only list (wheel, flip card, confetti — keep out of core kit)
   - Remap cheat-sheet (prototype token → GG token)
4. Mark the system note `status: prototype-harvest`.

### B. Identify a component

Ask: *Would another GutGuard product reuse this shape?*

| Answer | Action |
|---|---|
| Yes, already in Index | Add “Seen in” row on that component note |
| Yes, new shape | Create `Components/<Name>.md` as **Draft**; link from Index |
| No, one-off brand moment | List under system “product-specific” only |

### C. Finalize a component (Draft → Final)

On the component note, lock:

- [ ] Variants + which dialect each belongs to
- [ ] States: default, hover, focus-visible, active, disabled, loading, error (as relevant)
- [ ] Anatomy (slots / parts)
- [ ] Doctors-sourced measurements (not prototype hex/fonts)
- [ ] Do / don’t
- [ ] Portable `gg-*` mapping (or TODO pointing at [[03 - Portable CSS Starter]])
- [ ] Status → **Final**

Suggested finalize order:

1. Foundations (already largely locked)
2. Button → Form Field → Segmented Control / Tabs
3. Card → Badge → Alert → Toast
4. Top Bar · Sidebar · Bottom Bar · Masthead · Admin Shell
5. Modal / Drawer → Table → Definition List → QR
6. Product patterns (Rank Ladder, Timeline, etc.) only if a second system needs them

### D. Implement in a product

1. Pick **one dialect** for the screen.
2. Load Fraunces + Inter Tight explicitly.
3. Apply tokens from foundations / portable CSS.
4. Use only finalized (or explicitly Draft-approved) component notes.
5. Remap any leftover prototype styles before merge.
6. QA with the checklist below.

### E. Stitch generation

Follow [[04 - Stitch Workflow]].

Prompt essentials:

- Design system: `DESIGN.md` + dialect
- Preserve boss **structure/content**
- Force bone / ultramarine / Fraunces / Inter Tight
- No purple SaaS, no cool grey field, no Anton/Sora as brand type

---

## Remap table (prototypes → Doctors)

Use whenever harvesting Academy, Lifestyle, or similar.

| Prototype tendency | GutGuard |
|---|---|
| Cool paper `#eef2f7` | Bone `#F4F1EA` |
| White cards as default canvas | Paper `#FCFAF5` on bone |
| Royal / sky blue `#00249C` / `#2569b8` | Ultramarine `#0608A9` |
| Navy as action fill | Ink for dark fills; blue for primary actions |
| Bright amber `#f5b716` everywhere | Muted gold `#B08D5B` sparingly; don’t overload |
| Anton / Sora / Playfair / Fredoka | Fraunces + Inter Tight |
| Blue focus rings on buttons | Gold 3px focus-visible (fields may use blue halo) |

---

## Shell cheat-sheet

| Chrome | Doctors | Academy (proto) | Lifestyle (proto) | GG component |
|---|---|---|---|---|
| Top Bar | Shop / marketing yes; admin no | No | No | [[Components/Top Bar]] |
| Sidebar | No | Desktop yes | Desktop yes | [[Components/Sidebar]] |
| Bottom Bar | No (shop uses other CTAs) | Mobile “Next” | Mobile “Order” | [[Components/Bottom Bar]] |
| Masthead | Booth yes | Page mast | In-page header | [[Components/Masthead]] |
| Admin tabs | Yes | — | — | [[Components/Tabs]] + [[Components/Admin Shell]] |

When implementing Academy/Lifestyle: keep their **IA**, paint with Doctors chrome specs.

---

## QA checklist (every screen)

- [ ] Bone canvas + paper grain (or intentional dark ceremonial — rare)
- [ ] One dialect only
- [ ] Fraunces for display; Inter Tight for UI
- [ ] Primary actions ultramarine (or ink→blue hover on editorial primary)
- [ ] Focus-visible present; 44px targets
- [ ] No prototype fonts or cool-grey field left behind
- [ ] States not color-only (selected / error / disabled)
- [ ] Reduced-motion honored
- [ ] Component matches its vault note (or note updated first)

---

## What not to do

- Don’t create a second “Academy DS” or “Lifestyle DS”
- Don’t paste prototype hex into `Components/` as canonical values
- Don’t mix editorial square and commerce soft radius on one view
- Don’t use purple gradients, generic SaaS indigo, or pure-white default canvas
- Don’t invent a Top Bar where the product only has a mast + sidebar
- Don’t promote confetti, flip-cards, or wheels into the core kit unless a second product needs them

---

## Vault map (quick open)

| Need | Open |
|---|---|
| **How components look** | `Showcase/index.html` |
| Cursor / AGENTS gate | [[07 - Using the DS with Cursor]] |
| Ownership (read-only) | [[00 - OWNER — Read only]] |
| This process playbook | [[05 - Playbook]] |
| Overview | [[00 - GutGuard Design System]] |
| Tokens | [[01 - Visual Foundations]] |
| Dialects | [[Foundations/Dialects]] |
| Components | [[Components/Index]] |
| Doctors truth | [[Systems/Doctors-HTML]] |
| CSS to copy | [[03 - Portable CSS Starter]] |
| Stitch | [[DESIGN]] · [[04 - Stitch Workflow]] |

---

## One-line summary

**Prototypes tell us what to build; Doctors tells us how it should look; the vault is how the team stays aligned.**
