# GutGuard Design System — Compiled (Markdown only)

All `.md` notes from the `GutGuard Design System` vault, concatenated verbatim in folder order. Each section starts with `<!-- FILE: path -->` and a heading with its source path. HTML, MDC and image files are excluded.

## Contents

1. `00 - GutGuard Design System.md`
2. `00 - OWNER — Read only.md`
3. `01 - Visual Foundations.md`
4. `03 - Portable CSS Starter.md`
5. `04 - Stitch Workflow.md`
6. `05 - Playbook.md`
7. `07 - Using the DS with Cursor.md`
8. `DESIGN.md`
9. `Foundations/README.md`
10. `Foundations/Breakpoints.md`
11. `Foundations/Dialects.md`
12. `Components/Index.md`
13. `Components/Accordion.md`
14. `Components/Admin Shell.md`
15. `Components/Alert.md`
16. `Components/Avatar.md`
17. `Components/Badge.md`
18. `Components/Bottom Bar.md`
19. `Components/Breadcrumbs.md`
20. `Components/Button.md`
21. `Components/Card.md`
22. `Components/Certificate.md`
23. `Components/Chat Link Row.md`
24. `Components/Date Picker.md`
25. `Components/Definition List.md`
26. `Components/Dialog.md`
27. `Components/Drawer.md`
28. `Components/Dropdown Menu.md`
29. `Components/Empty State.md`
30. `Components/Event Row.md`
31. `Components/File Attachment.md`
32. `Components/Form Field.md`
33. `Components/Icon Button.md`
34. `Components/Lang Toggle.md`
35. `Components/Masthead.md`
36. `Components/Modal.md`
37. `Components/Notification Bell.md`
38. `Components/Pagination.md`
39. `Components/Progress Rail.md`
40. `Components/QR Block.md`
41. `Components/Quantity Stepper.md`
42. `Components/Rank Ladder.md`
43. `Components/Rank Plate.md`
44. `Components/Requirement Timeline.md`
45. `Components/Search Field.md`
46. `Components/Section Label.md`
47. `Components/Segmented Control.md`
48. `Components/Sidebar.md`
49. `Components/Skeleton.md`
50. `Components/Spinner.md`
51. `Components/Switch.md`
52. `Components/Table.md`
53. `Components/Tabs.md`
54. `Components/Task Item.md`
55. `Components/Toast.md`
56. `Components/Tooltip.md`
57. `Components/Top Bar.md`
58. `Systems/README.md`
59. `Systems/Doctors-HTML.md`
60. `Systems/Gentrep-Academy-Dashboard.md`
61. `Systems/GutGuard-Lifestyle.md`
62. `Templates/AGENTS-design-system.md`
63. `Inbox/README.md`
64. `Inbox/gentrep-academy-dashboard/NOTES.md`


---

<!-- FILE: 00 - GutGuard Design System.md -->
# 00 - GutGuard Design System.md

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


---

<!-- FILE: 00 - OWNER — Read only.md -->
# 00 - OWNER — Read only.md

---
title: Ownership — read only for the team
aliases:
  - DO NOT EDIT
  - Owner lock
tags: [gutguard, design-system, governance]
updated: 2026-08-12
---

# Ownership — do not edit this vault

> [!danger] Read-only for everyone except the owner
> This **GutGuard Design System** folder is the shared source of truth via Obsidian Sync.
> **Only the designated owner may change these notes** (and the Showcase HTML).
> Everyone else: **read, copy templates into your product repos, implement UI — do not edit the vault.**

## Owner

| Field | Value |
|---|---|
| Owner | Najee |
| Authoritative machine | Najee’s PC (this vault path under Najee’s user profile) |
| Contact | Ask Najee for DS changes |

## What teammates may do

- Read all notes and open `Showcase/index.html`
- Copy `Templates/` into their project `AGENTS.md` / `.cursor/rules/`
- Use the DS when building products
- Suggest changes in chat / Linear / Slack — **owner applies them here**

## What teammates must not do

- Edit, rename, or delete notes in this folder
- “Improve” tokens, components, or the showcase on their machine (Sync would overwrite the team copy)
- Point Cursor at this vault with write intent (`Write` / `StrReplace` / delete)

## For Cursor agents (any machine)

If the workspace includes this vault path:

1. **READ only** — never modify files under `GutGuard Design System/`
2. Implement UI in the **product repo**, not in Obsidian
3. If a DS change is needed, tell the user: *“Ask the design-system owner (Najee) to update the vault.”*

## Why Sync can’t lock it for real

Obsidian Sync is two-way. This is a **team rule + Cursor rule**, not a filesystem permission. Discipline + the templates below keep the vault stable.

Owner Cursor rule snippet lives in [[Templates/gutguard-design-system]] — includes “do not write to the vault.”


---

<!-- FILE: 01 - Visual Foundations.md -->
# 01 - Visual Foundations.md

---
title: GutGuard Visual Foundations
tags: [gutguard, design-system, css, tokens]
updated: 2026-08-14
---

# Visual foundations

Layout breakpoints and shell pairing (900px) live in [[Foundations/Breakpoints]]. Every component note has a **Responsive** section that points there.

## Color system

### Brand and surface tokens

| Token | Value | Role | Usage guidance |
|---|---|---|---|
| `--bone` | `#F4F1EA` | Primary canvas | Default body background; also text on dark buttons and panels |
| `--bone-soft` | `#EBE7DE` | Inset/disabled surface | Segmented-control tracks, disabled buttons, muted bands |
| `--bone-deep` | `#DDD7C8` | Strong muted surface | Disabled filled controls and deeper warm separators |
| `--paper` | `#FCFAF5` | Raised light surface | Cards, inputs, drawers, modals; inferred from repeated literal usage |
| `--blue` | `#0608A9` | Primary brand/action | Primary actions, links, focus, selected states, emphasized words |
| `--blue-press` | `#04067A` | Pressed/hover blue | Primary action hover or active darkening |
| `--gold` | `#B08D5B` | Premium accent | Decorative copy, focus outlines, celebration, restrained labels |
| `--gold-soft` | `#C9AC7E` | Light premium accent | Dark-surface labels and ornaments |
| `--ink` | `#0F0F18` | Primary text/dark fill | Main text, dark buttons, strong borders |
| `--ink-2` | `#3A3A48` | Secondary text | Long-form copy and supporting prose |
| `--ink-3` | `#6B6B7A` | Muted text | Labels, metadata, help text, secondary controls |
| `--ink-4` | `#A0A0AE` | Quiet/disabled text | Placeholders, disabled content, inactive numbering |
| `--rule` | `#D8D2C2` | Standard divider | Borders, field rules, card outlines |
| `--rule-soft` | `#E5E0D2` | Subtle divider | Internal separators and low-emphasis boundaries |

### Supporting semantic colors

| Purpose | Value | Typical treatment |
|---|---|---|
| Error / destructive | `#B0202E` | Border and label; background `rgba(176,32,46,.06–.07)` |
| Strong error text | `#8F1824` or `#821D28` | Body copy within pale-red notices |
| Alternative error border | `#9D2430` | Partner-auth invalid field |
| Success emphasis on dark toast | `#EAFF18` | Small uppercase toast title only |
| Error emphasis on dark toast | `#FFB8C2` | Small uppercase toast title only |
| Product heat accent | `#B5431F` | Thin product-label accent; use sparingly |
| Product recovery accent | `#1E6FB8` | Thin product-label accent; use sparingly |
| Celebration gold | `#F6D59D` | Large type on a blue gradient |
| Pure white | `#FFFFFF` | QR background and special paper-like surfaces only |

### Color hierarchy

- Use **ink** for headings, values, and primary reading content.
- Use **ink-2** for explanatory copy that should still read prominently.
- Use **ink-3** for metadata, field labels, helper text, secondary navigation, and quiet buttons.
- Use **ink-4** only for placeholders, inactive marks, and disabled states; it may be too faint for small normal text.
- Reserve **blue** for interaction or deliberate emphasis. Avoid turning every heading blue.
- Reserve **gold** for premium, celebratory, or focused moments. It is an accent, not the normal action color.
- Prefer bone and paper surfaces to stark white. Pure white is exceptional.

### Background recipes

**Default paper canvas**

```css
background-color: #F4F1EA;
background-image:
  radial-gradient(circle at 1px 1px, rgba(15, 15, 24, 0.025) 1px, transparent 0);
background-size: 3px 3px;
```

The texture is extremely subtle. It should register as tactile paper, not a visible pattern. When implemented as a fixed pseudo-element, use `pointer-events: none` and keep it below content.

**Raised paper**

```css
background: #FCFAF5;
border: 1px solid #D8D2C2;
```

**Muted band**

```css
background: rgba(235, 231, 222, 0.42); /* up to .50 */
border-top: 1px solid #D8D2C2;
```

**Dark ceremonial panel**

```css
background: linear-gradient(180deg, rgba(15,15,24,.96), rgba(4,6,122,.94)), #0F0F18;
color: #F4F1EA;
```

**Celebration card**

```css
background: linear-gradient(135deg, #04067A 0%, #0608A9 45%, #0F2D9D 100%);
color: #F4F1EA;
box-shadow: 0 10px 28px rgba(4, 6, 122, 0.25);
```

## Typography

### Font families

| Token | Stack | Use |
|---|---|---|
| `--font-display` / existing `--serif` | `'Fraunces', 'Times New Roman', serif` | Headlines, large values, ledes, editorial labels, italic annotations |
| `--font-ui` / existing `--sans` | `'Inter Tight', system-ui, sans-serif` | Body copy, controls, navigation, labels, tables |
| `--font-mono` | `ui-monospace, SFMono-Regular, Menlo, Consolas, monospace` | Verification codes and machine-readable identifiers |

Recommended web loading:

```css
/* Use self-hosted files or a font provider. Load only the weights in use. */
/* Fraunces: 400 normal, 400 italic, 500, 600 */
/* Inter Tight: 400, 500, 600, 700, 800, 900 */
```

The current source asks for `font-feature-settings: 'ss01', 'cv11', 'tnum' off` on body text, with `lnum` enabled selectively for editorial numbers. Preserve this only when the selected font files support those OpenType features.

### Type roles

| Role | Family | Size | Weight/style | Line height | Tracking |
|---|---|---:|---|---:|---:|
| Hero display | Fraunces | `clamp(48px, 13vw, 72px)` | 400 | `.92` | `-.025em` |
| Commerce display | Fraunces | `clamp(46px, 5.7vw, 74px)` | 400 | `.95` | inherited/slightly tight |
| Section heading | Fraunces | `clamp(28px, 4vw, 48px)` | 400 | `1–1.04` | normal |
| Modal heading | Fraunces | `28–38px` | 400 | `1` | normal |
| Lede | Fraunces | `18–19px` | 400 | `1.4–1.42` | normal |
| Body | Inter Tight | `16px` | 400 | `1.5` | normal |
| Strong body/control | Inter Tight | `15–17px` | 600–900 | `1.25–1.45` | `-.005em` to normal |
| Metadata/help | Inter Tight or Fraunces italic | `11–14px` | 400–700 | `1.35–1.5` | normal |
| Eyebrow/micro-label | Inter Tight | `9–11px` | 700–900 | normal | `.12–.22em` |
| Code entry | Monospace | `24–30px` | 700 | normal | `.32em` |

### Editorial devices

- Italic Fraunces marks human, premium, or explanatory content: section numbers, metadata, footnotes, and secondary button copy.
- Large display headings use tight line-height and negative tracking.
- Emphasized words inside a display heading may be italic and blue.
- Drop caps use italic Fraunces at `1.4em`, colored blue.
- Uppercase labels use strong weight and wide tracking; never apply wide tracking to long paragraphs.
- Use `text-wrap: balance` for short display text when supported.

## Borders and rules

- Default: `1px solid var(--rule)`.
- Quiet internal separator: `1px solid var(--rule-soft)`.
- Strong editorial separator: `1px solid var(--ink)`.
- Active choice: blue border plus `inset 0 0 0 1px var(--blue)`.
- Error: red border at full color or `rgba(176,32,46,.28–.38)` on notices.
- Focus ring: `3px solid var(--gold)` with `3px` offset for links/buttons, or a blue `0 0 0 3px rgba(6,8,169,.14)` halo for fields.
- Supplement-facts style uses `1.5–2px` ink rules and dotted row separators.

## Radius policy

| Token | Value | Use |
|---|---:|---|
| `--r-none` | `0` | Editorial registration and admin surfaces |
| `--r-sm` | `10px` | Inputs and compact secondary controls |
| `--r-md` | `14px` | Cards, options, primary shop buttons, segmented tracks |
| `--r-lg` | `24px` | Drawers, modals, large floating surfaces |
| `--r-pill` | `999px` | Badges, proof chips, status pills |

Use rounded corners as a coherent surface-level choice. The original system intentionally keeps registration and admin hard-edged while rounding commerce components.

## Shadows and elevation

| Level | Shadow | Use |
|---|---|---|
| Low | `0 2px 7px rgba(15,15,24,.09)` | Active segment |
| Card | `0 14px 36px rgba(15,15,24,.07)` | Raised commerce card |
| Brand card | `0 10px 28px rgba(4,6,122,.25)` | Blue celebration card |
| Drawer | `-22px 0 70px rgba(15,15,24,.22)` | Desktop side drawer |
| Modal | `0 24px 70px rgba(15,15,24,.22)` or `0 24px 80px rgba(15,15,24,.28)` | Confirmation / commerce modal |
| Toast | `0 20px 48px rgba(15,15,24,.28)` | Floating alert |

Shadows are neutral and soft. Do not use colored glows except the subtle blue field-focus halo.

## Iconography

- The application uses `lucide-react`; use outline icons with consistent stroke weight.
- Normal component icons are approximately `18–22px`.
- Directional icons may sit in a `28px` circular, 1px `currentColor` border.
- Icons inherit text color: ink for neutral, blue for informational, bone for primary actions.
- Icon-only hit areas should be at least `44 × 44px`, even when the glyph is smaller.
- Never use an icon as the only error or success signal; pair it with text.

## Motion

| Interaction | Timing/easing | Effect |
|---|---|---|
| Screen entrance | `.6s cubic-bezier(.22,1,.36,1)` | Fade from opacity 0 and translateY `12px` |
| Button color | `.2s ease` | Ink to blue or blue to pressed blue |
| Button press | `.1s ease` | Scale to `.99` |
| Button sheen | `.6s ease` | Low-opacity diagonal highlight sweeps across |
| Active rail / status | `.3–.6s` | Color, scale, or fill transition |
| Drawer/menu | `.32s cubic-bezier(.22,1,.36,1)` | Translate into view |
| Spinner | `.8s linear infinite` | Continuous rotation |
| Product image | `5s ease-in-out infinite` | Gentle ±5px vertical drift and ~1.5% scale |

Always include `@media (prefers-reduced-motion: reduce)`. Remove decorative drift and large translations; a slower spinner may remain when it communicates loading.

## Interaction-state grammar

