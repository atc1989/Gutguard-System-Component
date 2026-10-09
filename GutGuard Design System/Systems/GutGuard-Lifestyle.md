---
title: System — GutGuard Lifestyle
tags: [gutguard, design-system, systems, lifestyle, prototype]
source: d:\Users\najee\Downloads\GutguardLifestyle.html
scanned: 2026-08-12
updated: 2026-08-12
status: prototype-harvest
---

# System: GutGuard Lifestyle

**Prototype only.** Extract structure and component candidates; **skin everything with** [[Systems/Doctors-HTML]] / GutGuard DS (bone, ultramarine, Fraunces, Inter Tight). Do not adopt the prototype’s cool paper, royal blue, Anton/Sora/Playfair stack.

Same rule as [[Systems/Gentrep-Academy-Dashboard]].

Dialect for restyle: **commerce** (member app) with optional editorial accents on landing / ceremonial card.

## What it is

Member lifestyle SPA:

1. **Ginhawa funnel** — landing → register → invite / door card → nearly free → enter app  
2. **Member app** — My Health · My Team · My Story  
3. Overlays — BASE Activation · GEMA teaser · GG-VERSE · Settings · Order · Stories · QR

## Shell (structure)

| Chrome | Present? | Map to GG component |
|---|---|---|
| Fixed Top Bar | **No** | — (in-page header ≈ [[Components/Masthead]]) |
| Sidebar | **Yes** desktop ≥900px (`.gg-sidebar`, ~262px) | [[Components/Sidebar]] |
| Bottom Bar | **Yes** mobile (`.gg-foot` — “Order now” CTA) | [[Components/Bottom Bar]] |
| Bottom tab bar | **No** | Primary mobile IA = [[Components/Segmented Control]] (`.gg-tab`) |

## Component harvest → Doctors / GG map

Prefer existing notes. Prototype class names are evidence only.

| Pattern | Prototype evidence | GG component | Notes for finalize |
|---|---|---|---|
| Sidebar | `.gg-sidebar` brand + nav + supply footer | [[Components/Sidebar]] | Slots: brand, nav (badges), secondary links, reorder CTA |
| Bottom Bar | `.gg-foot` / `.gg-foot-inner` | [[Components/Bottom Bar]] | Same as Academy “Next”; label = Order |
| Mast / in-page header | Sponsor + product name + bell | [[Components/Masthead]] | Not a Top Bar |
| Segmented tabs | `.gg-tab` (Health / Team / Story) | [[Components/Segmented Control]] | Pill track under card |
| Button / CTA | `.g-press` `.g-cta` `.tap` | [[Components/Button]] | Commerce primary; drop pulse/shine in core kit |
| Big input | `.g-bigin` (60px, 14px radius) | [[Components/Form Field]] | Large commerce boxed variant |
| Card / panel | paper + edge + radius 14 | [[Components/Card]] | Commerce card |
| Stat numeral tile | large number + caption | [[Components/Card]] (trust/stat) | Already in Card note |
| Sheet / drawer | `.g-sheet` + grab | [[Components/Drawer]] / [[Components/Modal]] | Bottom sheet mobile |
| Centered modal | Door QR “show to staff” | [[Components/Modal]] | |
| Toast | `.t-drop` + bottom pill | [[Components/Toast]] | Optional drop variant |
| Badge / count | amber chips on tabs / bell | [[Components/Badge]] | |
| Progress bar / day-of-N | fill rail | [[Components/Progress Rail]] | Extend for % / day progress |
| Empty / locked | My Team lock | [[Components/Empty State]] | Locked-feature copy |
| Requirement steps | BASE checklist | [[Components/Requirement Timeline]] | From Academy harvest |
| Event / book row | BASE “Book this” | [[Components/Event Row]] | |
| QR | seed QR + white pad | [[Components/QR Block]] | |
| Alert / notice | check-in / success bands | [[Components/Alert]] | |
| Section micro-label | uppercase captions | [[Components/Section Label]] | |
| Dosing stepper | − / + caps | [[Components/Quantity Stepper]] | Doctors already has stepper |
| Roster row | team member + status | [[Components/Card]] + [[Components/Badge]] | |

## Product-specific (do not put in core kit)

- Flip door / member card (`.g-stage` `.g-3d` `.g-spin` `.g-face`)
- Confetti / FX (`.fx-fall` `.fx-burst` `.fx-twinkle`)
- Welcome full-screen overlay
- Stories of Hope feed + share wizard
- Dose calendar + camera proof capture
- Points economy UI copy
- GEMA teaser content (real training UI = Academy)
- Demo mode strip

## Prototype tokens (remap reference only)

| Prototype | GutGuard |
|---|---|
| field `#eef2f7` | bone `#F4F1EA` |
| royal `#00249C` / blue `#2f7fd6` | ultramarine `#0608A9` |
| navy / ink | ink `#0F0F18` |
| amber `#f5b716` | gold `#B08D5B` (sparing) |
| Inter / Sora / Anton / Playfair / Fredoka | Inter Tight + Fraunces |
| Focus blue | gold focus-visible (buttons) / blue field halo |

## Screens checklist (for Stitch / implementation)

- [ ] Landing (gift / plain)
- [ ] Register (name + mobile)
- [ ] Door card front / back (QR)
- [ ] Member — My Health
- [ ] Member — My Team
- [ ] Member — My Story
- [ ] Sheets: Order, Settings, BASE, GEMA, GG-VERSE, Story share

## Related

- Visual source of truth: [[Systems/Doctors-HTML]]
- Parallel prototype harvest: [[Systems/Gentrep-Academy-Dashboard]]
- Catalog: [[Components/Index]]
