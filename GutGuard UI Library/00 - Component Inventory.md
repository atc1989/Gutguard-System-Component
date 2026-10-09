---
title: Component Inventory — Website, Shop, Lifestyle
tags: [gutguard, ui-library, components, inventory]
created: 2026-10-08
status: done
source: D:\Users\najee\Downloads\Gutguard_Components_1\gutguard-components (captured 5 Oct 2026)
---

# Component inventory

Step 1 of the GutGuard UI Library: every one of the **79 captured parts** (Website 22 · Shop 26 · Lifestyle 20 · Landing 11) broken down into reusable pieces.

- **Part ids** (`w-nav`, `s-chips`, …) are anchors in `gutguard-components/pages/*.html`. Open e.g. `pages/shop.html#s-chips` to see the real part on phone and desktop.
- **Tier**: *Primitive* = smallest piece · *Component* = built from primitives · *Shell* = page frame · *Pattern* = GutGuard-specific, built from components.
- **Also in DS** = the closest note in [[GutGuard Design System/Components/Index|the existing design system]], for reference only. This library is kept separate.
- Target build: **Next.js + Tailwind**, with the tokens below mapped into the Tailwind theme.

**Result: 43 library items (12 primitives · 16 components · 3 shell · 4 overlays/states · 8 patterns) + 11 page sections that stay page-specific.** All 79 parts are accounted for.

---

## A. Foundations (tokens → Tailwind theme)

| Token | Value | Notes |
|---|---|---|
| `bone` / `bone-soft` / `bone-deep` | `#F4F1EA` / `#EBE7DE` / `#DDD7C8` | Page background family |
| `paper` | `#FCFAF5` | Cards, sheets |
| `ink` | **`#0F0F18` (site) vs `#141019` (Lifestyle)** | ⚠ conflict, pick one |
| `ink-2` / `ink-3` / `ink-4` | `#3A3A48` / `#6B6B7A` / `#A0A0AE` | Text steps |
| `rule` / `rule-soft` | `#D8D2C2` / `#E5E0D2` | Borders |
| `blue` / `blue-press` / `blue-deep` | `#0608A9` / `#04067A` / `#03044F` | Primary |
| `gold` / `gold-soft` / `gold-pale` / `gold-text` | `#B08D5B` / `#C9AC7E` / `#E8DCC4` / `#7E6035` | Accent, focus ring, E-Points |
| `heat` / `heat-text` / `heat-brick` | `#FF5E3A` / `#B5431F` / `#BF4A2B` | Inflammation readouts, warnings |
| `recovery` / `recovery-deep` | `#2F86C9` / `#1E6FB8` | Improvement readouts |
| Fonts | Fraunces (serif display, italic `em` accent) · Inter Tight (UI) · IBM Plex Mono (eyebrows) | Google Fonts |
| Radius | `sm 10` · `md 14` · `card 16` · `lg 24` · `pill 999` | `16` is Lifestyle-only today |
| Focus | 3px `gold` outline, 3px offset | Both systems |

---

## B. Primitives (12)

| # | Component | Variants / slots | Source classes | Found in | Also in DS |
|---|---|---|---|---|---|
| 1 | `Button` | primary · ghost (ring icon) · text-link · small (`soft`) · trailing arrow · price suffix | `.btn-primary` `.btn-ghost` `.nav-cta` `.tb-btn` `.bb-cta` `.slw-buy` `.co-paybtn` · `.co-link` `.sl-free` `.bb-skip` `.sheet-login` · Lifestyle `button.tap` `.lw-done` | w-hero-actions, w-offer, w-trialband, s-bar, s-card, s-free, s-paybtn, s-done, g-cta, l-firststep, g-first | Button |
| 2 | `IconButton` | plain · with count badge | `.burger` `.nav-back` `.sl-cart` (+`.n`) `.lw-icon` `.lw-cam` sheet close | w-nav, s-top, l-nav, l-dose-next | Icon Button |
| 3 | `Badge` | neutral · blue · gold · status dot (ok / slipping / stopped) | `.bs-beta` `.mh-beta` `.soon-badge` `.tag` `.ctag` `.tfree` `.save` · "ACTIVE", "NEW BUYERS" · team status `i` dot | w-hero, w-miage, w-doors, s-chips, s-watch, l-plan, g-offer, l-team | Badge |
| 4 | `Eyebrow` | mono label · numbered | `.eyebrow` `.tb-eyebrow` `.soh-eyebrow` `.co-grp` · Lifestyle `.g-m` | w-hero, w-trialband, s-co, l-plan | Section Label |
| 5 | `Price` | amount + caption · inline | `.tb-price` `.bb-price` (`.bb-amt` `.bb-sub`) `.tp` · Lifestyle `span.ant` | w-offer, w-trialband, s-watch, l-firststep, g-first | — |
| 6 | `Avatar` | initials | `.review-av` · Lifestyle `span.g-m`/`span.osw` initials | w-review, l-family, g-sponsor, l-team | Avatar |
| 7 | `PointsPill` | number + label · as button ("Log in") | `.lw-pts` | l-nav, g-nav | — |
| 8 | `ProgressBar` | thin bar · with label ("Night 3 of 5", "Day 4 of 90") · heat fill | `.bs-track` `.bs-fill` · Lifestyle inline | l-watch, l-story, w-hero | — |
| 9 | `Stepper` | − value + | `.lw-step` | l-settings | Quantity Stepper |
| 10 | `TextField` | label · input · help text · two-up row · tel / email / time | `.co-f` `.co-two` `.fe` `.co-inline` · Lifestyle `label.osw + input`, `.lw-time` | s-mobile, s-field, g-signup, g-login, l-settings | Form Field |
| 11 | `Checkbox` | consent line with links | `label.inr > input[type=checkbox]` | g-signup | — |
| 12 | `CodeInput` | 6-digit code | Lifestyle inline (⚠ check markup at build) | g-code, g-login | — |