- **Hover:** dark primary actions become blue; blue actions become `--blue-press`; outlined controls turn blue at border and text.
- **Focus-visible:** use a visible gold outline for links/buttons; inputs use blue border plus pale-blue halo.
- **Active/pressed:** primary button scales to `.99`; selected choices use blue fill or blue double border.
- **Disabled:** bone-soft/deep fill, ink-3 or ink-4 text, `cursor: not-allowed`; do not rely on opacity alone.
- **Error:** red border, red label/message, and optional pale-red surface.
- **Success:** blue is the normal positive/complete color; bright lime is confined to success toast headings on dark ink.
- **Loading:** retain button dimensions, add an 18px spinner, and prevent repeated activation.

## Accessibility requirements for reuse

- Keep body copy at `16px` when possible and never below `14px` for essential information.
- Micro-labels of `9–11px` must be bold, short, and nonessential or paired with readable content.
- Preserve visible keyboard focus; never remove outlines without replacement.
- Ensure all touch targets are at least `44px` high/wide.
- Communicate selected, error, success, and disabled states with text/attributes as well as color.
- Use `aria-invalid`, `aria-describedby`, `aria-current`, and `aria-live` where applicable.
- Allow browser zoom in the destination application.
- Test blue-on-bone, muted text, error text, and small gold labels for WCAG contrast at their actual sizes.


---

<!-- FILE: 03 - Portable CSS Starter.md -->
# 03 - Portable CSS Starter.md

---
title: GutGuard Portable CSS Starter
tags: [gutguard, css, implementation, design-system]
updated: 2026-08-13
---

# Portable CSS starter

This stylesheet carries the system's visual tokens and common component skins without copying any page layout. Rename the `gg-` classes to match the destination system.

```css
:root {
  color-scheme: light;

  --gg-bone: #f4f1ea;
  --gg-bone-soft: #ebe7de;
  --gg-bone-deep: #ddd7c8;
  --gg-paper: #fcfaf5;

  --gg-blue: #0608a9;
  --gg-blue-press: #04067a;
  --gg-gold: #b08d5b;
  --gg-gold-soft: #c9ac7e;

  --gg-ink: #0f0f18;
  --gg-ink-2: #3a3a48;
  --gg-ink-3: #6b6b7a;
  --gg-ink-4: #a0a0ae;
  --gg-rule: #d8d2c2;
  --gg-rule-soft: #e5e0d2;
  --gg-error: #b0202e;

  --gg-serif: "Fraunces", "Times New Roman", serif;
  --gg-sans: "Inter Tight", system-ui, -apple-system, "Segoe UI", sans-serif;
  --gg-mono: ui-monospace, SFMono-Regular, Menlo, Consolas, monospace;

  --gg-r-sm: 10px;
  --gg-r-md: 14px;
  --gg-r-lg: 24px;
  --gg-r-pill: 999px;

  --gg-shadow-card: 0 14px 36px rgba(15, 15, 24, 0.07);
  --gg-shadow-modal: 0 24px 80px rgba(15, 15, 24, 0.28);
  --gg-ease-out: cubic-bezier(0.22, 1, 0.36, 1);
}

/* Visual foundation only; attach this class to the destination surface. */
.gg-surface {
  color: var(--gg-ink);
  background-color: var(--gg-bone);
  background-image: radial-gradient(
    circle at 1px 1px,
    rgba(15, 15, 24, 0.025) 1px,
    transparent 0
  );
  background-size: 3px 3px;
  font-family: var(--gg-sans);
  font-size: 16px;
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.gg-display {
  margin: 0;
  color: var(--gg-ink);
  font-family: var(--gg-serif);
  font-size: clamp(46px, 7vw, 72px);
  font-weight: 400;
  letter-spacing: -0.025em;
  line-height: 0.95;
  text-wrap: balance;
}

.gg-display em {
  color: var(--gg-blue);
  font-style: italic;
  font-weight: 400;
}

.gg-heading {
  margin: 0;
  color: var(--gg-ink);
  font-family: var(--gg-serif);
  font-size: clamp(28px, 4vw, 46px);
  font-weight: 400;
  line-height: 1.04;
}

.gg-lede {
  color: var(--gg-ink-2);
  font-family: var(--gg-serif);
  font-size: 18px;
  line-height: 1.42;
}

.gg-eyebrow {
  color: var(--gg-blue);
  font-size: 10px;
  font-weight: 900;
  letter-spacing: 0.16em;
  text-transform: uppercase;
}

.gg-help {
  color: var(--gg-ink-3);
  font-size: 12px;
  line-height: 1.45;
}

.gg-card {
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-md);
  background: var(--gg-paper);
  padding: clamp(16px, 2.4vw, 24px);
  box-shadow: var(--gg-shadow-card);
}

.gg-card--editorial {
  border-radius: 0;
  background: var(--gg-bone);
  box-shadow: none;
}

.gg-button {
  min-height: 48px;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  border: 0;
  border-radius: var(--gg-r-sm);
  padding: 12px 18px;
  font: inherit;
  font-weight: 800;
  cursor: pointer;
  transition: background-color 0.2s ease, color 0.2s ease,
    border-color 0.2s ease, transform 0.1s ease;
}

.gg-button--primary {
  background: var(--gg-blue);
  color: var(--gg-bone);
}

.gg-button--primary:hover:not(:disabled) {
  background: var(--gg-blue-press);
}

.gg-button--editorial {
  min-height: 62px;
  justify-content: space-between;
  border-radius: 0;
  background: var(--gg-ink);
  color: var(--gg-bone);
  padding: 18px 24px;
}

.gg-button--editorial:hover:not(:disabled) {
  background: var(--gg-blue);
}

.gg-button--secondary {
  border: 1px solid var(--gg-rule);
  background: rgba(252, 250, 245, 0.72);
  color: var(--gg-ink);
  font-size: 12px;
  font-weight: 900;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.gg-button--secondary:hover:not(:disabled) {
  border-color: var(--gg-blue);
  color: var(--gg-blue);
}

.gg-button:active:not(:disabled) {
  transform: scale(0.99);
}

.gg-button:disabled {
  background: var(--gg-bone-soft);
  color: var(--gg-ink-4);
  cursor: not-allowed;
}

.gg-button:focus-visible,
.gg-link:focus-visible {
  outline: 3px solid var(--gg-gold);
  outline-offset: 3px;
}

.gg-field {
  display: grid;
  gap: 7px;
}

.gg-field__label {
  color: var(--gg-ink-3);
  font-size: 10px;
  font-weight: 900;
  letter-spacing: 0.14em;
  text-transform: uppercase;
}

.gg-field__control {
  width: 100%;
  min-height: 48px;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-sm);
  background: var(--gg-bone);
  padding: 12px 14px;
  color: var(--gg-ink);
  font: inherit;
  outline: none;
}

.gg-field__control::placeholder {
  color: var(--gg-ink-4);
}

.gg-field__control:hover {
  border-color: var(--gg-ink-4);
}

.gg-field__control:focus-visible {
  border-color: var(--gg-blue);
  box-shadow: 0 0 0 3px rgba(6, 8, 169, 0.14);
}

.gg-field__control[aria-invalid="true"] {
  border-color: var(--gg-error);
}

.gg-field__error {
  color: var(--gg-error);
  font-size: 12px;
  font-weight: 800;
}

.gg-segment {
  display: inline-grid;
  grid-auto-flow: column;
  gap: 4px;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-md);
  background: var(--gg-bone-soft);
  padding: 4px;
}

.gg-segment__button {
  min-height: 44px;
  border: 0;
  border-radius: var(--gg-r-sm);
  background: transparent;
  padding: 8px 14px;
  color: var(--gg-ink-3);
  font: inherit;
  font-size: 12px;
  font-weight: 800;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
}

.gg-segment__button[aria-selected="true"],
.gg-segment__button.is-active {
  background: var(--gg-paper);
  color: var(--gg-ink);
  box-shadow: 0 2px 7px rgba(15, 15, 24, 0.09);
}

.gg-badge {
  display: inline-flex;
  align-items: center;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-pill);
  padding: 4px 10px;
  color: var(--gg-ink-3);
  font-size: 10px;
  font-weight: 900;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  white-space: nowrap;
}

.gg-badge--active {
  border-color: rgba(6, 8, 169, 0.32);
  color: var(--gg-blue);
}

.gg-alert {
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-md);
  background: rgba(235, 231, 222, 0.66);
  padding: 13px 15px;
  color: var(--gg-blue);
  font-weight: 700;
}

.gg-alert--error {
  border-color: rgba(176, 32, 46, 0.32);
  background: rgba(176, 32, 46, 0.07);
  color: #8f1824;
}

.gg-backdrop {
  background: rgba(15, 15, 24, 0.58);
  backdrop-filter: blur(3px);
}

/* —— File attachment (never show native file chrome) —— */
.gg-file {
  position: relative;
}

.gg-file__input {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  white-space: nowrap;
  border: 0;
}

.gg-file__zone {
  display: block;
  border: 1.5px dashed var(--gg-rule);
  border-radius: var(--gg-r-md);
  background: var(--gg-bone);
  padding: 22px 18px;
  text-align: center;
  cursor: pointer;
  color: var(--gg-ink);
}

.gg-file__zone:hover,
.gg-file:focus-within .gg-file__zone {
  border-color: var(--gg-blue);
  background: rgba(6, 8, 169, 0.04);
}

.gg-file__zone.is-error {
  border-color: var(--gg-error);
  background: rgba(176, 32, 46, 0.05);
}

.gg-file__icon {
  display: inline-grid;
  place-items: center;
  width: 44px;
  height: 44px;
  margin: 0 auto 10px;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-sm);
  background: var(--gg-paper);
  color: var(--gg-ink-3);
}

.gg-file__zone:hover .gg-file__icon {
  color: var(--gg-blue);
  border-color: var(--gg-blue);
}

.gg-file__title {
  display: block;
  margin-bottom: 4px;
  font-size: 15px;
  font-weight: 700;
}

.gg-file__hint {
  display: block;
  margin-bottom: 14px;
  color: var(--gg-ink-3);
  font-size: 13px;
}

.gg-file__zone.is-error .gg-file__hint {
  color: #8f1824;
}

.gg-file__row {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 12px 14px;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-sm);
  background: var(--gg-paper);
}

.gg-file__row.is-error {
  border-color: var(--gg-error);
}

.gg-file__type {
  width: 36px;
  height: 36px;
  display: grid;
  place-items: center;
  flex-shrink: 0;
  border-radius: 8px;
  background: rgba(6, 8, 169, 0.08);
  color: var(--gg-blue);
  font-size: 11px;
  font-weight: 800;
}

.gg-file__name {
  font-size: 14px;
  font-weight: 700;
}

.gg-file__meta {
  font-size: 12px;
  color: var(--gg-ink-3);
}

.gg-file__progress {
  height: 6px;
  margin-top: 10px;
  border-radius: var(--gg-r-pill);
  background: var(--gg-bone-soft);
  overflow: hidden;
}

.gg-file__progress > i {
  display: block;
  height: 100%;
  background: var(--gg-blue);
  border-radius: inherit;
}

/* —— Icon button (Lucide-style SVG, currentColor) —— */
.gg-icon-btn {
  width: 44px;
  height: 44px;
  display: inline-grid;
  place-items: center;
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-sm);
  background: var(--gg-paper);
  color: var(--gg-ink);
  cursor: pointer;
  flex-shrink: 0;
}

.gg-icon-btn svg {
  width: 20px;
  height: 20px;
  stroke: currentColor;
  fill: none;
  stroke-width: 2;
  stroke-linecap: round;
  stroke-linejoin: round;
}

.gg-icon-btn:hover:not(:disabled) {
  border-color: var(--gg-blue);
  color: var(--gg-blue);
}

.gg-icon-btn:disabled {
  color: var(--gg-ink-4);
  cursor: not-allowed;
}

.gg-icon-btn--dense {
  width: 36px;
  height: 36px;
}

.gg-icon-btn--ghost {
  border-color: transparent;
  background: transparent;
}

.gg-icon-btn--square {
  border-radius: 0;
}

/* —— Dialog (structured header / body / footer) —— */
.gg-dialog {
  display: flex;
  flex-direction: column;
  width: min(100%, 520px);
  border: 1px solid var(--gg-rule);
  border-radius: var(--gg-r-lg);
  background: var(--gg-paper);
  box-shadow: var(--gg-shadow-modal);
  overflow: hidden;
}

.gg-dialog--square {
  border-radius: 0;
}

.gg-dialog-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  padding: 18px 20px;
  border-bottom: 1px solid var(--gg-rule);
}

.gg-dialog-header h2,
.gg-dialog-title {
  margin: 0;
  font-family: var(--gg-serif);
  font-size: 28px;
  font-weight: 400;
  line-height: 1.1;
  letter-spacing: -0.02em;
  color: var(--gg-ink);
}

.gg-dialog-body {
  padding: 20px;
  color: var(--gg-ink-2);
  font-size: 14px;
  line-height: 1.5;
  overflow: auto;
  max-height: min(50vh, 360px);
}

.gg-dialog-footer {
  display: flex;
  justify-content: flex-end;
  gap: 10px;
  padding: 16px 20px;
  border-top: 1px solid var(--gg-rule);
}

/* —— Switch —— */
.gg-switch {
  position: relative;
  width: 44px;
  height: 26px;
  border: 0;
  border-radius: var(--gg-r-pill);
  background: var(--gg-bone-deep);
  cursor: pointer;
  flex-shrink: 0;
  transition: background 0.18s var(--gg-ease-out);
}

.gg-switch::after {
  content: "";
  position: absolute;
  top: 3px;
  left: 3px;
  width: 20px;
  height: 20px;
  border-radius: 50%;
  background: var(--gg-paper);
  box-shadow: 0 1px 3px rgba(15, 15, 24, 0.18);
  transition: transform 0.18s var(--gg-ease-out);
}

.gg-switch[aria-checked="true"] {
  background: var(--gg-blue);
}

.gg-switch[aria-checked="true"]::after {
  transform: translateX(18px);
}

.gg-switch-row {
  display: inline-flex;
  align-items: center;
  gap: 12px;
  font-size: 14px;
  font-weight: 600;
  color: var(--gg-ink);
}

/* —— Accordion chevron (pair with .gg-icon-btn--ghost) —— */
.gg-acc-head {
  width: 100%;
  min-height: 52px;
  padding: 12px 16px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
  font-weight: 700;
  text-align: left;
  background: transparent;
  border: 0;
  cursor: pointer;
  color: inherit;
}

.gg-acc-head .gg-chev {
  color: var(--gg-ink-3);
  transition: transform 0.2s var(--gg-ease-out), color 0.2s var(--gg-ease-out);
}

.gg-acc-item[data-open="true"] .gg-acc-head .gg-chev,
.gg-acc-item.open .gg-acc-head .gg-chev {
  transform: rotate(180deg);
  color: var(--gg-blue);
}

@media (prefers-reduced-motion: reduce) {
  .gg-button,
  .gg-segment__button,
  .gg-switch,
  .gg-switch::after,
  .gg-acc-head .gg-chev {
    scroll-behavior: auto;
    transition-duration: 0.01ms;
  }
}
```


## Optional editorial ruled field

Use this variant for the square registration dialect instead of the boxed field.