## C. Components (16)

| # | Component | Variants / slots | Source classes | Found in | Also in DS |
|---|---|---|---|---|---|
| 13 | `SegmentedControl` | 2 or 3 options · radiogroup | `.sl-toggle.x3` `.co-for` `.lw-seg(.x3)` | s-toggle, s-for, l-settings | Segmented Control |
| 14 | `Tabs` | pills + scroll-spy (`sectabs`) · underline sticky (`lw-tabs`) | `.sectabs` `.sectab` · `.lw-tabs` `.lw-tab` | w-sectabs, l-tabs | Tabs |
| 15 | `OptionCard` | compact · wide (with badge) · radio (payment) | `.sl-topt` `.sl-wide-opt` · `.co-pay` (`.rd`) | s-watch, s-trials, s-pays | — |
| 16 | `ChoiceChip` | with top tag ("Best rate") · check mark · name / saving / duration | `.sl-chip` (`.ctag` `.cmk` `.cn` `.cpc.sv` `.cd`) | s-chips, s-sub | — |
| 17 | `Combobox` | type → listbox of suggestions | `.co-city` `.co-sugg[role=listbox]` | s-city | Search Field |
| 18 | `StatGroup` | editorial (big serif) · highlight-first · boxed 3-up · trust tiles | `.stat-row` · `.sl-stats` (`.hl`) · `.lw-stats` · `.trust-grid` `.sl-proof-grid` | w-stats, s-stats, s-sub-stats, l-stats, l-story, l-team, w-trust, s-proof | Card (stat) |
| 19 | `TrustLine` | icon + short text, inline | `.sl-trustline` `.sl-trust2` | s-trustline, s-basket | — |
| 20 | `Note` | icon + text info line | `.sl-note` `.co-cardnote` `.sl-eta` | s-card, s-co, s-basket | Alert |
| 21 | `LineItem` | basket (thumb, name, desc, remove, price) · numbered step (`01`) | `.sl-line` (`.lc` `.ln` `.ld` `.sl-rm` `.sl-lp` `.nx`) | s-basket, s-co, s-done | — |
| 22 | `OrderTotals` | rows + big total | `.co-tots` (`.big`) `.sl-ship` `.sl-tot` | s-tots, s-basket | Definition List |
| 23 | `ListRow` | title + sub + chevron · with trailing action ("Redeem") | Lifestyle `button.tap` / `a.tap` rows | l-plan-sheet, l-points, g-first, l-plan | — |
| 24 | `IconRow` | icon + title + text (benefit / feature) | Lifestyle inline · `.sl-line` icon rows | g-get, l-guard, s-inside | — |
| 25 | `Card` + `CardGrid` | slots: tag · title · meta · body · rows · footer | `.symptom` `.about-card` `.phase-card` `.ms-card` `.dose-card` (`.dc-row`) · Lifestyle panels · grids `.grid3` `.about-grid` `.phase-cards` `.dose-cards` | w-symptoms, w-about, w-phases, w-dose, w-miage, l-plan, g-offer | Card |
| 26 | `Quote` | quote + avatar + name + place | `figure.review` (`.review-q` `.review-who`) | w-review | — |
| 27 | `SectionHeading` | number + label · heading with italic accent · lead | `.sec-label` (`.num`) `h2.sec` `.sec-sub` | w-sechead | Section Label |
| 28 | `Timeline` | checkpoints (Day 30/60/90) · numbered steps (I, II, III) | `.timeline` `.tl-item` · `.steps` `.step-row` · `.co-next` | w-timeline, w-proto, s-done | Requirement Timeline |

## D. Shell (3)

| # | Component | Variants / slots | Source classes | Found in | Also in DS |
|---|---|---|---|---|---|
| 29 | `TopBar` | site (back, brand, page name, links, Log in, CTA, burger) · app (brand, "/ Lifestyle", links, right slot) | `nav.nav` (`.nav-*`) · `header.lw-nav` (`.lw-*`) | w-nav, l-nav, g-nav | Top Bar |
| 30 | `Footer` | site map columns ("You are here") · brand · legal | `footer` `.sitemap` `.smap-*` `.foot-*` | w-footer | — |
| 31 | `BottomBar` | offer (info + price + skip + CTA) · single button · pay button | `.buybar` · `.sl-bar` · `.co-paywrap` | w-offer, s-bar, s-paybtn | Bottom Bar |