```css
.gg-ruled-field {
  border-bottom: 1px solid var(--gg-rule);
  padding: 18px 0;
}

.gg-ruled-field:focus-within {
  border-bottom-color: var(--gg-blue);
}

.gg-ruled-field__label {
  color: var(--gg-ink-3);
  font-family: var(--gg-serif);
  font-size: 14px;
  font-style: italic;
}

.gg-ruled-field__control {
  border: 0;
  border-radius: 0;
  background: transparent;
  padding: 4px 0;
  color: var(--gg-ink);
  font: 500 17px/1.4 var(--gg-sans);
  outline: 0;
}

.gg-ruled-field:focus-within .gg-ruled-field__label {
  color: var(--gg-blue);
}

.gg-ruled-field.has-error {
  border-bottom-color: var(--gg-error);
}

.gg-ruled-field.has-error .gg-ruled-field__label {
  color: var(--gg-error);
}
```

## Variables supplied beyond the original stylesheet

The source CSS references several undefined names. For portability, map them as follows:

| Original reference | Safe portable value |
|---|---|
| `--paper` | `#FCFAF5` |
| `--cream` | `#FCFAF5` or `#F4F1EA` |
| `--rule-strong` | `#C8C0AE` |
| `--mono` | `ui-monospace, SFMono-Regular, Menlo, Consolas, monospace` |
| `--heat` | `#B5431F` |
| `--recovery` | `#1E6FB8` |

## Usage rule

Choose either the rounded component classes or the editorial square modifiers for a given product surface. Keep the tokens identical so separate systems still read as the same GutGuard brand.


---

<!-- FILE: 04 - Stitch Workflow.md -->
# 04 - Stitch Workflow.md

---
title: Boss HTML / Next.js → Obsidian → Stitch workflow
tags: [gutguard, stitch, workflow, cursor]
updated: 2026-08-12
---

# Stitch workflow

Goal: when the boss sends HTML or a Next.js app, Cursor reads this vault’s design system, Stitch generates on-brand screens, and we implement against the portable CSS.

## Paths

| Role | Path |
|---|---|
| Obsidian vault | `C:\Users\najee\OneDrive\Documents\Obsidian Vault\` |
| Design system | `GutGuard Design System\` |
| Stitch brief | `GutGuard Design System\DESIGN.md` |
| Portable CSS | `GutGuard Design System\03 - Portable CSS Starter.md` |
| Inbox for boss drops | `GutGuard Design System\Inbox\` |

## Operator steps (human)

1. Drop the boss file/folder into `Inbox\` (or paste the path in Cursor chat).
2. In Cursor **Customize → MCPs**, confirm `stitch` shows tools **> 0** (not “0 tools enabled”).
3. Tell Cursor: *“Run the GutGuard Stitch workflow on `<path>` using dialect `<editorial|commerce|admin>`.”*

## Agent steps (Cursor)

1. Read `DESIGN.md`, dialect notes (`01` + `Foundations/Dialects`), and relevant notes under `Components/`.
2. Inspect the boss HTML / Next.js screens (routes, components, copy, structure).
3. Create or select a Stitch project for this deliverable.
4. Upload / apply `DESIGN.md` as the design system for that project.
5. Generate screens in Stitch that preserve boss structure/content but GutGuard visual language.
6. Export HTML/screenshots from Stitch.
7. Implement into the Next.js/HTML target using tokens/classes from the portable CSS starter.
8. Log outputs under `Inbox\<deliverable-name>\` (notes + export paths).
9. If the boss system introduced new reusable UI, update `Systems/` + `Components/Index`.

## Prompt template

```text
Run the GutGuard Stitch workflow.

Input: <path to boss HTML or Next.js>
Dialect: <editorial | commerce | admin>
Design system: GutGuard Design System/DESIGN.md + 03 Portable CSS Starter

Do:
1) Summarize screens/routes in the input
2) Apply DESIGN.md in Stitch
3) Generate each screen on-brand
4) Export and propose Next.js/HTML implementation plan using gg-* tokens/classes
```

## Stitch MCP health

If MCP shows **Connected / 0 tools enabled**, Cursor is dropping Stitch’s oversized tool schemas. Use the local proxy:

- Proxy script: `%USERPROFILE%\.cursor\stitch-mcp-proxy.mjs`
- MCP config: `%USERPROFILE%\.cursor\mcp.json` must run `node` + that proxy with `STITCH_API_KEY`

Then toggle the `stitch` server off/on (or restart Cursor) until tool count is > 0.


---

<!-- FILE: 05 - Playbook.md -->
# 05 - Playbook.md

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


---

<!-- FILE: 07 - Using the DS with Cursor.md -->
# 07 - Using the DS with Cursor.md

---
title: Using the Design System with Cursor
aliases:
  - Cursor adoption guide
  - AGENTS design system
tags: [gutguard, design-system, cursor, agents, playbook]
updated: 2026-08-12
---

# Using the Design System with Cursor

**Before Cursor generates any frontend**, the human and the agent must read this vault’s design system. Prototypes/boss files define *what* to build; **Obsidian defines how it looks**.

Related: [[05 - Playbook]] (team process) · live preview `Showcase/index.html` · [[00 - OWNER — Read only]]

---

## For humans (before you open Cursor)

1. Sync Obsidian so `GutGuard Design System/` is current.
2. Remember: **read-only** unless you are the DS owner ([[00 - OWNER — Read only]]).
3. Skim in this order:
   1. [[00 - GutGuard Design System]]
   2. [[01 - Visual Foundations]] + [[Foundations/Dialects]]
   3. [[Components/Index]] (only the components you’ll need)
   4. Optional: open `Showcase/index.html` in a browser
4. Decide **one dialect** for the screen: editorial · commerce · admin.
5. Drop boss HTML / brief into `Inbox/` or keep the path ready (**owner** manages Inbox on the authority machine if Sync conflicts worry you).
6. In the **product repo**, paste the AGENTS / Cursor rule below (once per project).
7. Then prompt Cursor — e.g.  
   *“Build the Academy dashboard UI. Dialect: commerce. Read the GutGuard Design System vault first; do not invent colors or fonts; do not edit the vault.”*

---

## For Cursor / agents (hard rule)

**Always, before writing UI:**

1. Read (at minimum) from `{GG_DS}` — see path section above:
   - `00 - OWNER — Read only.md`
   - `00 - GutGuard Design System.md`
   - `01 - Visual Foundations.md`
   - `Foundations/Dialects.md`
   - `Components/Index.md`
   - Relevant `Components/<Name>.md` notes
   - `03 - Portable CSS Starter.md` when adding styles
2. Optional visual check: `Showcase/index.html`
3. Then generate frontend using Doctors tokens (bone, ultramarine, Fraunces, Inter Tight).
4. Never treat Academy / Lifestyle / other prototypes as visual source of truth.
5. **Never modify files under `GutGuard Design System/`.** Product repo only. DS changes → ask owner (Najee).

**Vault path:** each teammate uses **their own** synced path to the same folder name `GutGuard Design System`. Obsidian Sync shares the notes; the PC path is local.

Example shape (replace with yours):

`C:\Users\<you>\OneDrive\Documents\Obsidian Vault\GutGuard Design System\`

Najee’s machine (reference only):

`C:\Users\najee\OneDrive\Documents\Obsidian Vault\GutGuard Design System\`

---

## Paste into each product repo

### Option A — `AGENTS.md` (recommended)

Create or append in the project root:

```markdown
# GutGuard UI — Design System gate

Before generating or changing any frontend (HTML, CSS, React, Stitch):

1. Read the Obsidian GutGuard Design System (synced vault) — **READ ONLY**.
2. Do **not** edit, create, or delete files inside `GutGuard Design System/`. Only the DS owner (Najee) may change the vault. Implement UI in this product repo only.
3. Minimum reads:
   - `GutGuard Design System/00 - OWNER — Read only.md`
   - `GutGuard Design System/00 - GutGuard Design System.md`
   - `GutGuard Design System/01 - Visual Foundations.md`
   - `GutGuard Design System/Foundations/Dialects.md`
   - `GutGuard Design System/Components/Index.md`
   - Component notes under `GutGuard Design System/Components/` for UI you touch
   - `GutGuard Design System/03 - Portable CSS Starter.md` for tokens/classes
4. Open `GutGuard Design System/Showcase/index.html` if unsure how a control should look.
5. Pick one dialect per screen (editorial / commerce / admin). Do not mix radius policies.
6. Visual source of truth = Doctors / vault — NOT boss prototypes (Academy, Lifestyle, etc.).
7. Recognition cues: bone `#F4F1EA`, blue `#0608A9`, ink `#0F0F18`, gold `#B08D5B`, Fraunces + Inter Tight, paper grain, uppercase micro-labels.

Local vault path — **replace with YOUR synced path**:
`C:\Users\<you>\…\Obsidian Vault\GutGuard Design System\`

Workflow detail: vault note `07 - Using the DS with Cursor.md` and `05 - Playbook.md`.
```

### Option B — `.cursor/rules/gutguard-design-system.mdc`

Copy from [[Templates/gutguard-design-system]] (or `Templates/gutguard-design-system.mdc`). After paste, set `GG_DS` to **your** vault path — not a teammate’s.

Use **both** if you want belt-and-suspenders (AGENTS.md for all agents; `.mdc` for Cursor).

---

## Suggested first prompt (copy)

```text
We are building <system name>.

Design system (read BEFORE coding) — MY vault path:
C:\Users\<you>\…\Obsidian Vault\GutGuard Design System\

Read 00, 01, Foundations/Dialects, Components/Index, and any component notes we need.
Dialect for this work: <editorial | commerce | admin>
Boss / prototype structure (look is NOT from here): <path>

Do:
1) Confirm which components from the Index you will use
2) Generate the frontend using Doctors / vault visuals only
3) Prefer gg-* tokens from 03 - Portable CSS Starter
```

---

## Checklist for a new system

- [ ] Obsidian Sync on for the shared vault
- [ ] `AGENTS.md` and/or `.cursor/rules/gutguard-design-system.mdc` in the repo
- [ ] Dialect chosen
- [ ] Boss file in `Inbox/` or path given
- [ ] Agent read vault before first UI file
- [ ] QA against [[05 - Playbook]] checklist + `Showcase/index.html`

---

## FAQ

**Is the Playbook enough?**  
[[05 - Playbook]] is process + remap. **This note** is specifically “gate Cursor until the DS is read.”

**What if Cursor can’t see OneDrive?**  
Add the vault folder to the workspace (multi-root) or paste the absolute path in the prompt. The rule says: stop and ask — don’t invent UI.

**Stitch?**  
Still upload [[DESIGN]]; structure from boss; visuals from vault. See [[04 - Stitch Workflow]].


---

<!-- FILE: DESIGN.md -->
# DESIGN.md

# GutGuard Design System (Stitch)

Source of truth: this Obsidian vault folder. Use these rules when generating any UI in Stitch or Next.js.

## Brand character

Clinical + editorial premium health:

- Warm bone canvas `#F4F1EA` (not pure white)
- Ultramarine `#0608A9` for actions, focus, emphasis
- Near-black ink `#0F0F18`
- Muted gold `#B08D5B` sparingly for premium moments
- Fraunces for display/editorial; Inter Tight for UI
- Subtle 3px paper-grain texture
- Uppercase micro-labels, strong weight, wide tracking

## Dialects (pick one per screen)

| Dialect | Radius | Use |
|---|---|---|
| Editorial registration | mostly `0` | Registration, verification, prize reveal |
| Commerce / partner | `10–24px` | Shop, checkout, partner auth, order status |
| Admin | mostly `0` | Tables, management forms, tabs, alerts |

Do not mix radius policies on one screen.

## Color tokens

| Token | Value | Role |
|---|---|---|
| bone | `#F4F1EA` | Primary canvas |
| bone-soft | `#EBE7DE` | Inset / disabled |
| bone-deep | `#DDD7C8` | Strong muted surface |
| paper | `#FCFAF5` | Raised surfaces |
| blue | `#0608A9` | Primary action / focus |
| blue-press | `#04067A` | Pressed blue |
| gold | `#B08D5B` | Premium accent |
| gold-soft | `#C9AC7E` | Light premium accent |
| ink | `#0F0F18` | Primary text |
| ink-2 | `#3A3A48` | Secondary text |
| ink-3 | `#6B6B7A` | Muted labels / help |
| ink-4 | `#A0A0AE` | Placeholder / disabled |
| rule | `#D8D2C2` | Borders |
| rule-soft | `#E5E0D2` | Quiet separators |
| error | `#B0202E` | Destructive / invalid |

## Canvas

```css
background-color: #F4F1EA;
background-image: radial-gradient(circle at 1px 1px, rgba(15,15,24,0.025) 1px, transparent 0);
background-size: 3px 3px;
```

## Typography

- Display / headings: Fraunces 400, tight line-height, slight negative tracking
- Body / controls: Inter Tight 16px / 1.5
- Eyebrows: Inter Tight 9–11px, weight 700–900, uppercase, tracking `.12–.22em`
- Italic Fraunces for human/premium annotations
- Emphasized words in display headings may be italic blue

## Components (visual only)

### Buttons

- **Editorial primary:** full width, ~62px, ink fill, bone text, square; hover → blue
- **Commerce primary:** blue fill, bone text, 14px radius, min-height 62px, heavy label
- **Partner compact:** blue, 9–10px radius, min-height 48px
- **Secondary outline:** 1px rule, paper background, uppercase micro label
- **Text link:** blue, underline offset 3px
- Focus-visible: 3px gold outline, 3px offset
- Disabled: bone-soft / ink-4, not-allowed

### Fields

- **Commerce boxed:** bone fill, 1px rule, 10px radius, min-height 48px; focus blue border + pale blue halo
- **Editorial ruled:** transparent, bottom rule only; Fraunces italic label; focus rule/label → blue; error → `#B0202E`

### Surfaces

- Cards: paper, 1px rule; commerce radius 14px + soft shadow; editorial square, no shadow
- Badges: pill, uppercase micro label
- Alerts: muted bone band; error uses pale red wash
- Dialogs: paper, large radius (commerce) or square (admin), soft modal shadow

## Motion

- Entrance: `.6s cubic-bezier(.22,1,.36,1)`, fade + 12px rise
- Button color `.2s ease`; press scale `.99`
- Honor `prefers-reduced-motion`

## Hard constraints for Stitch

1. No purple gradients, no generic SaaS indigo, no pure-white default canvas.
2. No floating badge clutter on heroes.
3. One dialect per screen.
4. Preserve bone / blue / ink / gold recognition cues above all else.
5. Generate component skins only; page layout may follow the boss HTML/Next.js structure.
6. Prefer lucide-style outline icons, 18–22px, never icon-only status without text.

## Vault references

- `00 - GutGuard Design System.md` — overview
- `Foundations/` + `01 - Visual Foundations.md` — tokens, type, motion, a11y, dialects
- `Components/Index.md` — living component catalog (prefer over legacy `02`)
- `Systems/Doctors-HTML.md` — first system harvest
- `03 - Portable CSS Starter.md` — copy-ready CSS (`gg-*` classes)


---

<!-- FILE: Foundations/README.md -->
# Foundations/README.md

---
title: Foundations
tags: [gutguard, design-system, foundations]
updated: 2026-08-14
---

# Foundations

Tokens and rules every component inherits. Finalize these before inventing new component skins.

- [[01 - Visual Foundations]] — colors, type, borders, radii, shadows, icons, motion, states, a11y
- [[Foundations/Dialects]] — editorial / commerce / admin radius + tone policy
- [[Foundations/Breakpoints]] — **900px** shell cut, content widths, responsive rules for components
- [[03 - Portable CSS Starter]] — copy-ready `gg-*` tokens and skins
- [[DESIGN]] — compact Stitch brief


---

<!-- FILE: Foundations/Breakpoints.md -->
# Foundations/Breakpoints.md

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


---

<!-- FILE: Foundations/Dialects.md -->
# Foundations/Dialects.md

---
title: Dialects
tags: [gutguard, design-system, foundations]
updated: 2026-08-12
---

# Dialects

One screen = one dialect. Shared colors and type hierarchy stay constant; radius and density change.

| Dialect | Character | Radius | Typical use |
|---|---|---:|---|
| Editorial (booth) | Magazine-like, ceremonial, high type contrast | Mostly `0` | Registration, verification, prize |
| Editorial (marketing) | Warm premium site, mono eyebrows, pill CTAs | Soft / pill | Marketing site nav + sections |
| Commerce / partner | Warm, friendly, softly premium | `10–24px` | Shop, checkout, partner, order status |
| Admin | Dense, functional, high clarity | Mostly `0` | Tables, management forms, tabs, alerts |

## Rules

1. Do not mix radius policies randomly on one screen.
2. Blue / bone / ink / gold tokens are shared across all dialects.
3. When a component has dialect variants, document them on that component note — not as separate unrelated components.
4. Marketing soft-pill buttons are a **variant of Button**, not a fourth brand.


---

<!-- FILE: Components/Index.md -->
# Components/Index.md

---
title: Component Index
aliases: [Components]
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: living
---

# Component index

Canonical GutGuard components. Each note is the team source of truth for look, variants, states, dialect rules, and **Responsive** behavior ([[Foundations/Breakpoints]]).

Harvested first from [[Systems/Doctors-HTML]]. When another system is scanned, add new notes or update variants — do not fork parallel specs.

## Shell / chrome

| Component | Status | Notes |
|---|---|---|
| [[Components/Top Bar]] | Draft | Shop / marketing fixed header (Academy has none — page mast only) |
| [[Components/Sidebar]] | Draft | **New from Academy** — desktop 280px rail (≥900px) |
| [[Components/Bottom Bar]] | Draft | **New from Academy** — mobile sticky “Next” CTA |
| [[Components/Masthead]] | Draft | Booth / Academy page mast (not a fixed top bar) |
| [[Components/Admin Shell]] | Draft | Admin hero + tabbed ops chrome |
| [[Components/Progress Rail]] | Draft | Multi-step booth progress |

## Actions & forms

| Component | Status | Notes |
|---|---|---|
| [[Components/Button]] | Draft | Editorial / commerce / marketing / admin variants |
| [[Components/Icon Button]] | Draft | Square icon control — Lucide SVG (`x`, chevrons, more) |
| [[Components/Form Field]] | Draft | Ruled / boxed / partner / admin |
| [[Components/Segmented Control]] | Draft | Trial/protocol, QR mode toggles |
| [[Components/Switch]] | Draft | Boolean on/off — blue track when on |

## Navigation

| Component | Status | Notes |
|---|---|---|
| [[Components/Tabs]] | Draft | Admin tabs + marketing section tabs |

## Surfaces

| Component | Status | Notes |
|---|---|---|
| [[Components/Card]] | Draft | Editorial panel, commerce card, auth card, admin panel |
| [[Components/Modal]] | Draft | Overlay surface variants (backdrop / shell) |
| [[Components/Dialog]] | Draft | Structured header · body · footer + SVG close |
| [[Components/Drawer]] | Draft | Shop basket / checkout |

## Feedback

| Component | Status | Notes |
|---|---|---|
| [[Components/Alert]] | Draft | Inline info / error |
| [[Components/Toast]] | Draft | Floating dark toast |
| [[Components/Badge]] | Draft | Status pills, proof chips |
| [[Components/Empty State]] | Draft | Quiet empty panels |

## Data

| Component | Status | Notes |
|---|---|---|
| [[Components/Table]] | Draft | Admin data tables |
| [[Components/Definition List]] | Draft | Confirm / detail rows |
| [[Components/QR Block]] | Draft | Printable QR surface |

## Editorial atoms

| Component | Status | Notes |
|---|---|---|
| [[Components/Section Label]] | Draft | Numbered section eyebrow |
| [[Components/Task Item]] | Draft | Verification checklist row |

## Common utilities (added)

| Component | Status | Notes |
|---|---|---|
| [[Components/File Attachment]] | Draft | Custom drop zone — **hide native file input** |
| [[Components/Avatar]] | Draft | Initials or image |
| [[Components/Tooltip]] | Draft | Short hover/focus help |
| [[Components/Pagination]] | Draft | Admin table paging |
| [[Components/Spinner]] | Draft | Inline / block / page loading |
| [[Components/Search Field]] | Draft | Filter input with icon |
| [[Components/Dropdown Menu]] | Draft | ··· overflow actions |
| [[Components/Quantity Stepper]] | Draft | − / value / + (shop & dosing) |
| [[Components/Skeleton]] | Draft | Loading placeholders |

## Extended (nice-to-have)

| Component | Status | Notes |
|---|---|---|
| [[Components/Accordion]] | Draft | FAQ / disclosure — SVG chevron-down (not text ▾) |
| [[Components/Breadcrumbs]] | Draft | Nested path nav |
| [[Components/Date Picker]] | Draft | Calendar booking |
| [[Components/Notification Bell]] | Draft | Bell + badge + panel |
| [[Components/Chat Link Row]] | Draft | External chat CTA row |

## Academy / training (from Gentrep scan)

| Component | Status | Notes |
|---|---|---|
| [[Components/Rank Ladder]] | Draft | Horizontal rank chips |
| [[Components/Rank Plate]] | Draft | Hero progress plate (brand-special) |
| [[Components/Requirement Timeline]] | Draft | Spine + requirement cards |
| [[Components/Event Row]] | Draft | Bookable session row |
| [[Components/Lang Toggle]] | Draft | EN/TL segmented switch |
| [[Components/Certificate]] | Draft | Printable cert — system-special |

## Status key

- **Draft** — extracted from Doctors; needs team finalize pass
- **Final** — locked for team use across systems
- **System-only** — brand special; see Systems notes, not core kit

## Finalize checklist (per component)

- [ ] Variants named and dialect-tagged
- [ ] Default / hover / focus-visible / active / disabled / loading / error covered
- [ ] **Responsive** section present (breakpoints or “container-fluid”) — see [[Foundations/Breakpoints]]
- [ ] Source classes + React files listed
- [ ] Portable `gg-*` mapping noted (or TODO)
- [ ] Conflicts with other systems resolved
- [ ] Status flipped to **Final**


---

<!-- FILE: Components/Accordion.md -->
# Components/Accordion.md

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


---

<!-- FILE: Components/Admin Shell.md -->
# Components/Admin Shell.md

---
title: Admin Shell
tags: [gutguard, design-system, components, shell]
updated: 2026-08-12
status: draft
sources:
  - GutGuard-Doctors-HTML/app/admin/wheel/page.tsx
  - GutGuard-Doctors-HTML/app/admin/tiktok/page.tsx
  - GutGuard-Doctors-HTML/app/admin/orders/page.tsx
  - GutGuard-Doctors-HTML/styles/globals.css (.admin-wheel-shell*)
---

# Admin Shell

Ops chrome for admin tools. In Doctors: **hero + horizontal tabs** — not a sidebar layout, and **not a [[Components/Top Bar]]**.

## Anatomy

1. **Shell** — `.admin-wheel-shell` (+ page modifiers like `.admin-tiktok-shell`, `.admin-shop-orders-shell`)
2. **Hero** — `.admin-wheel-hero`, kicker, summary metrics
3. **Tabs** — [[Components/Tabs]] admin variant
4. **Panel** — `.admin-wheel-panel` / panel head for content blocks
5. **Auth gate** — password unlock row before tools

## Visual rules

- Dialect: **Admin** (square, dense)
- Bone canvas + paper/bone panels with 1px rules
- Buttons / fields inherit shell-scoped skins (see [[Components/Button]], [[Components/Form Field]])
- Tables and modals nest inside panels

## Future sidebar

If a later system adds a left nav, use [[Components/Sidebar]] and keep Admin Shell as the page frame that can host either tabs or sidebar + content.

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` | Hero stacks (title → metrics); [[Components/Tabs]] scroll horizontally if needed; panels full width with reduced padding |
| `≥ 900px` | Hero can sit in a row; tabs + panels in full admin width |

Admin Shell does **not** auto-pair with Bottom Bar. Dense 36px controls allowed only inside admin tables/toolbars.

## Finalize

- [ ] Rename shell classes to dialect-neutral `admin-shell`
- [ ] Document hero density + summary chip rules
- [ ] Mark **Final**


---

<!-- FILE: Components/Alert.md -->
# Components/Alert.md

﻿---
title: Alert
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/styles/globals.css
  - ConfirmRegistrationModal, admin pages, Shoplet, WheelSection, PartnerPortal
---

# Alert

Inline feedback inside a page or panel (not floating — see [[Components/Toast]]).

## Variants

| Variant | Treatment |
|---|---|
| Info | Rule border; pale bone-soft ~66%; blue text / 700 |
| Error | Border `rgba(176,32,46,.28–.38)`; wash `rgba(176,32,46,.06–.07)`; title `#B0202E`; body `#8F1824` |
| Compact auth error | 3px red left border; tight padding |
| Confirm warning | `.confirm-warning` in booth modal |
| Admin | `.admin-wheel-alert` (+ `.error`) |
| Shop | `.shop-error` / `.shop-success` |

## Rules

- Square in admin; 14px radius on commerce
- Title often 10px uppercase tracked
- Never icon-only — pair with text
- Live region when the alert appears dynamically

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** — full width of the content column. Multi-line copy wraps; do not truncate error text on mobile.

## Finalize
- [ ] Collapse shop/admin/booth class names into `gg-alert` variants
- [ ] Mark **Final**


---

<!-- FILE: Components/Avatar.md -->
# Components/Avatar.md

﻿---
title: Avatar
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Avatar

User / member identity mark for sidebars, rosters, headers.

## Spec

- Circle (or soft 10px square in admin lists)
- Sizes: `32` · `40` · `48` · `64`
- Image cover, or initials on bone-soft / blue wash
- Initials: Inter Tight 700, ink or blue
- Optional status ring: blue (online/active), rule (default)
- Pair with name + meta — never icon-only identity for critical actions

## Seen in

Lifestyle sidebar `.who` / `.avatar`; team roster cards.

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint — fixed sizes (sm/md/lg). In headers, allow the text block to wrap beside the avatar.

## Finalize
- [ ] Lock size scale
- [ ] Mark **Final**


---

<!-- FILE: Components/Badge.md -->
# Components/Badge.md

﻿---
title: Badge
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - PartnerPortal (.partner-badge)
  - GutguardSite (BetaFlag)
  - globals status pill patterns
---

# Badge

Compact status or proof chip.

## Variants

| Variant | Treatment |
|---|---|
| Status pill | 1px rule, pill radius, 4px 10px pad; 10px / 900 / uppercase / `.1em` / ink-3 |
| Paid / active | Border `rgba(6,8,169,.32)`, blue text (e.g. `.partner-badge.paid`) |
| Proof chip | Paper tint, rule, pill; slightly tighter pad |
| Marketing beta | `.beta-tag` / `.sec-flag` — editorial flags |

## Rules

- Always include readable status text
- Don’t color entire table rows — badge the status cell
- Pill radius token `--r-pill`

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint — inline chip. May wrap with adjacent text; do not shrink below readable 11–12px caps.

## Finalize
- [ ] Standardize paid/failed/pending/cancelled set
- [ ] Mark **Final**


---

<!-- FILE: Components/Bottom Bar.md -->
# Components/Bottom Bar.md

---
title: Bottom Bar
aliases:
  - Sticky Next Bar
  - Foot Bar
tags: [gutguard, design-system, components, shell]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.foot, .foot-in, .foot-title, .eyebrow-dark)
---

# Bottom Bar

Fixed mobile chrome for a primary next / order action. From prototypes [[Systems/Gentrep-Academy-Dashboard]] and [[Systems/GutGuard-Lifestyle]] — **skin with Doctors / GG**, not prototype colors.

## Behavior

- `position: fixed`; bottom 0; full width; `z-index: 40`
- Paper/bone surface; 1px top rule; soft upward shadow optional
- Inner max-width ~440px
- Safe-area padding
- **Hidden on desktop** when [[Components/Sidebar]] is shown

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` | **Visible** (when the product uses a sticky primary CTA) |
| `≥ 900px` | **Hidden** if Sidebar carries the same CTA / next action |

Reserve bottom safe-area (`env(safe-area-inset-bottom)`). Toasts sit above the bar (~96px from bottom on Academy).

## Anatomy

```
optional eyebrow
title / CTA label                 [ Button ]
```

Uses [[Components/Button]] commerce primary.

## Seen in

| System | Class | CTA |
|---|---|---|
| Academy | `.foot` | Do this next |
| Lifestyle | `.gg-foot` | Order now |

## vs Top Bar / tabs

- [[Components/Top Bar]] = navigation
- **Bottom Bar** = single persistent CTA
- Do **not** turn this into a multi-tab bar — Lifestyle tabs are [[Components/Segmented Control]]

## Finalize

- [ ] Remap to bone/paper + ink/blue
- [ ] Confirm toast sits above bar (Academy toast `bottom: 96px`)
- [ ] Mark **Final**


---

<!-- FILE: Components/Breadcrumbs.md -->
# Components/Breadcrumbs.md

﻿---
title: Breadcrumbs
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Breadcrumbs

Path navigation for nested admin / content.

## Spec

- Items: 13px / 600, ink-3; current: ink, not a link
- Separator: `/` or chevron in ink-4
- Hover links → blue
- Wrap on small screens; don’t truncate current page
- Optional home icon with accessible name

## Responsive

See [[Foundations/Breakpoints]].

On < 900px, allow wrap or collapse middle crumbs to ellipsis; keep current page visible.

## Finalize
- [ ] Mark **Final** when needed


---

<!-- FILE: Components/Button.md -->
# Components/Button.md

﻿---
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


---

<!-- FILE: Components/Card.md -->
# Components/Card.md

﻿---
title: Card
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/styles/globals.css
  - Shop / Partner / Admin panels
---

# Card

Raised or ruled content surface. Prefer rules over heavy shadows.

## Variants

| Variant | Treatment | Dialect |
|---|---|---|
| Editorial panel | Bone, 1px rule, square, little/no shadow | Editorial |
| Commerce card | Paper, 1px rule, 14px radius, soft card shadow | Commerce |
| Auth card | Paper ~94% opacity, rule, **3px blue top border**, 14px radius | Commerce |
| Order panel | `.shop-order-panel` + status modifiers (`paid` / `failed` / `cancelled`) | Commerce |
| Admin panel | `.admin-wheel-panel` + panel head | Admin |
| Dark ceremonial | Ink→blue gradient, bone text, gold-soft eyebrows | Editorial special |
| Stat / trust | Centered; Fraunces value; uppercase caption | Commerce / marketing |

## Rules

- Nested blocks use bone, not a second white card
- Selectable option cards: active = blue border + inset blue line → see choice patterns in Shop
- Cards are for grouping content; interactive choices should expose selected state in text/ARIA too

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid**. In grids: 1 column < 900px, 2+ columns from desktop unless the page defines otherwise. Padding may reduce slightly on narrow screens; radius follows dialect.

## Finalize
- [ ] Name status tones for order panel
- [ ] Mark **Final**


---

<!-- FILE: Components/Certificate.md -->
# Components/Certificate.md

---
title: Certificate
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.cert, .cert-*)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Certificate

Ceremonial rank certificate surface. **System-special** — print-optimized.

## Anatomy

- Cream card (`#FCFAF4` / `#F3EFE4`), navy outline (6px inset offset)
- Brand row, eyebrow, “hereby certifies”, italic display name
- Rank line, horizontal rule, citation, evidence list
- Signature row + QR + record fields + fine print
- Actions outside print: download / share (no-print)