## E. Overlays and states (part of components, listed apart for clarity)

| # | Component | Variants / slots | Source classes | Found in | Also in DS |
|---|---|---|---|---|---|
| 32 | `Sheet` | bottom sheet (phone) · side/centre (desktop) · grip · header with close · scrim | `.sl-sheet` `.sl-scrim` `.sl-grip` `.sl-sh-h` · Lifestyle `.ov-c > .up` `.grab` | s-inside, s-basket, s-co, s-done, l-plan-sheet, l-settings, l-points, l-card | Drawer / Modal |
| 33 | `MobileMenu` | numbered links · CTA · login link | `.sheet#mobile-menu` | w-menu | — |
| 34 | `EmptyState` | inline ("Your basket is empty.") · coming-soon box | `.sl-empty` · `.doors-soon` | s-basket, w-doors | Empty State |
| 35 | `SuccessState` | icon + title + text + content + actions | `.co-ok` | s-done | — |

## F. Patterns — GutGuard-specific (8)

| # | Pattern | Built from | Source | Found in |
|---|---|---|---|---|
| 36 | `MemberCard` | full card · flip to QR · mini (`.mini-card`) | `MemberCard` (LifestyleMember.jsx:308) · `.mini-card` | l-bigcard, l-card-desk, l-card, g-card, s-minicard |
| 37 | `DoseRow` | states next / done / off · settings (Stepper + time) | `.lw-dose` (`.next` `.done` `.lw-set` `.off`) | l-dose-next, l-dose-done, l-settings |
| 38 | `OfferCard` | website band · Lifestyle box | `.trialband` · Lifestyle offer boxes | w-trialband, g-hero, g-offer, l-firststep |
| 39 | `PersonRow` | Avatar + name + meta + trailing (Manage › / status) | Lifestyle inline | l-family, l-team, g-sponsor |
| 40 | `AdherenceCalendar` | month grid · dose dots (half/full) · photo mark · legend | `.lw-cal` `.lw-legend` | l-story |
| 41 | `NutritionFacts` | label panel | `.fx` | s-facts, s-inside |
| 42 | `StepProgress` | 3-step sign-up bar ("1 · Card") | Lifestyle inline | g-signup, g-code, g-first |
| 43 | `ProductHeader` + `BuyPanel` | product name + tagline + cart · desktop buy card (SegmentedControl + OptionCard + ChoiceChip + StatGroup + TrustLine + Button) | `.sl-top` `.sl-prow` · `.slw-card` | s-top, s-card |

## G. Page sections

Built *from* library pieces, each used on one page. Built 8 Oct 2026 as section components (`components/sections/`, notes in `Sections/`) and full screens in the showcase; see [[README]].

| Section | Part | Uses |
|---|---|---|
| Home hero + Blood Scan readout | w-hero | Eyebrow, Button, Badge, ProgressBar |
| MiAge block | w-miage | Badge, Card |
| 90-day trajectory chart | w-traj | (custom SVG chart) |
| Story of Hope | w-soh | Eyebrow, Quote-like, Timeline |
| Product + three steps | w-proto | Timeline (steps) |
| Lifestyle greeting column | l-greet | MemberCard, PointsPill, Card, PersonRow |
| Business tools | l-tools | IconButton |
| My Story tab | l-story | ProgressBar, StatGroup, AdherenceCalendar, Button |
| My Team tab | l-team | StatGroup, PersonRow, Badge |
| Sign-up / code / first step / log-in screens | g-signup, g-code, g-first, g-login | StepProgress, TextField, Checkbox, CodeInput, Button, ListRow |
| Checkout screen | s-co | Sheet, LineItem, SegmentedControl, TextField, Combobox, OptionCard, Note, OrderTotals, BottomBar |

---

## Decisions (agreed 8 Oct 2026)

1. **Ink colour:** `#0F0F18` (website/shop). Lifestyle's `#141019` is folded into it.
2. **Breakpoints:** mobile-first `sm 520 · md 900 · lg 1080 · xl 1440`, replacing ~30 `max-width` queries.
3. **One Button** with `size` (`lg` = full-width phone / Lifestyle button) instead of two button systems.
4. **Prototype leftovers** (`#1A2740` input text, `#2F7FD6` caret) normalised to `ink` / `blue`.
5. **Demo content** stays in examples, never inside components.
6. **Tailwind** is used for this library, and since 8 Oct 2026 the Tech Stack allows it on new apps through [[06 - Tailwind Bridge]]. Existing portable-CSS apps (Website, Lifestyle, Academy) keep portable CSS unless a migration is approved.

Added while building: the site's `slate` colours (dark sections) and the member card's own blue and gold (`card-blue*`, `card-gold`) became tokens, so those parts match the original.

## Built

- One note per component in `Components/`; index in [[README]].
- Code and showcase: `D:\Users\najee\Downloads\Gutguard_Components_1\gutguard-ui`.