## Notes

- Closest GG cousins: ceremonial panels + [[Components/QR Block]]
- Keep print CSS: hide shell/foot/toast; expand sheet

## Responsive

See [[Foundations/Breakpoints]].

Scale certificate surface to viewport width with margins; preserve print aspect. On mobile, offer download/print rather than tiny unreadable preview-only.

## Finalize
- [ ] Keep as Academy system-only unless another product needs certificates
- [ ] Mark status


---

<!-- FILE: Components/Chat Link Row.md -->
# Components/Chat Link Row.md

﻿---
title: Chat Link Row
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.chat, .tg)
---

# Chat Link Row

CTA row to open an external chat (e.g. Telegram community).

## Spec

- Paper card, 1px rule, 14px radius
- Leading brand tile 42×42 (channel color allowed as **local** accent — e.g. Telegram teal)
- Title: Inter Tight 600; sub: ink-3
- Whole row clickable; min height ~64px
- Hover: blue border or slight shadow
- Trailing chevron or “Open” text button

## Note

Channel brand color is an exception tile only — do not recolor the whole DS.

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** row. Title/meta truncate with ellipsis; trailing action stays visible.

## Finalize
- [ ] Mark **Final** if reused beyond Academy


---

<!-- FILE: Components/Date Picker.md -->
# Components/Date Picker.md

﻿---
title: Date Picker
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - Academy Event Row booking
---

# Date Picker

Choose a calendar day (booking, scheduling).

## Spec

- Trigger: Form Field–styled control showing selected date
- Popover panel: paper, rule, commerce radius, card shadow
- Month nav: icon buttons 44×44
- Day grid: 40–44px cells; today = blue outline; selected = blue fill + bone text
- Disabled / past days: ink-4
- Keyboard navigable grid

## Related

- List booking UI may use [[Components/Event Row]] instead of a full calendar

## Responsive

See [[Foundations/Breakpoints]].

Calendar panel ~280px; on mobile open as centered popover or bottom sheet so month grid is fully tappable. Chevron icon buttons dense 36px OK.

## Finalize
- [ ] Prefer native `input type="date"` styled as field when enough
- [ ] Mark **Final** when custom picker ships


---

<!-- FILE: Components/Definition List.md -->
# Components/Definition List.md

﻿---
title: Definition List
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - ConfirmRegistrationModal (.confirm-row)
  - RevealSection (.reveal-meta-row)
  - Admin doctor details
---

# Definition List

Term / value rows for confirmations and detail summaries.

## Spec

- Thin rule separators between rows
- Term: Fraunces italic **or** uppercase micro-label in ink-3
- Value: Inter Tight 500–700, ink
- Long identifiers: `overflow-wrap: anywhere`
- Used in modals, reveal meta, admin detail panes, shop order meta

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid**. Stack dt above dd on narrow widths if a side-by-side row would crush labels; from desktop, two-column rows OK.

## Finalize
- [ ] Pick term style per dialect (italic editorial vs micro-label admin)
- [ ] Mark **Final**


---

<!-- FILE: Components/Dialog.md -->
# Components/Dialog.md

---
title: Dialog
tags: [gutguard, design-system, components]
updated: 2026-08-13
status: draft
---

# Dialog

Structured overlay chrome: **header · body · footer**. Prefer this for confirm/detail flows that need a title, dismiss control, and explicit actions.

Overlay surface rules (backdrop, shadow, radius dialects) live on [[Components/Modal]]. Dialog is the **inner structure** that sits on that overlay.

## Anatomy

| Region | Content |
|---|---|
| **Header** | Fraunces title (`id` for `aria-labelledby`) + trailing [[Components/Icon Button]] close (`X` SVG, `aria-label="Close"`). Bottom 1px rule. |
| **Body** | Scrollable content; ink-2; 14–16px type; padding 16–24px |
| **Footer** | Right-aligned [[Components/Button]] pair — secondary **Cancel** + primary **Confirm**. Top 1px rule. Gap 10px. |

## Geometry

- Max width ~480–560px (product choice)
- Radius: **24px** commerce/partner · **0** editorial/admin
- Shadow: `0 24px 70–80px rgba(15,15,24,.22–.28)`
- Paper/bone fill; 1px rule border
- Close control: ≥44px hit target (36px dense admin OK)

## Header / footer defaults

**Header**
- Title: Fraunces 28–32px / 400; ink
- Close: Icon Button with Lucide-style `x` (24px viewBox, 2px stroke, `currentColor`)

**Footer**
- Cancel → secondary / ghost button
- Confirm → primary matching dialect (partner blue rounded · admin square ink/blue)
- Destructive confirms may use error-tinted primary — keep copy explicit

## Variants

| Variant | Notes |
|---|---|
| Commerce dialog | 24px radius; partner primary in footer |
| Admin dialog | Square; denser header; admin primary |
| Editorial dialog | Square; booth primary if used in registration |

## A11y

- `role="dialog"` + `aria-modal="true"`
- `aria-labelledby` → header title id
- Focus trap while open; restore focus on close
- Escape dismisses (unless destructive critical — product choice)
- Backdrop click dismiss optional; document per product

## Do / don’t

- **Do** use Icon Button + SVG for close — never text `✕` / `×`
- **Do** keep actions in the footer, not only in the body
- **Don’t** mix Dialog chrome with Drawer side-sheet layout (see [[Components/Drawer]])
- **Don’t** invent a second overlay language — share Modal backdrop tokens

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` | Width `min(100% - 32px, 520px)` or bottom-sheet style; body `max-height` ~50vh with scroll; footer buttons may stack full-width if two actions won’t fit |
| `≥ 900px` | Centered; max-width ~480–560px; footer actions in a row |

Close control stays ≥44px on mobile.

## Portable CSS

`.gg-dialog` · `.gg-dialog-header` · `.gg-dialog-body` · `.gg-dialog-footer` — see [[03 - Portable CSS Starter]]

## Showcase

`Showcase/index.html` → `#dialog`

## Finalize

- [ ] Align Doctors confirm modals to this anatomy
- [ ] Mark **Final**


---

<!-- FILE: Components/Drawer.md -->
# Components/Drawer.md

---
title: Drawer
tags: [gutguard, design-system, components]
updated: 2026-08-12
status: draft
sources:
  - GutGuard-Doctors-HTML/components/Shoplet.tsx
  - GutGuard-Doctors-HTML/components/GutguardSite.jsx (.sheet, .cart-drawer)
---

# Drawer

Sliding panel for basket, checkout, or mobile nav. Commerce-first.

## Anatomy

- Classes: `.shop-drawer-wrap`, `.shop-drawer-scrim`, `.shop-drawer`, `.shop-drawer-head`
- Scrim/backdrop shared with modal family
- Surface: paper, rule on exposed edge
- Inward corners **24px** on commerce
- Desktop: side drawer shadow `-22px 0 70px rgba(15,15,24,.22)`
- ≤720px: treat as bottom sheet (Shoplet behavior)

## Related

- Marketing mobile `.sheet` = full-screen menu variant of drawer/sheet
- Use [[Components/Button]] for footer CTAs

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` (and often `< 720px` in Shoplet) | **Bottom sheet** or full-height sheet for nav/basket — grab handle optional; top radius ~20–24px commerce |
| `≥ 900px` | **Side drawer** (typically right); fixed width ~280–360px; scrim + edge shadow |

Do not show a side drawer and bottom sheet for the same surface at once.

## Finalize

- [ ] Lock 720 vs 900 cut for shop basket (document product override if kept at 720)
- [ ] Mark **Final**


---

<!-- FILE: Components/Dropdown Menu.md -->
# Components/Dropdown Menu.md

﻿---
title: Dropdown Menu
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Dropdown Menu

Action overflow (`···`) and compact menus.

## Spec

- Trigger: icon button 44×44 or secondary text
- Panel: paper, 1px rule, commerce 10–14px radius (0 admin)
- Shadow: card-level
- Items: 44px min height, Inter Tight 14px / 600
- Hover/focus item: pale blue wash or blue text
- Destructive item: error red text
- Separators: rule-soft
- Keyboard: arrows, Enter, Escape; focus trap in menu
- Close on outside click

## Responsive

See [[Foundations/Breakpoints]].

Menu repositions to stay in viewport. On mobile, prefer full-width sheet/drawer for long action lists instead of a tiny anchored menu.

## Finalize
- [ ] Distinguish from Select field (forms use Form Field select)
- [ ] Mark **Final**


---

<!-- FILE: Components/Empty State.md -->
# Components/Empty State.md

﻿---
title: Empty State
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - .admin-wheel-empty, .shop-empty, .partner-empty-orders
---

# Empty State

Quiet placeholder when a list or panel has no data.

## Spec

- Bone surface; solid or dashed rule border
- Padding ~16–22px
- Main label ~14px bold; copy ~13px ink-3
- Optional single [[Components/Button]] secondary/text action
- Avoid large illustrations unless the destination system already uses them

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** inside the panel. Centered stack; comfortable padding on mobile (~22px).

## Finalize
- [ ] One class family across admin/shop/partner
- [ ] Mark **Final**


---

<!-- FILE: Components/Event Row.md -->
# Components/Event Row.md

﻿---
title: Event Row
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.ev, .datebox, .ev-place, .ev-meta, .ev-seats, .confirm)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Event Row

Bookable session row inside a requirement card.

## Anatomy

- Date tile (`.datebox`) — month + day number (display type)
- Place title + meta (time, venue) + seats line
- Confirm stack — [[Components/Button]] sm (book / booked / cancel)

## States

| State | Treatment |
|---|---|
| Available | Default card border |
| Mine / booked | `.ev.mine` gold border; button `.booked` |
| Full / disabled | Disabled button |

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid**. Stack time/meta under title on narrow screens; keep booking CTA full-width or trailing ≥44px.

## Finalize
- [ ] Remap gold booked state to GG tokens
- [ ] Mark status


---

<!-- FILE: Components/File Attachment.md -->
# Components/File Attachment.md

﻿---
title: File Attachment
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML (.admin-newsletter-upload, .registration-email-upload)
  - GutguardLifestyle.html (camera proof capture)
---

# File Attachment

Custom upload / attach control for HTML, images, and proofs. **Doctors look — never the browser’s native file-input chrome.**

## Hard rule

> [!danger] Hide the native control
> Use `<input type="file">` only as an invisible engine.
> - Visually hide it (clip / `sr-only` / off-screen) — do **not** leave the default “Choose file / No file chosen” UI visible
> - Open the picker via a custom [[Components/Button]] or by activating the drop zone / `<label>`
> - In React: `ref` + `input.click()`, or associate `<label htmlFor={id}>`

Products use `lucide-react` icons (`Upload`, `File`, `X`). Showcase uses the same SVG paths.

## Anatomy

| Part | Spec |
|---|---|
| **Drop zone** | Paper/bone; **1.5px dashed** rule; commerce radius 10–14px; centered stack |
| **Icon** | Lucide `Upload` (or `Image` for camera) — ink-3 → blue on hover/drag |
| **Title** | Inter Tight 700, ~15px |
| **Helper** | ink-3 13px — accepted types + max size |
| **Choose control** | Secondary [[Components/Button]] (≥44px) — not a raw file input |
| **Selected row** | Solid 1px rule · paper · type chip + name + meta + [[Components/Icon Button]] remove (`X`) |
| **Progress** | Optional bone-soft track, blue fill |
| **Error** | Red border on zone/row + helper in error-text / [[Components/Alert]] |
| **Loading** | [[Components/Spinner]] on Upload action |

## Variants

| Variant | Use |
|---|---|
| Drop zone | Admin newsletter / email HTML / multi-proof |
| Compact button | Single “Choose file” secondary — still hides native input |
| Camera capture | Lifestyle proof — `accept="image/*" capture="environment"`; same custom shell |

## States

| State | Treatment |
|---|---|
| Default | Dashed rule, bone fill |
| Hover / drag-over | Border + icon → blue; light blue wash |
| Focus-within | Gold focus ring on the interactive surface |
| Selected | Show file row; zone may collapse or stay as “replace” |
| Error | `--error` border; message below |
| Disabled | ink-4; no hover; input `disabled` |

## Implementation sketch

```html
<div class="gg-file">
  <input id="proof" class="gg-file__input" type="file" accept=".png,.jpg,image/*" />
  <label class="gg-file__zone" for="proof">
    <!-- upload SVG -->
    <strong>Drop image here</strong>
    <span>Max 5MB · PNG JPG</span>
    <span class="gg-button gg-button--secondary" aria-hidden="true">Choose file</span>
  </label>
  <!-- after select: .gg-file__row with name + Icon Button remove -->
</div>
```

## Rules

- Never rely on color alone for error
- Hit targets ≥44px (remove uses Icon Button)
- Helper text always lists types/size limits
- Ultramarine for primary **Upload** — not prototype blues
- Multi-file: stack rows; each row has its own remove

## Related

[[Components/Button]] · [[Components/Icon Button]] · [[Components/Alert]] · [[Components/Spinner]]

## Portable CSS

`.gg-file` · `.gg-file__input` · `.gg-file__zone` · `.gg-file__row` — see [[03 - Portable CSS Starter]]

## Showcase

`Showcase/index.html` → `#file`

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid**. Drop zone full width of form column. File row stacks meta under the name if needed; remove [[Components/Icon Button]] stays ≥44px and does not overflow off-screen.

## Finalize
- [ ] Confirm dashed (empty) vs solid (selected row) as the locked pair
- [ ] Mark **Final**


---

<!-- FILE: Components/Form Field.md -->
# Components/Form Field.md

﻿---
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


---

<!-- FILE: Components/Icon Button.md -->
# Components/Icon Button.md

﻿---
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


---

<!-- FILE: Components/Lang Toggle.md -->
# Components/Lang Toggle.md

﻿---
title: Lang Toggle
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.langs, .lang)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Lang Toggle

Compact language switcher (e.g. EN | Tagalog) inside document sheets.

## Spec

- Track: paper fill, 1px rule, radius 12px, padding 4px, gap 6px
- Segment: min touch 44px; `.lang.on` = selected
- Essentially a small [[Components/Segmented Control]]

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint — compact segmented control. Keep in masthead/toolbar without wrapping under 320px if possible.

## Finalize
- [ ] Merge into Segmented Control as `size: sm` variant, or keep named alias
- [ ] Mark status


---

<!-- FILE: Components/Masthead.md -->
# Components/Masthead.md

---
title: Masthead
tags: [gutguard, design-system, components, shell]
updated: 2026-08-12
status: draft
sources:
  - GutGuard-Doctors-HTML/components/Header.tsx
---

# Masthead

Editorial booth header for program moments (registration / wheel). Not a site IA nav.

## Anatomy

- Classes: `.masthead`, `.masthead-logos`, `.masthead-logo.gg/.tt`, `.masthead-x`, `.masthead-name`, `.masthead-edition`
- Dual logos (GutGuard × partner) with × mark
- Program name + edition / date label
- Hard-edged editorial dialect; sits above [[Components/Progress Rail]]

## Rules

- Keep ceremonial and compact — no nav links
- Use on booth/stage flows only
- Partner marks are content, not a new brand color

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** for booth pages. Stack or scale logos on `< 600px` so dual marks stay readable; keep hard-edged editorial dialect. No shell show/hide at 900px.

## Finalize

- [ ] Capture exact spacing from CSS
- [ ] Mark **Final** or demote to system-only if unused outside Doctors booth


---

<!-- FILE: Components/Modal.md -->
# Components/Modal.md

---
title: Modal
tags: [gutguard, design-system, components]
updated: 2026-08-12
status: draft
sources:
  - GutGuard-Doctors-HTML/components/ConfirmRegistrationModal.tsx
  - GutGuard-Doctors-HTML/app/admin/*/page.tsx
  - GutGuard-Doctors-HTML/components/Shoplet.tsx
---

# Modal

Focused overlay. Surface treatment only in DS; positioning follows implementation.

> [!important] Structured chrome
> For overlays with a **title, close icon, body, and footer actions**, prefer [[Components/Dialog]]. This note covers backdrop / shell variants (booth, admin, shop, Academy sheet).

## Anatomy

- Backdrop: `rgba(15,15,24,.58)`; optional blur 3px
- Surface: paper/bone, 1px rule
- Radius: **24px** commerce; **0** editorial/admin
- Shadow: `0 24px 70–80px rgba(15,15,24,.22–.28)`
- Header: bottom rule; Fraunces heading 28–38px
- Close: secondary control, ≥44px target
- Actions: [[Components/Button]] pair (primary + secondary)

## Variants in Doctors

| Variant | Classes |
|---|---|
| Booth confirm | `.modal-shell`, `.modal-backdrop`, `.confirm-modal` |
| Admin | `.admin-modal-backdrop`, `.admin-modal`, head/body/actions |
| Shop info | `.shop-modal-wrap`, `.shop-modal` |

## Academy sheet (from Gentrep)

| Variant | Classes | Notes |
|---|---|---|
| Bottom sheet / dialog | `.modal` + `.sheet` + `.grab` + `.sheet-head` | Mobile: align flex-end, top radius 20px; ≥900px: centered, full radius, max-width 560px |

Treat Academy `.sheet` as a Modal presentation (or shared with [[Components/Drawer]] bottom-sheet mode).

## A11y

Trap focus, restore on close, Escape to dismiss, mark page inert, label dialog.

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` | Prefer **bottom sheet** presentation when from Academy/mobile patterns (top radius ~20px, align flex-end); or full-width centered with side margins ≥16px |
| `≥ 900px` | Centered overlay; max-width ~560px; full radius per dialect (commerce 24px / admin 0) |

Structured title/close/footer chrome → [[Components/Dialog]].

## Finalize

- [ ] One modal shell API across booth/admin/shop
- [ ] Mark **Final**


---

<!-- FILE: Components/Notification Bell.md -->
# Components/Notification Bell.md

﻿---
title: Notification Bell
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutguardLifestyle.html (header bell + badge)
---

# Notification Bell

Header affordance for alerts + optional panel.

## Anatomy

- Icon button 44×44
- [[Components/Badge]] count pill (blue or ink) on corner
- Panel: paper dropdown under bell — list of notification rows
- Unread: pale blue wash or blue dot
- Empty: [[Components/Empty State]] compact

## Visual

- Doctors tokens only (no prototype amber flood on the badge — prefer blue count)

## Responsive

See [[Foundations/Breakpoints]].

Bell stays in chrome. Panel: anchored dropdown on desktop; on < 900px prefer full-width sheet under the top bar.

## Finalize
- [ ] Mark **Final**


---

<!-- FILE: Components/Pagination.md -->
# Components/Pagination.md

﻿---
title: Pagination
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML (.admin-pagination*)
---

# Pagination

Navigate long admin tables / lists.

## Anatomy

- Meta: “Showing 1–20 of 240” in ink-3
- Controls: Prev / Next square admin buttons
- Optional page-size select (admin field skin)
- Disabled at ends; ≥44px targets where possible

## Visual

- Square dialect with tables
- No pill page numbers unless commerce surface needs them — prefer Prev/Next + page select for ops density

## Responsive

See [[Foundations/Breakpoints]].

On < 900px, show prev/next + current page; collapse excess page numbers into ellipsis. Targets ≥44px where possible.

## Finalize
- [ ] Align with [[Components/Table]]
- [ ] Mark **Final**


---

<!-- FILE: Components/Progress Rail.md -->
# Components/Progress Rail.md

---
title: Progress Rail
tags: [gutguard, design-system, components]
updated: 2026-08-12
status: draft
sources:
  - GutGuard-Doctors-HTML/components/ProgressRail.tsx
---

# Progress Rail

Multi-step progress for booth flows.

## Anatomy

- Classes: `.rail`, `.rail-fill`, `.rail-dot` (+ `.active` / `.done`)
- Prop: `screen` (1–4) drives fill % and dot states
- Editorial / hard-edged; sits under [[Components/Masthead]]

## Rules

- Active / done communicated with color **and** state class (not color alone)
- Motion ~0.3–0.6s; honor reduced motion
- Reuse as a generic stepper only if step count stays small and labeled elsewhere

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** — full width of the booth column (often max ~440px on mobile). Dots stay evenly spaced; do not hide step markers on small screens — shorten labels instead if needed.

## Finalize

- [ ] Decide if this is core kit or booth system-only
- [ ] Mark status


---

<!-- FILE: Components/QR Block.md -->
# Components/QR Block.md

﻿---
title: QR Block
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - Admin doctor QR
  - PartnerPortal QR
---

# QR Block

Scannable QR presentation with actions.

## Spec

- QR modules on **pure white** (`#FFFFFF`) only — no paper texture behind modules
- Outer frame: 1px rule; commerce radius 14px; padding ~10px
- Actions: download / print / copy via [[Components/Button]] secondary or icon buttons
- Mode switch (shop vs profile): [[Components/Segmented Control]]

## Responsive

See [[Foundations/Breakpoints]].

Fixed QR art size with readable quiet zone; center in column on mobile. Mode switch ([[Components/Segmented Control]]) stacks above the QR when width is tight.

## Finalize
- [ ] Unify admin + partner QR layouts
- [ ] Mark **Final**


---

<!-- FILE: Components/Quantity Stepper.md -->
# Components/Quantity Stepper.md

﻿---
title: Quantity Stepper
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML (.shop-qty)
---

# Quantity Stepper

− / value / + control for shop and dosing.

## Spec (Doctors shop)

- Three-cell: ~36 / 34 / 36 visual widths
- Buttons: bone fill, rule border, weight 900, 36px high
- Only **outer** corners round (10px); interior edges square
- Center value: plain text, centered, Inter Tight
- Disabled at min/max
- Focus-visible gold on buttons

## Lifestyle dosing

- Same geometry; remap any prototype colors to bone/blue/ink

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint. Keep − / value / + targets ≥36–44px; do not compress below usable touch size.

## Finalize
- [ ] Mark **Final**


---

<!-- FILE: Components/Rank Ladder.md -->
# Components/Rank Ladder.md

﻿---
title: Rank Ladder
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.ladder, .rung, .ant, .lock)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Rank Ladder

Horizontal, scrollable rank chips for selecting progression level.

## Anatomy

- Track: `.ladder` — flex row, gap 8px, overflow-x auto
- Chip: `.rung` — padding ~10×15, radius 12px, border
- Label: display sans uppercase (Academy: Anton `.ant`)
- Lock meta: small mute text when locked
- Active: `.rung.on` — filled (boss: navy; GG: ink or blue)

## States

`default` · `on` · `locked`

## Desktop twin

Sidebar rank rows (`.side-rank`) should share selection state with the ladder — same data, two presentations.

## Responsive

See [[Foundations/Breakpoints]].

Horizontal scroll on narrow viewports; snap chips. Desktop may show more chips without scroll if space allows ([[Components/Rank Ladder]] desktop twin).

## Finalize
- [ ] Map display type to Fraunces or keep a condensed UI chip style in Inter Tight
- [ ] Mark **Final** or system-only if unused outside Academy


---

<!-- FILE: Components/Rank Plate.md -->
# Components/Rank Plate.md

﻿---
title: Rank Plate
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.plate, .plate-*, .hatch, .pips, .pip, .bar)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Rank Plate

Hero progress card for the active rank. Brand-forward.

## Anatomy

- Dark brand gradient surface, radius ~18px, white type
- Optional hatch texture + watermark mark
- Eyebrow rule row (gold tick + uppercase label)
- Large uppercase title
- Subline + footer (status text + diamond **pips**)
- Progress **bar** (gold fill on translucent track)
- Note line under bar

## States

| State | Treatment |
|---|---|
| In progress | Brand blue gradient |
| Done | Green gradient (`#1a7a49` → `#0f5a35` in boss) |
| Pip done / booked / missed | gold / soft gold / clay |

## GG remap notes

- Prefer ultramarine gradient over boss `#1f5d99`
- Use muted gold carefully for pips — may need a brighter semantic “progress” token
- Done state → DS success green (extend foundations if missing)

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** hero plate in the main column (mobile max ~440px pattern). Stack metrics on very narrow widths.

## Finalize
- [ ] Decide core kit vs Academy-only
- [ ] Mark status


---

<!-- FILE: Components/Requirement Timeline.md -->
# Components/Requirement Timeline.md

---
title: Requirement Timeline
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.reqs, .req, .spine, .rail, .node, .req-card)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Requirement Timeline

Vertical checklist of unlock requirements with a spine/rail and cards.

## Anatomy

```
(node)  ┌─ card ─────────────────┐
  │     │ TYPE (uppercase)       │
 rail   │ Title                  │
  │     │ Description            │
  │     │ [ Button ]             │
  │     │ optional Event Rows    │
        └────────────────────────┘
```

- Node states: default · done (gold fill) · booked (gold ring) · missed (clay)
- Card states: default · `.active` (blue border + soft blue shadow) · `.missed`
- Types seen: document · attendance · demonstration · derived

## Related

- Actions use [[Components/Button]]
- Attendance expand uses [[Components/Event Row]]
- Related spirit to [[Components/Task Item]] but richer

## Responsive

See [[Foundations/Breakpoints]].

Spine + cards in a single column on mobile; keep card padding readable. From desktop, same single column inside content well unless product specifies two-up.

## Finalize
- [ ] Unify node colors with GG semantic tokens
- [ ] Mark **Final** or system-only


---

<!-- FILE: Components/Search Field.md -->
# Components/Search Field.md

﻿---
title: Search Field
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Search Field

Filter / find control for tables and lists. Extends [[Components/Form Field]].

## Spec

- Commerce boxed field skin; leading search icon (ink-3)
- Optional clear (×) when value present
- min-height 44–48px; placeholder ink-4
- Focus: blue border + pale blue halo
- Debounce in product code — not a visual concern

## Admin

- Square corners when inside admin shell

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** — typically 100% of toolbar/column (max ~420px in demos). Clear control stays inside the field on narrow widths.

## Finalize
- [ ] Mark **Final**


---

<!-- FILE: Components/Section Label.md -->
# Components/Section Label.md

﻿---
title: Section Label
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/components/SectionLabel.tsx
---

# Section Label

Editorial eyebrow for booth/marketing sections.

## Spec

- Class: `.section-label` + italic numeral `.section-label-num`
- Optional 24px thin rule before label
- Number: Fraunces italic blue ~14px
- Label: uppercase micro tracking, ink-3 or blue
- Props: `number` + children

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint — inline editorial eyebrow. Allow wrap; keep number + label on one line when possible.

## Finalize
- [ ] Confirm whether marketing mono eyebrows stay a separate token
- [ ] Mark **Final** or system-only


---

<!-- FILE: Components/Segmented Control.md -->
# Components/Segmented Control.md

﻿---
title: Segmented Control
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/styles/globals.css (.shop-segment)
  - GutGuard-Doctors-HTML/components/PartnerPortal.tsx (.partner-qr-toggle)
  - GutGuard-Doctors-HTML/app/admin/wheel/page.tsx (.admin-doctor-qr-toggle)
---

# Segmented Control

Mutually exclusive choices in one compact track (not page-level tabs).

## Anatomy

- Track: bone-soft fill, 1px rule, **14px** radius (commerce); square acceptable in admin
- Padding/gap ~4px
- Segments ≥ 44px high; equal height
- Label: 12px / 800 / uppercase / `.08em` / ink-3
- Active: paper fill, ink text, low shadow `0 2px 7px rgba(15,15,24,.09)`
  - Alternate active (partner/admin toggles): blue fill, bone text

## Seen in Doctors as

| Use | Class |
|---|---|
| Shop trial / protocol | `.shop-segment` |
| Partner QR mode | `.partner-qr-toggle` |
| Admin doctor QR mode | `.admin-doctor-qr-toggle` |

## Seen in prototypes (remap to this component)

| Use | Evidence |
|---|---|
| Lifestyle Health / Team / Story | `.gg-tab` |
| Academy EN / Tagalog | `.langs` / `.lang` → also [[Components/Lang Toggle]] |

These should converge to one component with an `activeTone: paper | blue` option.

## vs Tabs

- **Segmented** = filter / mode inside a panel
- **Tabs** = switching major panels or admin sections

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid**. Segments share width equally; allow horizontal scroll only if more than ~4 segments. Min segment height ≥44px on mobile.

## Finalize
- [ ] One shared class / React component
- [ ] Document paper-active vs blue-active
- [ ] Mark **Final**


---

<!-- FILE: Components/Sidebar.md -->
# Components/Sidebar.md

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


---

<!-- FILE: Components/Skeleton.md -->
# Components/Skeleton.md

﻿---
title: Skeleton
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Skeleton

Placeholder shapes while content loads.

## Spec

- Bone-soft / bone-deep fills on paper
- Radius matches destination dialect (14px commerce cards, 0 admin)
- Subtle shimmer optional — disable under reduced motion
- Match approximate layout of final content (title line, avatar circle, rows)
- Never use as the only loading cue for screen readers — pair with `aria-busy` / live text

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** — mirrors the layout being loaded (1-col mobile / multi-col desktop).

## Finalize
- [ ] Mark **Final**


---

<!-- FILE: Components/Spinner.md -->
# Components/Spinner.md

﻿---
title: Spinner
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML (.spinner, .partner-spinner)
---

# Spinner

Loading indicator. Pair with text when the wait is >1s.

## Variants

| Variant | Spec |
|---|---|
| Inline | 18px ring, currentColor, on buttons |
| Block | 28–36px centered in a panel |
| Page | Centered on bone with optional “Loading…” ink-3 |

## Motion

- `.8s linear infinite` rotation
- Honor `prefers-reduced-motion` — slow pulse or static “Loading” text instead

## Color

- On bone/paper: blue or ink
- On blue/ink buttons: bone

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint. Center in the loading region; page-level spinner respects safe areas / bottom bar.

## Finalize
- [ ] One SVG/CSS recipe in portable CSS
- [ ] Mark **Final**


---

<!-- FILE: Components/Switch.md -->
# Components/Switch.md

﻿---
title: Switch
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Switch

Binary on/off control for settings. Prefer [[Components/Segmented Control]] when choosing among **named modes** (e.g. Trial / Protocol); use Switch for a single boolean.

## Spec

- Track: width ~44px · height ~26px · radius pill
- Thumb: ~20px circle · paper fill · subtle shadow
- Off: track `--bone-deep` / rule
- On: track `--blue`; thumb stays paper
- Focus-visible: gold ring on the control
- Optional label to the right (Inter Tight 14–15px / 600)

## A11y

- `role="switch"`
- `aria-checked="true|false"`
- Keyboard: Space / Enter toggles
- Associate with visible label via `aria-labelledby` or wrapping `<label>`

## Do / don’t

- **Do** animate thumb with short ease; respect `prefers-reduced-motion`
- **Don’t** use Switch for multi-option filters — use Segmented or checkboxes
- **Don’t** use purple/teal track fills — blue only when on

## Portable CSS

`.gg-switch` — see [[03 - Portable CSS Starter]]

## Showcase

`Showcase/index.html` → `#switch`

## Responsive

See [[Foundations/Breakpoints]].

No breakpoint. Keep 44×26 track; pair with label in a wrapping row. Touch target for the control ≥44px height via padding if needed.

## Finalize
- [ ] Mark **Final** when used in a second product


---

<!-- FILE: Components/Table.md -->
# Components/Table.md

﻿---
title: Table
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/app/admin/tiktok/page.tsx
  - GutGuard-Doctors-HTML/app/admin/orders/page.tsx
---

# Table

Dense admin data display.

## Spec

- Light rule dividers; bone/paper surfaces
- Header: 10–11px / 800–900 / uppercase / wide tracking / ink-3
- Cell: 12–15px ink; supporting line ink-3
- Row actions: compact square admin buttons
- Status: [[Components/Badge]] — not full-row color fills
- Align numbers consistently; tabular numerals when available
- Wrapper: scroll container for wide tables (`.admin-tiktok-table-wrap`)

## Related

- Doctor list rows (`.admin-doctor-row`) are a list/card hybrid — keep separate unless they become a true table
- Pagination: `.admin-pagination` family lives with Table for now

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| < 900px | Horizontal scroll in a ruled wrapper **or** cardized rows (product choice — document in repo). Keep actions reachable |
| ≥ 900px | Full table; sticky header optional |

Never hide critical columns without a detail drill-in.

## Finalize
- [ ] One table class (drop per-page duplicates)
- [ ] Document compact modifier
- [ ] Mark **Final**


---

<!-- FILE: Components/Tabs.md -->
# Components/Tabs.md

﻿---
title: Tabs
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/app/admin/wheel/page.tsx (.admin-tabs)
  - GutGuard-Doctors-HTML/app/admin/tiktok/page.tsx (.admin-tiktok-tabs)
  - GutGuard-Doctors-HTML/components/GutguardSite.jsx (.sectabs / .sectab)
---

# Tabs

Horizontal section switcher. Doctors admin uses this as **top chrome** (no sidebar).

## Variants

### 1. Admin tabs

- Classes: `.admin-tabs button` (+ `.active`); TikTok twin `.admin-tiktok-tabs`
- Track: transparent with rule-bottom
- Tab min-height ~42px; padding ~12px 18px
- Type: 11px / 800 / uppercase / `.16em`
- Inactive: ink-3, transparent 2px bottom border
- Hover + active: **blue fill**, bone text, blue bottom border
- Square corners

### 2. Marketing section tabs

- Classes: `.sectabs`, `.sectab` (+ `.on`)
- Used for in-page section jumping on the marketing site
- May use mono eyebrow styling (IBM Plex Mono in GutguardSite)
- Soften geometry only within marketing dialect

## Behavior

- One selected tab; expose `aria-current` or `aria-selected`
- Keyboard: arrow keys when used as a tablist
- Do not use tabs for primary app IA if a future system adds a sidebar — keep tabs for peer panels

## Do / don’t

- Do reuse one Admin Tabs skin across wheel / tiktok / orders
- Don’t invent a third admin tab class per page

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| < 900px | Horizontal scroll if tabs overflow; do not wrap into multiple rows |
| ≥ 900px | Full tab row in admin/marketing shell |

Active tab stays fully visible (scroll into view on change).

## Finalize
- [ ] Merge `.admin-tabs` and `.admin-tiktok-tabs` into one class name in code
- [ ] Decide whether marketing sectabs stay a Tabs variant or become “Section jump”
- [ ] Mark **Final**


---

<!-- FILE: Components/Task Item.md -->
# Components/Task Item.md

﻿---
title: Task Item
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/components/TaskItem.tsx
---

# Task Item

Checklist row for verification / onboarding steps.

## Spec

- Class: `.task` (+ `.done`)
- Number / title / meta; chevron → check when done
- Optional TikTok mark (`.task-tiktok-mark`) — content-specific
- Done state via class + icon change (not color alone)

## Responsive

See [[Foundations/Breakpoints]].

**Container-fluid** list rows. Chevron/actions stay trailing; title + meta may wrap. Min row height comfortable for touch (~48px).

## Finalize
- [ ] Keep in core kit if Academy/other systems need checklists; else system-only
- [ ] Mark status


---

<!-- FILE: Components/Toast.md -->
# Components/Toast.md

﻿---
title: Toast
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - GutGuard-Doctors-HTML/styles/globals.css (.admin-toast)
---

# Toast

Floating, temporary feedback.

## Spec

- Ink background, bone body text, subtle blue-translucent border
- Square; padding ~16px; shadow `0 20px 48px rgba(15,15,24,.28)`
- Title: success lime `#EAFF18` or error pink `#FFB8C2`; 12px / 800 / uppercase / `.12em`
- Body: bone 14px / 700 / 1.35
- Dismiss: translucent bone border; prefer 44px target
- Announce via `aria-live`

## Notes

Lime/pink title colors are **toast-only** — do not use as general success/error fills.

## Responsive

See [[Foundations/Breakpoints]].

Fixed position; max-width ~340px. On mobile, inset ≥16px from edges and sit **above** [[Components/Bottom Bar]] when that bar is visible.

## Finalize
- [ ] Promote beyond admin-only usage
- [ ] Mark **Final**


---

<!-- FILE: Components/Tooltip.md -->
# Components/Tooltip.md

﻿---
title: Tooltip
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
---

# Tooltip

Short helper on hover/focus. Not for essential instructions (use field helper text).

## Spec

- Ink fill, bone text, 12–13px / 600
- Padding ~8px 10px; radius 8px commerce / 0 editorial
- Soft shadow; max-width ~220px
- Arrow optional
- Appear on focus-visible as well as hover
- Delay ~300ms; dismiss on Escape
- Never trap focus inside a tooltip

## Responsive

See [[Foundations/Breakpoints]].

Prefer tooltips on hover/focus for desktop. On touch (< 900px or coarse pointer), use tap-to-toggle or move copy into visible helper text — do not rely on hover-only.

## Finalize
- [ ] Prefer Popover for interactive content — keep Tooltip text-only
- [ ] Mark **Final**


---

<!-- FILE: Components/Top Bar.md -->
# Components/Top Bar.md

---
title: Top Bar
aliases:
  - Site Header
  - App Header
tags: [gutguard, design-system, components, shell]
updated: 2026-08-12
status: draft
sources:
  - GutGuard-Doctors-HTML/components/Shoplet.tsx (.shop-site-header)
  - GutGuard-Doctors-HTML/components/GutguardSite.jsx (Nav)
  - GutGuard-Doctors-HTML/components/OrderStatus.tsx / PartnerPortal.tsx (.shop-nav)
---

# Top Bar

Horizontal chrome pinned to the **top** of public / commerce screens. This is the component formerly drafted as “Site Header.”

## Where it exists in Doctors

| Surface | Has top bar? | What you see instead |
|---|---|---|
| Shop (`Shoplet`) | **Yes** — fixed `.shop-site-header` | — |
| Marketing site | **Yes** — fixed `.nav` | — |
| Order status / partner | **Yes (light)** — `.shop-nav` strip | — |
| Admin (`/admin/*`) | **No** | Page hero (`.admin-wheel-hero`) + [[Components/Tabs]] |
| Booth registration | **No** | [[Components/Masthead]] (program header, not IA nav) |
| Gentrep Academy | **No** | Page `.mast` + desktop [[Components/Sidebar]] + mobile [[Components/Bottom Bar]] |
| GutGuard Lifestyle | **No** | In-page mast + [[Components/Sidebar]] + [[Components/Bottom Bar]] + [[Components/Segmented Control]] for Health/Team/Story |

So if you were looking at **admin**, you will not see a top bar — that screen never had one.

## Canonical anatomy (shop top bar — best reference)

```
┌─────────────────────────────────────────────────────────┐
│ ▬ heat→gold→recovery accent (2px)                       │
│  Brand     · Links · Links ·     Login    [Basket]      │
└─────────────────────────────────────────────────────────┘
```

- Fixed; `z-index: 100`
- Background: bone @ ~96% + `backdrop-filter: blur(14px)`
- Bottom border: `1px solid rgba(20,16,25,.08)`
- Soft shadow: `0 5px 14px rgba(20,16,25,.04)`
- Inner: max-width ~1320px; padding `12px 32px`
- Grid: brand | links | actions
- Links: 14px / 600 / ink-2; hover + current → blue; current gets 2px blue underline
- Actions slot: login text + basket (or CTA)
- Mobile: collapse links into menu / sheet

## Responsive

See [[Foundations/Breakpoints]].

| Viewport | Behavior |
|---|---|
| `< 900px` | Collapse link row into menu / sheet ([[Components/Drawer]]); keep brand + primary action visible; reduce horizontal padding (~16px) |
| `≥ 900px` | Full brand \| links \| actions grid; inner max-width ~1320px; padding ~12×32 |

Optional: at `< 600px`, icon-only basket/actions if labels collide.

## Variants

### 1. Full top bar (shop / marketing)

- Shop: `.shop-site-header` …
- Marketing: `.nav` (+ `.scrolled`) …
- Slots: brand · links · actions (CTA or basket)

### 2. Simple top bar

- `.shop-nav` + `.shop-brand` + `.shop-nav-link`
- Lightweight; used on order status / partner

## Visual rules

- Bone surface, ink text, blue for current/hover
- Focus-visible: 3px gold outline, 3px offset
- CTA / basket uses [[Components/Button]] patterns
- Mobile menu → sheet ([[Components/Drawer]] family)

## Not a top bar

- [[Components/Masthead]] — booth logos + edition
- [[Components/Admin Shell]] hero — large title block, not a nav bar
- [[Components/Tabs]] — sit under admin hero; not a top bar

## Sidebar

Doctors has **no sidebar**. If a later system adds one, create `Components/Sidebar.md` — do not stretch Top Bar to cover it.

## Finalize

- [ ] Lock full vs simple variants + measurements
- [ ] Unify shop + marketing into one Top Bar with slots
- [ ] Decide whether admin should ever get a top bar (today: no)
- [ ] Mark **Final**


---

<!-- FILE: Systems/README.md -->
# Systems/README.md

---
title: Systems
tags: [gutguard, design-system, systems]
updated: 2026-08-12
---

# Systems

One note per product scanned. Each note records where components were found and what became canonical.

| System | Note | Role |
|---|---|---|
| GutGuard Doctors HTML | [[Systems/Doctors-HTML]] | **Visual source of truth** |
| Gentrep Academy Dashboard | [[Systems/Gentrep-Academy-Dashboard]] | Prototype — structure only; remap to Doctors |
| GutGuard Lifestyle | [[Systems/GutGuard-Lifestyle]] | Prototype — structure only; remap to Doctors |

## When adding the next system

1. Read [[05 - Playbook]] — prototypes are structure only; Doctors is the look
2. Scan UI → list candidate components
3. Diff against [[Components/Index]]
4. Only create new component notes for net-new patterns
5. Record conflicts (same name, different look) on both the system note and the component note — resolve toward Doctors
6. Finalize variants; don’t fork a second design system


---

<!-- FILE: Systems/Doctors-HTML.md -->
# Systems/Doctors-HTML.md

---
title: System — GutGuard Doctors HTML
tags: [gutguard, design-system, systems, doctors]
source: C:\Users\najee\Projects\GutGuard-Doctors-HTML
scanned: 2026-08-12
updated: 2026-08-12
---

# System: GutGuard Doctors HTML

Primary source of the GutGuard design system. Scanned 2026-08-12.

## Role

This system established the brand tokens, three dialects, and most component skins. Later systems should **consume** the vault specs rather than invent parallel classes.

## Dialects in this system

| Dialect | Where | Edge language |
|---|---|---|
| Editorial (booth) | Registration experience + sections | Hard edges, masthead, ruled fields |
| Editorial (marketing) | `GutguardSite.jsx` | Softer radius, pill CTAs, mono eyebrows |
| Commerce | Shop, order status, partner portal | `--r-sm/md/lg/pill` |
| Admin | `/admin/wheel`, `/admin/tiktok`, `/admin/orders` | Hard edges, dense ops UI |

## Shell findings

- **No left sidebar** in this system.
- Admin chrome = hero strip + **horizontal tabs**.
- Marketing / shop use **top nav** (fixed or simple).
- Booth uses **masthead + progress rail** (narrow stage, max ~520px).

## Component harvest (canonical candidates)

| Candidate | Source evidence | Vault note |
|---|---|---|
| Button | `.action`, `.shop-primary`, `.btn-primary`, admin shell buttons | [[Components/Button]] |
| Form field | `FormField.tsx`, shop fields, admin inputs, partner OTP | [[Components/Form Field]] |
| Tabs | `.admin-tabs`, `.admin-tiktok-tabs`, marketing `.sectabs` | [[Components/Tabs]] |
| Segmented control | `.shop-segment`, `.partner-qr-toggle`, `.admin-doctor-qr-toggle` | [[Components/Segmented Control]] |
| Top bar | marketing `Nav`, `.shop-site-header`, `.shop-nav` | [[Components/Top Bar]] |
| Masthead | `Header.tsx` booth | [[Components/Masthead]] |
| Progress rail | `ProgressRail.tsx` | [[Components/Progress Rail]] |
| Card / panel | shop card, admin panel, partner auth card, order panel | [[Components/Card]] |
| Modal | confirm modal, admin modal, shop modal | [[Components/Modal]] |
| Drawer | shop basket/checkout drawer | [[Components/Drawer]] |
| Alert | admin alert, confirm warning, shop error, wheel notice | [[Components/Alert]] |
| Toast | `.admin-toast` | [[Components/Toast]] |
| Badge | `.partner-badge`, marketing beta tags, status pills | [[Components/Badge]] |
| Table | admin TikTok / orders tables | [[Components/Table]] |
| Definition list | confirm rows, reveal meta, admin doctor details | [[Components/Definition List]] |
| Empty state | admin / shop / partner empties | [[Components/Empty State]] |
| QR block | admin doctor QR, partner QR | [[Components/QR Block]] |
| Admin shell | `.admin-wheel-shell` family | [[Components/Admin Shell]] |
| Section label | `SectionLabel.tsx` | [[Components/Section Label]] |
| Task item | `TaskItem.tsx` | [[Components/Task Item]] |

## Brand specials (system-specific, document lightly)

Keep out of the core kit unless another system needs them:

- Prize wheel (`WheelSection`)
- Reveal stage (`RevealSection` — currently unused in live flow)
- Congrats banner CSS (orphaned — no JSX usage found)
- Marketing science visuals (MiAge, constellation, heat/recovery seam)
- Supplement facts panel

## Fragmentation to resolve in the DS

1. **Three button systems** — booth `.action`, shop `.shop-primary`, marketing `.btn-primary` → one [[Components/Button]] with dialect variants.
2. **Three form dialects** — ruled / boxed commerce / dense admin → one [[Components/Form Field]] with variants.
3. **Duplicate QR toggles** — partner vs admin → one [[Components/Segmented Control]].
4. **Duplicate empty / alert classes** → unify under Alert / Empty State notes.

## Source map

| Area | Paths |
|---|---|
| Tokens + skins | `styles/globals.css` |
| Booth components | `components/{ActionButton,FormField,Header,ProgressRail,ConfirmRegistrationModal,TaskItem,SectionLabel}.tsx` |
| Commerce | `components/{Shoplet,OrderStatus,PartnerPortal}.tsx` |
| Marketing | `components/GutguardSite.jsx` |
| Admin | `app/admin/{wheel,tiktok,orders}/page.tsx` |
| Booth sections | `sections/*` |

## Next systems

When scanning the next product, only add components that are **new** or that **conflict** with this harvest. Update this note’s harvest table if Doctors itself gains a sidebar or new chrome.


---

<!-- FILE: Systems/Gentrep-Academy-Dashboard.md -->
# Systems/Gentrep-Academy-Dashboard.md

---
title: System — Gentrep Academy Dashboard
tags: [gutguard, design-system, systems, academy, gentrep]
source: d:\Users\najee\Downloads\gentrep-academy-dashboard.html
inbox: GutGuard Design System/Inbox/gentrep-academy-dashboard/
scanned: 2026-08-12
updated: 2026-08-12
---
t
# System: Gentrep Academy Dashboard

**Prototype only.** Harvest structure and component shapes; **always restyle with** [[Systems/Doctors-HTML]] (bone, ultramarine, Fraunces, Inter Tight). Boss theme `m` below is remap reference — not DS tokens.

Boss input: single-file React SPA (minified). CSS is a template string driven by theme object `m`.

Also in vault: Inbox notes + Stitch run under `Inbox/gentrep-academy-dashboard/`.

## What this product is

A **rank ladder training dashboard**: pick a rank → see progress plate → complete requirements (docs, attendance booking, demos) → earn certificate. Mobile-first; desktop adds a left sidebar.

## Screens / surfaces

| Surface | How it appears |
|---|---|
| Ladder dashboard | Primary view — mast, ladder, plate, chat CTA, requirements timeline |
| About | Sheet — levels table + rules |
| Document reader | Sheet — agreement/ethics/creed + EN/TL lang toggle |
| Video | Sheet — poster + play |
| Booking | Inline expand inside requirement card — event rows |
| Certificate | Sheet / print — cream ceremonial card + QR |
| Toast + confetti | Completion feedback |

Ranks: **BASE → TL → SL → PL → CC**.

## Theme tokens (boss — not GutGuard)

```js
m = {
  navy: "#0e2249", navyD: "#07142e",
  blue: "#2569b8", sky: "#9DB8DE",
  paper: "#eef2f7", card: "#ffffff",
  ink: "#1a2740", mute: "#5a6b82",
  gold: "#f5b716", goldD: "#8a5a00",
  line: "#e2e8f0",
  good: "#157a43", goodBg: "#E4F4EC",
  warn: "#8a5a00", warnBg: "#FDF4E0",
  clay: "#a63a20", clayBg: "#FBEAE5",
  olive: "#3f4c37", oliveLt: "#EDEFE9",
  brand: "#1f5d99", brandD: "#163f66",
  tg: "#1373a2",
}
```

Fonts: **Anton** (display) · **Sora** (UI/buttons) · **Inter** (body) · **Playfair Display** italic (brand / cert name).

> When restyling into GutGuard, remap to bone / ultramarine / Fraunces / Inter Tight — see conflict table below. Do **not** treat boss colors as new DS tokens unless the team explicitly wants an Academy dialect.

## Shell (important)

| Chrome | Mobile | Desktop ≥900px |
|---|---|---|
| [[Components/Sidebar]] `.side` | **Hidden** | Sticky **280px** left rail |
| [[Components/Top Bar]] | **No fixed top bar** — page [[Components/Masthead\|mast]] only | Mast moves into main column; brand also in sidebar |
| [[Components/Bottom Bar]] `.foot` | Fixed sticky “Next” CTA | **Hidden** (sidebar `side-next` replaces it) |
| Main column `.col` | max-width 440px | Fluid inside shell max ~1240px |

This is the first scanned system with a real **sidebar** and **bottom bar**.

## Component harvest

### Map to existing DS components

| Candidate | Boss evidence | Vault note | Action |
|---|---|---|---|
| Button | `.btn` + primary/navy/tg/outline/danger/booked/sm/wide | [[Components/Button]] | Add Academy variants; remap colors to GG |
| Badge / pill | `.pill` | [[Components/Badge]] | Compact nav/about pill |
| Card | `.req-card`, `.chat`, `.ev` | [[Components/Card]] | Active/missed/mine borders |
| Modal / sheet | `.modal` + `.sheet` (bottom sheet mobile, centered desktop) | [[Components/Modal]] / [[Components/Drawer]] | Document sheet pattern |
| Toast | `.toast` | [[Components/Toast]] | Already exists |
| Alert / outcome | `.outcome` | [[Components/Alert]] | Success/olive bands |
| Progress (bar/pips) | `.bar`, `.pips` / `.pip` | related to [[Components/Progress Rail]] | Different metaphor — new or extend |
| Section label | `.bar-title` + `.sec` | [[Components/Section Label]] | Anton uppercase + hairline |
| Empty / fine copy | `.fine`, empty booking copy | [[Components/Empty State]] | Light use |

### New DS components (from this scan)

| Candidate | Classes | Vault note | Layer |
|---|---|---|---|
| **Sidebar** | `.side` `.who` `.avatar` `.side-nav` `.side-rank` `.side-btn` `.side-next` | [[Components/Sidebar]] | Shell |
| **Bottom Bar** | `.foot` `.foot-in` `.foot-title` `.eyebrow-dark` | [[Components/Bottom Bar]] | Shell |
| **Rank Ladder** | `.ladder` `.rung` `.ant` `.lock` | [[Components/Rank Ladder]] | Content |
| **Rank Plate** | `.plate` `.plate-*` `.hatch` `.pips` `.bar` | [[Components/Rank Plate]] | Brand-special |
| **Requirement Timeline** | `.reqs` `.req` `.spine` `.rail` `.node` `.req-card` | [[Components/Requirement Timeline]] | Content |
| **Event Row** | `.ev` `.datebox` `.ev-place` `.confirm` | [[Components/Event Row]] | Content |
| **Lang Toggle** | `.langs` `.lang` | [[Components/Lang Toggle]] | Content |
| **Certificate** | `.cert` `.cert-*` | [[Components/Certificate]] | Brand-special / system-only |
| **Chat CTA row** | `.chat` `.tg` | keep under Card or small “Link row” — see harvest note below | Content |

### System-only / don’t force into core kit yet

- Rank insignia metals (bronze / silver / gold seals)
- Confetti (`.cf-wrap`)
- Demo QA panel (`.demo`)
- Telegram brand tile color (`.tg`)
- Video poster (`.video` `.play`) and Doc reader (`.doc`) — simple sheet body patterns

## Anatomy snapshots

### Sidebar (desktop)

```
┌─ 280px sticky ─────────────┐
│ Gentrep (Playfair)         │
│ [avatar] Name · Team       │
│ ○ BASE                     │
│ ● TL          (on)         │
│ ○ SL  lock                 │
│ …                          │
│ [ About Academy ]          │
│ Do this next →             │
└────────────────────────────┘
```

### Mobile mast (not a Top Bar)

```
Gentrep Academy          [About]
Rey · Bravo
[ BASE ] [ TL ] [ SL ] …
```

### Bottom Bar (mobile)

```
┌────────────────────────────┐
│ DO THIS NEXT               │
│ Book Testimonial Session → │
└────────────────────────────┘
```

### Requirement row

```
(node)──┐
 rail   │  ┌ req-card ─────────────┐
        │  │ TYPE                  │
        │  │ Title                 │
        │  │ helper                │
        │  │ [ Action button ]     │
        │  │ optional .dates/.ev   │
        │  └───────────────────────┘
```

## Conflicts with GutGuard DS

| Axis | Academy boss | GutGuard | Decision needed |
|---|---|---|---|
| Canvas | cool `#eef2f7` | warm bone `#F4F1EA` | Remap to bone when implementing GG |
| Action blue | `#2569b8` | `#0608A9` | Remap |
| Brand navy | `#0e2249` fills + text | ink + ultramarine split | Don’t keep navy as primary action |
| Gold | bright `#f5b716` progress | muted `#B08D5B` accent | Need semantic “progress gold” vs premium gold |
| Fonts | Anton / Sora / Inter / Playfair | Fraunces / Inter Tight | Full remap |
| Focus ring | 3px blue | 3px gold | Follow GG (gold) |

Stitch Inbox run already used **commerce** dialect + bone — structure from this file, visuals from DS.

## Finalize priorities from this system

1. Lock [[Components/Sidebar]] + [[Components/Bottom Bar]] (new shell pieces)
2. Extend [[Components/Button]] / [[Components/Modal]] for sheet + booked/danger variants
3. Add Academy content components (Ladder, Plate, Timeline, Event Row)
4. Keep Certificate as system-special unless another product needs it


---

<!-- FILE: Systems/GutGuard-Lifestyle.md -->
# Systems/GutGuard-Lifestyle.md

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


---

<!-- FILE: Templates/AGENTS-design-system.md -->
# Templates/AGENTS-design-system.md

---
title: Template — AGENTS.md Design System gate
tags: [gutguard, design-system, template, cursor]
updated: 2026-08-12
---

# Template: paste into product `AGENTS.md`

Full instructions: [[07 - Using the DS with Cursor]] · Ownership: [[00 - OWNER — Read only]]

```markdown
# GutGuard UI — Design System gate

Before generating or changing any frontend (HTML, CSS, React, Stitch):

1. Read the Obsidian GutGuard Design System (synced vault) — **READ ONLY**.
2. Do **not** edit, create, or delete files inside `GutGuard Design System/`. Only the DS owner (Najee) may change the vault. Implement UI in this product repo only.
3. Minimum reads:
   - `GutGuard Design System/00 - OWNER — Read only.md`
   - `GutGuard Design System/00 - GutGuard Design System.md`
   - `GutGuard Design System/01 - Visual Foundations.md`
   - `GutGuard Design System/Foundations/Dialects.md`
   - `GutGuard Design System/Components/Index.md`
   - Component notes under `GutGuard Design System/Components/` for UI you touch
   - `GutGuard Design System/03 - Portable CSS Starter.md` for tokens/classes
4. Open `GutGuard Design System/Showcase/index.html` if unsure how a control should look.
5. Pick one dialect per screen (editorial / commerce / admin). Do not mix radius policies.
6. Visual source of truth = Doctors / vault — NOT boss prototypes (Academy, Lifestyle, etc.).
7. Recognition cues: bone `#F4F1EA`, blue `#0608A9`, ink `#0F0F18`, gold `#B08D5B`, Fraunces + Inter Tight, paper grain, uppercase micro-labels.

Local vault path — **each person sets their own** (synced Obsidian → `GutGuard Design System` folder):
`C:\Users\<you>\…\Obsidian Vault\GutGuard Design System\`

Workflow: vault `07 - Using the DS with Cursor.md` and `05 - Playbook.md`.
```

> After pasting into a repo, replace `<you>…` with the real path on that machine. Obsidian Sync keeps the *folder contents* the same; only the *disk location* differs.
> Need a DS change? Message the owner — don’t edit the vault on your PC.


---

<!-- FILE: Inbox/README.md -->
# Inbox/README.md

# Inbox

Drop boss HTML files or Next.js project zips/folders here.

Then in Cursor say:

> Run the GutGuard Stitch workflow on `GutGuard Design System/Inbox/<name>` using dialect `<editorial|commerce|admin>`.


---

<!-- FILE: Inbox/gentrep-academy-dashboard/NOTES.md -->
# Inbox/gentrep-academy-dashboard/NOTES.md

---
title: Gentrep Academy → GutGuard Stitch run
updated: 2026-08-12
---

# Gentrep Academy dashboard — Stitch run

## Input
- Boss file: `D:\Users\najee\Downloads\gentrep-academy-dashboard.html`
- Type: single-file React SPA (Gentrep Academy training dashboard)
- Dialect used: **commerce / partner**

## Stitch
- Project: `GutGuard × Gentrep Academy Dashboard`
- Project ID: `7912845079174759558`
- Open: https://stitch.withgoogle.com/projects/7912845079174759558
- Design system asset: `assets/1068384056446977363`
- Screen: `Gentrep Academy Dashboard` (`963d00a144484d948ce26af82a01bcc1`)

## Exports in this folder
- `gentrep-academy-dashboard.html` — original boss input (if copied)
- `stitch-screenshot.png` — generated preview
- `stitch-export.html` — generated HTML from Stitch

## Next options
- Add a detailed view for Testimonial Session
- Generate mobile version
- Strengthen muted gold on rank cards
- Implement into Next.js using `03 - Portable CSS Starter.md` (`gg-*` classes)
