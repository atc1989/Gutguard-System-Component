# GutGuard Design System — Compiled

Every file from the `GutGuard Design System` vault folder, concatenated in folder order. Source paths are shown above each section. Markdown notes are included verbatim; HTML/MDC files are included verbatim inside code blocks.

> Note: `Inbox/gentrep-academy-dashboard/stitch-screenshot.png` (binary image, 141 KB) is not included as text.

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
63. `Templates/gutguard-design-system.mdc`
64. `Inbox/README.md`
65. `Inbox/gentrep-academy-dashboard/gentrep-academy-dashboard.html`
66. `Inbox/gentrep-academy-dashboard/NOTES.md`
67. `Inbox/gentrep-academy-dashboard/stitch-export.html`
68. `Showcase/index.html`




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

<!-- FILE: Templates/gutguard-design-system.mdc -->
# Templates/gutguard-design-system.mdc

````markdown
---
description: Always read GutGuard Obsidian design system before any frontend work — never edit the vault
alwaysApply: true
---

# GutGuard Design System (required)

Before creating or editing UI (*.tsx, *.jsx, *.css, *.html, Stitch, layouts, components):

1. READ the Obsidian vault design system first. Do not invent a new look.
2. Set `GG_DS` to **this machine’s** path to the synced folder `GutGuard Design System`
   (everyone replaces this — do not keep a teammate’s PC path).

   Example:
   `GG_DS` = `C:\Users\<you>\OneDrive\Documents\Obsidian Vault\GutGuard Design System`

3. Required reads:
   - `{GG_DS}/00 - OWNER — Read only.md` (governance)
   - `{GG_DS}/00 - GutGuard Design System.md`
   - `{GG_DS}/01 - Visual Foundations.md`
   - `{GG_DS}/Foundations/Dialects.md`
   - `{GG_DS}/Components/Index.md`
4. Also read matching notes in `{GG_DS}/Components/` for every control you implement, and `{GG_DS}/03 - Portable CSS Starter.md` for CSS tokens. Optional: `{GG_DS}/Showcase/index.html`
5. Visual truth = Doctors + this vault. Prototypes only define structure/IA.
6. Use bone / ultramarine / Fraunces / Inter Tight. One dialect per screen.

## Hard rule — vault is read-only

- **NEVER** create, edit, rename, or delete files under `GutGuard Design System/` (Obsidian).
- Implement UI only in the **product repository**.
- If the design system itself needs a change, tell the user to ask the **owner (Najee)** — do not patch the vault from a teammate machine.
- If the vault path is missing or wrong, STOP and ask — do not freestyle UI.

Human guide: `{GG_DS}/07 - Using the DS with Cursor.md`
````


---

<!-- FILE: Inbox/README.md -->
# Inbox/README.md

# Inbox

Drop boss HTML files or Next.js project zips/folders here.

Then in Cursor say:

> Run the GutGuard Stitch workflow on `GutGuard Design System/Inbox/<name>` using dialect `<editorial|commerce|admin>`.



---

<!-- FILE: Inbox/gentrep-academy-dashboard/gentrep-academy-dashboard.html -->
# Inbox/gentrep-academy-dashboard/gentrep-academy-dashboard.html

````html
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover" />
<meta name="theme-color" content="#0e2249" />
<title>Gentrep Academy</title>
<style>html,body{margin:0;padding:0;background:#eef2f7;}#root{min-height:100vh;}</style>
</head>
<body>
<div id="root"></div>
<script>(()=>{var Td=Object.create;var Pa=Object.defineProperty;var Rd=Object.getOwnPropertyDescriptor;var Md=Object.getOwnPropertyNames;var Ad=Object.getPrototypeOf,Dd=Object.prototype.hasOwnProperty;var Xe=(e,t)=>()=>(t||e((t={exports:{}}).exports,t),t.exports);var $d=(e,t,n,r)=>{if(t&&typeof t=="object"||typeof t=="function")for(let l of Md(t))!Dd.call(e,l)&&l!==n&&Pa(e,l,{get:()=>t[l],enumerable:!(r=Rd(t,l))||r.enumerable});return e};var zn=(e,t,n)=>(n=e!=null?Td(Ad(e)):{},$d(t||!e||!e.__esModule?Pa(n,"default",{value:e,enumerable:!0}):n,e));var Ua=Xe(M=>{"use strict";var Pn=Symbol.for("react.element"),Od=Symbol.for("react.portal"),Id=Symbol.for("react.fragment"),Fd=Symbol.for("react.strict_mode"),jd=Symbol.for("react.profiler"),Bd=Symbol.for("react.provider"),Ud=Symbol.for("react.context"),Wd=Symbol.for("react.forward_ref"),Hd=Symbol.for("react.suspense"),Vd=Symbol.for("react.memo"),bd=Symbol.for("react.lazy"),Ta=Symbol.iterator;function Qd(e){return e===null||typeof e!="object"?null:(e=Ta&&e[Ta]||e["@@iterator"],typeof e=="function"?e:null)}var Aa={isMounted:function(){return!1},enqueueForceUpdate:function(){},enqueueReplaceState:function(){},enqueueSetState:function(){}},Da=Object.assign,$a={};function Kt(e,t,n){this.props=e,this.context=t,this.refs=$a,this.updater=n||Aa}Kt.prototype.isReactComponent={};Kt.prototype.setState=function(e,t){if(typeof e!="object"&&typeof e!="function"&&e!=null)throw Error("setState(...): takes an object of state variables to update or a function which returns an object of state variables.");this.updater.enqueueSetState(this,e,t,"setState")};Kt.prototype.forceUpdate=function(e){this.updater.enqueueForceUpdate(this,e,"forceUpdate")};function Oa(){}Oa.prototype=Kt.prototype;function Xl(e,t,n){this.props=e,this.context=t,this.refs=$a,this.updater=n||Aa}var Jl=Xl.prototype=new Oa;Jl.constructor=Xl;Da(Jl,Kt.prototype);Jl.isPureReactComponent=!0;var Ra=Array.isArray,Ia=Object.prototype.hasOwnProperty,ql={current:null},Fa={key:!0,ref:!0,__self:!0,__source:!0};function ja(e,t,n){var r,l={},o=null,i=null;if(t!=null)for(r in t.ref!==void 0&&(i=t.ref),t.key!==void 0&&(o=""+t.key),t)Ia.call(t,r)&&!Fa.hasOwnProperty(r)&&(l[r]=t[r]);var a=arguments.length-2;if(a===1)l.children=n;else if(1<a){for(var s=Array(a),d=0;d<a;d++)s[d]=arguments[d+2];l.children=s}if(e&&e.defaultProps)for(r in a=e.defaultProps,a)l[r]===void 0&&(l[r]=a[r]);return{$$typeof:Pn,type:e,key:o,ref:i,props:l,_owner:ql.current}}function Gd(e,t){return{$$typeof:Pn,type:e.type,key:t,ref:e.ref,props:e.props,_owner:e._owner}}function eo(e){return typeof e=="object"&&e!==null&&e.$$typeof===Pn}function Kd(e){var t={"=":"=0",":":"=2"};return"$"+e.replace(/[=:]/g,function(n){return t[n]})}var Ma=/\/+/g;function Zl(e,t){return typeof e=="object"&&e!==null&&e.key!=null?Kd(""+e.key):t.toString(36)}function Er(e,t,n,r,l){var o=typeof e;(o==="undefined"||o==="boolean")&&(e=null);var i=!1;if(e===null)i=!0;else switch(o){case"string":case"number":i=!0;break;case"object":switch(e.$$typeof){case Pn:case Od:i=!0}}if(i)return i=e,l=l(i),e=r===""?"."+Zl(i,0):r,Ra(l)?(n="",e!=null&&(n=e.replace(Ma,"$&/")+"/"),Er(l,t,n,"",function(d){return d})):l!=null&&(eo(l)&&(l=Gd(l,n+(!l.key||i&&i.key===l.key?"":(""+l.key).replace(Ma,"$&/")+"/")+e)),t.push(l)),1;if(i=0,r=r===""?".":r+":",Ra(e))for(var a=0;a<e.length;a++){o=e[a];var s=r+Zl(o,a);i+=Er(o,t,n,s,l)}else if(s=Qd(e),typeof s=="function")for(e=s.call(e),a=0;!(o=e.next()).done;)o=o.value,s=r+Zl(o,a++),i+=Er(o,t,n,s,l);else if(o==="object")throw t=String(e),Error("Objects are not valid as a React child (found: "+(t==="[object Object]"?"object with keys {"+Object.keys(e).join(", ")+"}":t)+"). If you meant to render a collection of children, use an array instead.");return i}function Sr(e,t,n){if(e==null)return e;var r=[],l=0;return Er(e,r,"","",function(o){return t.call(n,o,l++)}),r}function Yd(e){if(e._status===-1){var t=e._result;t=t(),t.then(function(n){(e._status===0||e._status===-1)&&(e._status=1,e._result=n)},function(n){(e._status===0||e._status===-1)&&(e._status=2,e._result=n)}),e._status===-1&&(e._status=0,e._result=t)}if(e._status===1)return e._result.default;throw e._result}var de={current:null},Nr={transition:null},Zd={ReactCurrentDispatcher:de,ReactCurrentBatchConfig:Nr,ReactCurrentOwner:ql};function Ba(){throw Error("act(...) is not supported in production builds of React.")}M.Children={map:Sr,forEach:function(e,t,n){Sr(e,function(){t.apply(this,arguments)},n)},count:function(e){var t=0;return Sr(e,function(){t++}),t},toArray:function(e){return Sr(e,function(t){return t})||[]},only:function(e){if(!eo(e))throw Error("React.Children.only expected to receive a single React element child.");return e}};M.Component=Kt;M.Fragment=Id;M.Profiler=jd;M.PureComponent=Xl;M.StrictMode=Fd;M.Suspense=Hd;M.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED=Zd;M.act=Ba;M.cloneElement=function(e,t,n){if(e==null)throw Error("React.cloneElement(...): The argument must be a React element, but you passed "+e+".");var r=Da({},e.props),l=e.key,o=e.ref,i=e._owner;if(t!=null){if(t.ref!==void 0&&(o=t.ref,i=ql.current),t.key!==void 0&&(l=""+t.key),e.type&&e.type.defaultProps)var a=e.type.defaultProps;for(s in t)Ia.call(t,s)&&!Fa.hasOwnProperty(s)&&(r[s]=t[s]===void 0&&a!==void 0?a[s]:t[s])}var s=arguments.length-2;if(s===1)r.children=n;else if(1<s){a=Array(s);for(var d=0;d<s;d++)a[d]=arguments[d+2];r.children=a}return{$$typeof:Pn,type:e.type,key:l,ref:o,props:r,_owner:i}};M.createContext=function(e){return e={$$typeof:Ud,_currentValue:e,_currentValue2:e,_threadCount:0,Provider:null,Consumer:null,_defaultValue:null,_globalName:null},e.Provider={$$typeof:Bd,_context:e},e.Consumer=e};M.createElement=ja;M.createFactory=function(e){var t=ja.bind(null,e);return t.type=e,t};M.createRef=function(){return{current:null}};M.forwardRef=function(e){return{$$typeof:Wd,render:e}};M.isValidElement=eo;M.lazy=function(e){return{$$typeof:bd,_payload:{_status:-1,_result:e},_init:Yd}};M.memo=function(e,t){return{$$typeof:Vd,type:e,compare:t===void 0?null:t}};M.startTransition=function(e){var t=Nr.transition;Nr.transition={};try{e()}finally{Nr.transition=t}};M.unstable_act=Ba;M.useCallback=function(e,t){return de.current.useCallback(e,t)};M.useContext=function(e){return de.current.useContext(e)};M.useDebugValue=function(){};M.useDeferredValue=function(e){return de.current.useDeferredValue(e)};M.useEffect=function(e,t){return de.current.useEffect(e,t)};M.useId=function(){return de.current.useId()};M.useImperativeHandle=function(e,t,n){return de.current.useImperativeHandle(e,t,n)};M.useInsertionEffect=function(e,t){return de.current.useInsertionEffect(e,t)};M.useLayoutEffect=function(e,t){return de.current.useLayoutEffect(e,t)};M.useMemo=function(e,t){return de.current.useMemo(e,t)};M.useReducer=function(e,t,n){return de.current.useReducer(e,t,n)};M.useRef=function(e){return de.current.useRef(e)};M.useState=function(e){return de.current.useState(e)};M.useSyncExternalStore=function(e,t,n){return de.current.useSyncExternalStore(e,t,n)};M.useTransition=function(){return de.current.useTransition()};M.version="18.3.1"});var Tn=Xe((h1,Wa)=>{"use strict";Wa.exports=Ua()});var Ja=Xe(I=>{"use strict";function lo(e,t){var n=e.length;e.push(t);e:for(;0<n;){var r=n-1>>>1,l=e[r];if(0<Lr(l,t))e[r]=t,e[n]=l,n=r;else break e}}function De(e){return e.length===0?null:e[0]}function zr(e){if(e.length===0)return null;var t=e[0],n=e.pop();if(n!==t){e[0]=n;e:for(var r=0,l=e.length,o=l>>>1;r<o;){var i=2*(r+1)-1,a=e[i],s=i+1,d=e[s];if(0>Lr(a,n))s<l&&0>Lr(d,a)?(e[r]=d,e[s]=n,r=s):(e[r]=a,e[i]=n,r=i);else if(s<l&&0>Lr(d,n))e[r]=d,e[s]=n,r=s;else break e}}return t}function Lr(e,t){var n=e.sortIndex-t.sortIndex;return n!==0?n:e.id-t.id}typeof performance=="object"&&typeof performance.now=="function"?(Ha=performance,I.unstable_now=function(){return Ha.now()}):(to=Date,Va=to.now(),I.unstable_now=function(){return to.now()-Va});var Ha,to,Va,We=[],st=[],Xd=1,_e=null,ie=3,Pr=!1,Mt=!1,Mn=!1,Ga=typeof setTimeout=="function"?setTimeout:null,Ka=typeof clearTimeout=="function"?clearTimeout:null,ba=typeof setImmediate<"u"?setImmediate:null;typeof navigator<"u"&&navigator.scheduling!==void 0&&navigator.scheduling.isInputPending!==void 0&&navigator.scheduling.isInputPending.bind(navigator.scheduling);function oo(e){for(var t=De(st);t!==null;){if(t.callback===null)zr(st);else if(t.startTime<=e)zr(st),t.sortIndex=t.expirationTime,lo(We,t);else break;t=De(st)}}function io(e){if(Mn=!1,oo(e),!Mt)if(De(We)!==null)Mt=!0,so(ao);else{var t=De(st);t!==null&&uo(io,t.startTime-e)}}function ao(e,t){Mt=!1,Mn&&(Mn=!1,Ka(An),An=-1),Pr=!0;var n=ie;try{for(oo(t),_e=De(We);_e!==null&&(!(_e.expirationTime>t)||e&&!Xa());){var r=_e.callback;if(typeof r=="function"){_e.callback=null,ie=_e.priorityLevel;var l=r(_e.expirationTime<=t);t=I.unstable_now(),typeof l=="function"?_e.callback=l:_e===De(We)&&zr(We),oo(t)}else zr(We);_e=De(We)}if(_e!==null)var o=!0;else{var i=De(st);i!==null&&uo(io,i.startTime-t),o=!1}return o}finally{_e=null,ie=n,Pr=!1}}var Tr=!1,_r=null,An=-1,Ya=5,Za=-1;function Xa(){return!(I.unstable_now()-Za<Ya)}function no(){if(_r!==null){var e=I.unstable_now();Za=e;var t=!0;try{t=_r(!0,e)}finally{t?Rn():(Tr=!1,_r=null)}}else Tr=!1}var Rn;typeof ba=="function"?Rn=function(){ba(no)}:typeof MessageChannel<"u"?(ro=new MessageChannel,Qa=ro.port2,ro.port1.onmessage=no,Rn=function(){Qa.postMessage(null)}):Rn=function(){Ga(no,0)};var ro,Qa;function so(e){_r=e,Tr||(Tr=!0,Rn())}function uo(e,t){An=Ga(function(){e(I.unstable_now())},t)}I.unstable_IdlePriority=5;I.unstable_ImmediatePriority=1;I.unstable_LowPriority=4;I.unstable_NormalPriority=3;I.unstable_Profiling=null;I.unstable_UserBlockingPriority=2;I.unstable_cancelCallback=function(e){e.callback=null};I.unstable_continueExecution=function(){Mt||Pr||(Mt=!0,so(ao))};I.unstable_forceFrameRate=function(e){0>e||125<e?console.error("forceFrameRate takes a positive int between 0 and 125, forcing frame rates higher than 125 fps is not supported"):Ya=0<e?Math.floor(1e3/e):5};I.unstable_getCurrentPriorityLevel=function(){return ie};I.unstable_getFirstCallbackNode=function(){return De(We)};I.unstable_next=function(e){switch(ie){case 1:case 2:case 3:var t=3;break;default:t=ie}var n=ie;ie=t;try{return e()}finally{ie=n}};I.unstable_pauseExecution=function(){};I.unstable_requestPaint=function(){};I.unstable_runWithPriority=function(e,t){switch(e){case 1:case 2:case 3:case 4:case 5:break;default:e=3}var n=ie;ie=e;try{return t()}finally{ie=n}};I.unstable_scheduleCallback=function(e,t,n){var r=I.unstable_now();switch(typeof n=="object"&&n!==null?(n=n.delay,n=typeof n=="number"&&0<n?r+n:r):n=r,e){case 1:var l=-1;break;case 2:l=250;break;case 5:l=1073741823;break;case 4:l=1e4;break;default:l=5e3}return l=n+l,e={id:Xd++,callback:t,priorityLevel:e,startTime:n,expirationTime:l,sortIndex:-1},n>r?(e.sortIndex=n,lo(st,e),De(We)===null&&e===De(st)&&(Mn?(Ka(An),An=-1):Mn=!0,uo(io,n-r))):(e.sortIndex=l,lo(We,e),Mt||Pr||(Mt=!0,so(ao))),e};I.unstable_shouldYield=Xa;I.unstable_wrapCallback=function(e){var t=ie;return function(){var n=ie;ie=t;try{return e.apply(this,arguments)}finally{ie=n}}}});var es=Xe((y1,qa)=>{"use strict";qa.exports=Ja()});var ld=Xe(Le=>{"use strict";var Jd=Tn(),Ee=es();function k(e){for(var t="https://reactjs.org/docs/error-decoder.html?invariant="+e,n=1;n<arguments.length;n++)t+="&args[]="+encodeURIComponent(arguments[n]);return"Minified React error #"+e+"; visit "+t+" for the full message or use the non-minified dev environment for full errors and additional helpful warnings."}var au=new Set,tr={};function bt(e,t){gn(e,t),gn(e+"Capture",t)}function gn(e,t){for(tr[e]=t,e=0;e<t.length;e++)au.add(t[e])}var rt=!(typeof window>"u"||typeof window.document>"u"||typeof window.document.createElement>"u"),Ao=Object.prototype.hasOwnProperty,qd=/^[:A-Z_a-z\u00C0-\u00D6\u00D8-\u00F6\u00F8-\u02FF\u0370-\u037D\u037F-\u1FFF\u200C-\u200D\u2070-\u218F\u2C00-\u2FEF\u3001-\uD7FF\uF900-\uFDCF\uFDF0-\uFFFD][:A-Z_a-z\u00C0-\u00D6\u00D8-\u00F6\u00F8-\u02FF\u0370-\u037D\u037F-\u1FFF\u200C-\u200D\u2070-\u218F\u2C00-\u2FEF\u3001-\uD7FF\uF900-\uFDCF\uFDF0-\uFFFD\-.0-9\u00B7\u0300-\u036F\u203F-\u2040]*$/,ts={},ns={};function ef(e){return Ao.call(ns,e)?!0:Ao.call(ts,e)?!1:qd.test(e)?ns[e]=!0:(ts[e]=!0,!1)}function tf(e,t,n,r){if(n!==null&&n.type===0)return!1;switch(typeof t){case"function":case"symbol":return!0;case"boolean":return r?!1:n!==null?!n.acceptsBooleans:(e=e.toLowerCase().slice(0,5),e!=="data-"&&e!=="aria-");default:return!1}}function nf(e,t,n,r){if(t===null||typeof t>"u"||tf(e,t,n,r))return!0;if(r)return!1;if(n!==null)switch(n.type){case 3:return!t;case 4:return t===!1;case 5:return isNaN(t);case 6:return isNaN(t)||1>t}return!1}function me(e,t,n,r,l,o,i){this.acceptsBooleans=t===2||t===3||t===4,this.attributeName=r,this.attributeNamespace=l,this.mustUseProperty=n,this.propertyName=e,this.type=t,this.sanitizeURL=o,this.removeEmptyString=i}var oe={};"children dangerouslySetInnerHTML defaultValue defaultChecked innerHTML suppressContentEditableWarning suppressHydrationWarning style".split(" ").forEach(function(e){oe[e]=new me(e,0,!1,e,null,!1,!1)});[["acceptCharset","accept-charset"],["className","class"],["htmlFor","for"],["httpEquiv","http-equiv"]].forEach(function(e){var t=e[0];oe[t]=new me(t,1,!1,e[1],null,!1,!1)});["contentEditable","draggable","spellCheck","value"].forEach(function(e){oe[e]=new me(e,2,!1,e.toLowerCase(),null,!1,!1)});["autoReverse","externalResourcesRequired","focusable","preserveAlpha"].forEach(function(e){oe[e]=new me(e,2,!1,e,null,!1,!1)});"allowFullScreen async autoFocus autoPlay controls default defer disabled disablePictureInPicture disableRemotePlayback formNoValidate hidden loop noModule noValidate open playsInline readOnly required reversed scoped seamless itemScope".split(" ").forEach(function(e){oe[e]=new me(e,3,!1,e.toLowerCase(),null,!1,!1)});["checked","multiple","muted","selected"].forEach(function(e){oe[e]=new me(e,3,!0,e,null,!1,!1)});["capture","download"].forEach(function(e){oe[e]=new me(e,4,!1,e,null,!1,!1)});["cols","rows","size","span"].forEach(function(e){oe[e]=new me(e,6,!1,e,null,!1,!1)});["rowSpan","start"].forEach(function(e){oe[e]=new me(e,5,!1,e.toLowerCase(),null,!1,!1)});var Ni=/[\-:]([a-z])/g;function Li(e){return e[1].toUpperCase()}"accent-height alignment-baseline arabic-form baseline-shift cap-height clip-path clip-rule color-interpolation color-interpolation-filters color-profile color-rendering dominant-baseline enable-background fill-opacity fill-rule flood-color flood-opacity font-family font-size font-size-adjust font-stretch font-style font-variant font-weight glyph-name glyph-orientation-horizontal glyph-orientation-vertical horiz-adv-x horiz-origin-x image-rendering letter-spacing lighting-color marker-end marker-mid marker-start overline-position overline-thickness paint-order panose-1 pointer-events rendering-intent shape-rendering stop-color stop-opacity strikethrough-position strikethrough-thickness stroke-dasharray stroke-dashoffset stroke-linecap stroke-linejoin stroke-miterlimit stroke-opacity stroke-width text-anchor text-decoration text-rendering underline-position underline-thickness unicode-bidi unicode-range units-per-em v-alphabetic v-hanging v-ideographic v-mathematical vector-effect vert-adv-y vert-origin-x vert-origin-y word-spacing writing-mode xmlns:xlink x-height".split(" ").forEach(function(e){var t=e.replace(Ni,Li);oe[t]=new me(t,1,!1,e,null,!1,!1)});"xlink:actuate xlink:arcrole xlink:role xlink:show xlink:title xlink:type".split(" ").forEach(function(e){var t=e.replace(Ni,Li);oe[t]=new me(t,1,!1,e,"http://www.w3.org/1999/xlink",!1,!1)});["xml:base","xml:lang","xml:space"].forEach(function(e){var t=e.replace(Ni,Li);oe[t]=new me(t,1,!1,e,"http://www.w3.org/XML/1998/namespace",!1,!1)});["tabIndex","crossOrigin"].forEach(function(e){oe[e]=new me(e,1,!1,e.toLowerCase(),null,!1,!1)});oe.xlinkHref=new me("xlinkHref",1,!1,"xlink:href","http://www.w3.org/1999/xlink",!0,!1);["src","href","action","formAction"].forEach(function(e){oe[e]=new me(e,1,!1,e.toLowerCase(),null,!0,!0)});function _i(e,t,n,r){var l=oe.hasOwnProperty(t)?oe[t]:null;(l!==null?l.type!==0:r||!(2<t.length)||t[0]!=="o"&&t[0]!=="O"||t[1]!=="n"&&t[1]!=="N")&&(nf(t,n,l,r)&&(n=null),r||l===null?ef(t)&&(n===null?e.removeAttribute(t):e.setAttribute(t,""+n)):l.mustUseProperty?e[l.propertyName]=n===null?l.type===3?!1:"":n:(t=l.attributeName,r=l.attributeNamespace,n===null?e.removeAttribute(t):(l=l.type,n=l===3||l===4&&n===!0?"":""+n,r?e.setAttributeNS(r,t,n):e.setAttribute(t,n))))}var at=Jd.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED,Rr=Symbol.for("react.element"),Xt=Symbol.for("react.portal"),Jt=Symbol.for("react.fragment"),zi=Symbol.for("react.strict_mode"),Do=Symbol.for("react.profiler"),su=Symbol.for("react.provider"),uu=Symbol.for("react.context"),Pi=Symbol.for("react.forward_ref"),$o=Symbol.for("react.suspense"),Oo=Symbol.for("react.suspense_list"),Ti=Symbol.for("react.memo"),ct=Symbol.for("react.lazy");Symbol.for("react.scope");Symbol.for("react.debug_trace_mode");var cu=Symbol.for("react.offscreen");Symbol.for("react.legacy_hidden");Symbol.for("react.cache");Symbol.for("react.tracing_marker");var rs=Symbol.iterator;function Dn(e){return e===null||typeof e!="object"?null:(e=rs&&e[rs]||e["@@iterator"],typeof e=="function"?e:null)}var b=Object.assign,co;function Wn(e){if(co===void 0)try{throw Error()}catch(n){var t=n.stack.trim().match(/\n( *(at )?)/);co=t&&t[1]||""}return`
`+co+e}var fo=!1;function po(e,t){if(!e||fo)return"";fo=!0;var n=Error.prepareStackTrace;Error.prepareStackTrace=void 0;try{if(t)if(t=function(){throw Error()},Object.defineProperty(t.prototype,"props",{set:function(){throw Error()}}),typeof Reflect=="object"&&Reflect.construct){try{Reflect.construct(t,[])}catch(d){var r=d}Reflect.construct(e,[],t)}else{try{t.call()}catch(d){r=d}e.call(t.prototype)}else{try{throw Error()}catch(d){r=d}e()}}catch(d){if(d&&r&&typeof d.stack=="string"){for(var l=d.stack.split(`
`),o=r.stack.split(`
`),i=l.length-1,a=o.length-1;1<=i&&0<=a&&l[i]!==o[a];)a--;for(;1<=i&&0<=a;i--,a--)if(l[i]!==o[a]){if(i!==1||a!==1)do if(i--,a--,0>a||l[i]!==o[a]){var s=`
`+l[i].replace(" at new "," at ");return e.displayName&&s.includes("<anonymous>")&&(s=s.replace("<anonymous>",e.displayName)),s}while(1<=i&&0<=a);break}}}finally{fo=!1,Error.prepareStackTrace=n}return(e=e?e.displayName||e.name:"")?Wn(e):""}function rf(e){switch(e.tag){case 5:return Wn(e.type);case 16:return Wn("Lazy");case 13:return Wn("Suspense");case 19:return Wn("SuspenseList");case 0:case 2:case 15:return e=po(e.type,!1),e;case 11:return e=po(e.type.render,!1),e;case 1:return e=po(e.type,!0),e;default:return""}}function Io(e){if(e==null)return null;if(typeof e=="function")return e.displayName||e.name||null;if(typeof e=="string")return e;switch(e){case Jt:return"Fragment";case Xt:return"Portal";case Do:return"Profiler";case zi:return"StrictMode";case $o:return"Suspense";case Oo:return"SuspenseList"}if(typeof e=="object")switch(e.$$typeof){case uu:return(e.displayName||"Context")+".Consumer";case su:return(e._context.displayName||"Context")+".Provider";case Pi:var t=e.render;return e=e.displayName,e||(e=t.displayName||t.name||"",e=e!==""?"ForwardRef("+e+")":"ForwardRef"),e;case Ti:return t=e.displayName||null,t!==null?t:Io(e.type)||"Memo";case ct:t=e._payload,e=e._init;try{return Io(e(t))}catch{}}return null}function lf(e){var t=e.type;switch(e.tag){case 24:return"Cache";case 9:return(t.displayName||"Context")+".Consumer";case 10:return(t._context.displayName||"Context")+".Provider";case 18:return"DehydratedFragment";case 11:return e=t.render,e=e.displayName||e.name||"",t.displayName||(e!==""?"ForwardRef("+e+")":"ForwardRef");case 7:return"Fragment";case 5:return t;case 4:return"Portal";case 3:return"Root";case 6:return"Text";case 16:return Io(t);case 8:return t===zi?"StrictMode":"Mode";case 22:return"Offscreen";case 12:return"Profiler";case 21:return"Scope";case 13:return"Suspense";case 19:return"SuspenseList";case 25:return"TracingMarker";case 1:case 0:case 17:case 2:case 14:case 15:if(typeof t=="function")return t.displayName||t.name||null;if(typeof t=="string")return t}return null}function Et(e){switch(typeof e){case"boolean":case"number":case"string":case"undefined":return e;case"object":return e;default:return""}}function du(e){var t=e.type;return(e=e.nodeName)&&e.toLowerCase()==="input"&&(t==="checkbox"||t==="radio")}function of(e){var t=du(e)?"checked":"value",n=Object.getOwnPropertyDescriptor(e.constructor.prototype,t),r=""+e[t];if(!e.hasOwnProperty(t)&&typeof n<"u"&&typeof n.get=="function"&&typeof n.set=="function"){var l=n.get,o=n.set;return Object.defineProperty(e,t,{configurable:!0,get:function(){return l.call(this)},set:function(i){r=""+i,o.call(this,i)}}),Object.defineProperty(e,t,{enumerable:n.enumerable}),{getValue:function(){return r},setValue:function(i){r=""+i},stopTracking:function(){e._valueTracker=null,delete e[t]}}}}function Mr(e){e._valueTracker||(e._valueTracker=of(e))}function fu(e){if(!e)return!1;var t=e._valueTracker;if(!t)return!0;var n=t.getValue(),r="";return e&&(r=du(e)?e.checked?"true":"false":e.value),e=r,e!==n?(t.setValue(e),!0):!1}function il(e){if(e=e||(typeof document<"u"?document:void 0),typeof e>"u")return null;try{return e.activeElement||e.body}catch{return e.body}}function Fo(e,t){var n=t.checked;return b({},t,{defaultChecked:void 0,defaultValue:void 0,value:void 0,checked:n??e._wrapperState.initialChecked})}function ls(e,t){var n=t.defaultValue==null?"":t.defaultValue,r=t.checked!=null?t.checked:t.defaultChecked;n=Et(t.value!=null?t.value:n),e._wrapperState={initialChecked:r,initialValue:n,controlled:t.type==="checkbox"||t.type==="radio"?t.checked!=null:t.value!=null}}function pu(e,t){t=t.checked,t!=null&&_i(e,"checked",t,!1)}function jo(e,t){pu(e,t);var n=Et(t.value),r=t.type;if(n!=null)r==="number"?(n===0&&e.value===""||e.value!=n)&&(e.value=""+n):e.value!==""+n&&(e.value=""+n);else if(r==="submit"||r==="reset"){e.removeAttribute("value");return}t.hasOwnProperty("value")?Bo(e,t.type,n):t.hasOwnProperty("defaultValue")&&Bo(e,t.type,Et(t.defaultValue)),t.checked==null&&t.defaultChecked!=null&&(e.defaultChecked=!!t.defaultChecked)}function os(e,t,n){if(t.hasOwnProperty("value")||t.hasOwnProperty("defaultValue")){var r=t.type;if(!(r!=="submit"&&r!=="reset"||t.value!==void 0&&t.value!==null))return;t=""+e._wrapperState.initialValue,n||t===e.value||(e.value=t),e.defaultValue=t}n=e.name,n!==""&&(e.name=""),e.defaultChecked=!!e._wrapperState.initialChecked,n!==""&&(e.name=n)}function Bo(e,t,n){(t!=="number"||il(e.ownerDocument)!==e)&&(n==null?e.defaultValue=""+e._wrapperState.initialValue:e.defaultValue!==""+n&&(e.defaultValue=""+n))}var Hn=Array.isArray;function cn(e,t,n,r){if(e=e.options,t){t={};for(var l=0;l<n.length;l++)t["$"+n[l]]=!0;for(n=0;n<e.length;n++)l=t.hasOwnProperty("$"+e[n].value),e[n].selected!==l&&(e[n].selected=l),l&&r&&(e[n].defaultSelected=!0)}else{for(n=""+Et(n),t=null,l=0;l<e.length;l++){if(e[l].value===n){e[l].selected=!0,r&&(e[l].defaultSelected=!0);return}t!==null||e[l].disabled||(t=e[l])}t!==null&&(t.selected=!0)}}function Uo(e,t){if(t.dangerouslySetInnerHTML!=null)throw Error(k(91));return b({},t,{value:void 0,defaultValue:void 0,children:""+e._wrapperState.initialValue})}function is(e,t){var n=t.value;if(n==null){if(n=t.children,t=t.defaultValue,n!=null){if(t!=null)throw Error(k(92));if(Hn(n)){if(1<n.length)throw Error(k(93));n=n[0]}t=n}t==null&&(t=""),n=t}e._wrapperState={initialValue:Et(n)}}function mu(e,t){var n=Et(t.value),r=Et(t.defaultValue);n!=null&&(n=""+n,n!==e.value&&(e.value=n),t.defaultValue==null&&e.defaultValue!==n&&(e.defaultValue=n)),r!=null&&(e.defaultValue=""+r)}function as(e){var t=e.textContent;t===e._wrapperState.initialValue&&t!==""&&t!==null&&(e.value=t)}function hu(e){switch(e){case"svg":return"http://www.w3.org/2000/svg";case"math":return"http://www.w3.org/1998/Math/MathML";default:return"http://www.w3.org/1999/xhtml"}}function Wo(e,t){return e==null||e==="http://www.w3.org/1999/xhtml"?hu(t):e==="http://www.w3.org/2000/svg"&&t==="foreignObject"?"http://www.w3.org/1999/xhtml":e}var Ar,gu=function(e){return typeof MSApp<"u"&&MSApp.execUnsafeLocalFunction?function(t,n,r,l){MSApp.execUnsafeLocalFunction(function(){return e(t,n,r,l)})}:e}(function(e,t){if(e.namespaceURI!=="http://www.w3.org/2000/svg"||"innerHTML"in e)e.innerHTML=t;else{for(Ar=Ar||document.createElement("div"),Ar.innerHTML="<svg>"+t.valueOf().toString()+"</svg>",t=Ar.firstChild;e.firstChild;)e.removeChild(e.firstChild);for(;t.firstChild;)e.appendChild(t.firstChild)}});function nr(e,t){if(t){var n=e.firstChild;if(n&&n===e.lastChild&&n.nodeType===3){n.nodeValue=t;return}}e.textContent=t}var Qn={animationIterationCount:!0,aspectRatio:!0,borderImageOutset:!0,borderImageSlice:!0,borderImageWidth:!0,boxFlex:!0,boxFlexGroup:!0,boxOrdinalGroup:!0,columnCount:!0,columns:!0,flex:!0,flexGrow:!0,flexPositive:!0,flexShrink:!0,flexNegative:!0,flexOrder:!0,gridArea:!0,gridRow:!0,gridRowEnd:!0,gridRowSpan:!0,gridRowStart:!0,gridColumn:!0,gridColumnEnd:!0,gridColumnSpan:!0,gridColumnStart:!0,fontWeight:!0,lineClamp:!0,lineHeight:!0,opacity:!0,order:!0,orphans:!0,tabSize:!0,widows:!0,zIndex:!0,zoom:!0,fillOpacity:!0,floodOpacity:!0,stopOpacity:!0,strokeDasharray:!0,strokeDashoffset:!0,strokeMiterlimit:!0,strokeOpacity:!0,strokeWidth:!0},af=["Webkit","ms","Moz","O"];Object.keys(Qn).forEach(function(e){af.forEach(function(t){t=t+e.charAt(0).toUpperCase()+e.substring(1),Qn[t]=Qn[e]})});function yu(e,t,n){return t==null||typeof t=="boolean"||t===""?"":n||typeof t!="number"||t===0||Qn.hasOwnProperty(e)&&Qn[e]?(""+t).trim():t+"px"}function vu(e,t){e=e.style;for(var n in t)if(t.hasOwnProperty(n)){var r=n.indexOf("--")===0,l=yu(n,t[n],r);n==="float"&&(n="cssFloat"),r?e.setProperty(n,l):e[n]=l}}var sf=b({menuitem:!0},{area:!0,base:!0,br:!0,col:!0,embed:!0,hr:!0,img:!0,input:!0,keygen:!0,link:!0,meta:!0,param:!0,source:!0,track:!0,wbr:!0});function Ho(e,t){if(t){if(sf[e]&&(t.children!=null||t.dangerouslySetInnerHTML!=null))throw Error(k(137,e));if(t.dangerouslySetInnerHTML!=null){if(t.children!=null)throw Error(k(60));if(typeof t.dangerouslySetInnerHTML!="object"||!("__html"in t.dangerouslySetInnerHTML))throw Error(k(61))}if(t.style!=null&&typeof t.style!="object")throw Error(k(62))}}function Vo(e,t){if(e.indexOf("-")===-1)return typeof t.is=="string";switch(e){case"annotation-xml":case"color-profile":case"font-face":case"font-face-src":case"font-face-uri":case"font-face-format":case"font-face-name":case"missing-glyph":return!1;default:return!0}}var bo=null;function Ri(e){return e=e.target||e.srcElement||window,e.correspondingUseElement&&(e=e.correspondingUseElement),e.nodeType===3?e.parentNode:e}var Qo=null,dn=null,fn=null;function ss(e){if(e=xr(e)){if(typeof Qo!="function")throw Error(k(280));var t=e.stateNode;t&&(t=Dl(t),Qo(e.stateNode,e.type,t))}}function ku(e){dn?fn?fn.push(e):fn=[e]:dn=e}function xu(){if(dn){var e=dn,t=fn;if(fn=dn=null,ss(e),t)for(e=0;e<t.length;e++)ss(t[e])}}function wu(e,t){return e(t)}function Cu(){}var mo=!1;function Su(e,t,n){if(mo)return e(t,n);mo=!0;try{return wu(e,t,n)}finally{mo=!1,(dn!==null||fn!==null)&&(Cu(),xu())}}function rr(e,t){var n=e.stateNode;if(n===null)return null;var r=Dl(n);if(r===null)return null;n=r[t];e:switch(t){case"onClick":case"onClickCapture":case"onDoubleClick":case"onDoubleClickCapture":case"onMouseDown":case"onMouseDownCapture":case"onMouseMove":case"onMouseMoveCapture":case"onMouseUp":case"onMouseUpCapture":case"onMouseEnter":(r=!r.disabled)||(e=e.type,r=!(e==="button"||e==="input"||e==="select"||e==="textarea")),e=!r;break e;default:e=!1}if(e)return null;if(n&&typeof n!="function")throw Error(k(231,t,typeof n));return n}var Go=!1;if(rt)try{Yt={},Object.defineProperty(Yt,"passive",{get:function(){Go=!0}}),window.addEventListener("test",Yt,Yt),window.removeEventListener("test",Yt,Yt)}catch{Go=!1}var Yt;function uf(e,t,n,r,l,o,i,a,s){var d=Array.prototype.slice.call(arguments,3);try{t.apply(n,d)}catch(g){this.onError(g)}}var Gn=!1,al=null,sl=!1,Ko=null,cf={onError:function(e){Gn=!0,al=e}};function df(e,t,n,r,l,o,i,a,s){Gn=!1,al=null,uf.apply(cf,arguments)}function ff(e,t,n,r,l,o,i,a,s){if(df.apply(this,arguments),Gn){if(Gn){var d=al;Gn=!1,al=null}else throw Error(k(198));sl||(sl=!0,Ko=d)}}function Qt(e){var t=e,n=e;if(e.alternate)for(;t.return;)t=t.return;else{e=t;do t=e,t.flags&4098&&(n=t.return),e=t.return;while(e)}return t.tag===3?n:null}function Eu(e){if(e.tag===13){var t=e.memoizedState;if(t===null&&(e=e.alternate,e!==null&&(t=e.memoizedState)),t!==null)return t.dehydrated}return null}function us(e){if(Qt(e)!==e)throw Error(k(188))}function pf(e){var t=e.alternate;if(!t){if(t=Qt(e),t===null)throw Error(k(188));return t!==e?null:e}for(var n=e,r=t;;){var l=n.return;if(l===null)break;var o=l.alternate;if(o===null){if(r=l.return,r!==null){n=r;continue}break}if(l.child===o.child){for(o=l.child;o;){if(o===n)return us(l),e;if(o===r)return us(l),t;o=o.sibling}throw Error(k(188))}if(n.return!==r.return)n=l,r=o;else{for(var i=!1,a=l.child;a;){if(a===n){i=!0,n=l,r=o;break}if(a===r){i=!0,r=l,n=o;break}a=a.sibling}if(!i){for(a=o.child;a;){if(a===n){i=!0,n=o,r=l;break}if(a===r){i=!0,r=o,n=l;break}a=a.sibling}if(!i)throw Error(k(189))}}if(n.alternate!==r)throw Error(k(190))}if(n.tag!==3)throw Error(k(188));return n.stateNode.current===n?e:t}function Nu(e){return e=pf(e),e!==null?Lu(e):null}function Lu(e){if(e.tag===5||e.tag===6)return e;for(e=e.child;e!==null;){var t=Lu(e);if(t!==null)return t;e=e.sibling}return null}var _u=Ee.unstable_scheduleCallback,cs=Ee.unstable_cancelCallback,mf=Ee.unstable_shouldYield,hf=Ee.unstable_requestPaint,K=Ee.unstable_now,gf=Ee.unstable_getCurrentPriorityLevel,Mi=Ee.unstable_ImmediatePriority,zu=Ee.unstable_UserBlockingPriority,ul=Ee.unstable_NormalPriority,yf=Ee.unstable_LowPriority,Pu=Ee.unstable_IdlePriority,Tl=null,Qe=null;function vf(e){if(Qe&&typeof Qe.onCommitFiberRoot=="function")try{Qe.onCommitFiberRoot(Tl,e,void 0,(e.current.flags&128)===128)}catch{}}var je=Math.clz32?Math.clz32:wf,kf=Math.log,xf=Math.LN2;function wf(e){return e>>>=0,e===0?32:31-(kf(e)/xf|0)|0}var Dr=64,$r=4194304;function Vn(e){switch(e&-e){case 1:return 1;case 2:return 2;case 4:return 4;case 8:return 8;case 16:return 16;case 32:return 32;case 64:case 128:case 256:case 512:case 1024:case 2048:case 4096:case 8192:case 16384:case 32768:case 65536:case 131072:case 262144:case 524288:case 1048576:case 2097152:return e&4194240;case 4194304:case 8388608:case 16777216:case 33554432:case 67108864:return e&130023424;case 134217728:return 134217728;case 268435456:return 268435456;case 536870912:return 536870912;case 1073741824:return 1073741824;default:return e}}function cl(e,t){var n=e.pendingLanes;if(n===0)return 0;var r=0,l=e.suspendedLanes,o=e.pingedLanes,i=n&268435455;if(i!==0){var a=i&~l;a!==0?r=Vn(a):(o&=i,o!==0&&(r=Vn(o)))}else i=n&~l,i!==0?r=Vn(i):o!==0&&(r=Vn(o));if(r===0)return 0;if(t!==0&&t!==r&&!(t&l)&&(l=r&-r,o=t&-t,l>=o||l===16&&(o&4194240)!==0))return t;if(r&4&&(r|=n&16),t=e.entangledLanes,t!==0)for(e=e.entanglements,t&=r;0<t;)n=31-je(t),l=1<<n,r|=e[n],t&=~l;return r}function Cf(e,t){switch(e){case 1:case 2:case 4:return t+250;case 8:case 16:case 32:case 64:case 128:case 256:case 512:case 1024:case 2048:case 4096:case 8192:case 16384:case 32768:case 65536:case 131072:case 262144:case 524288:case 1048576:case 2097152:return t+5e3;case 4194304:case 8388608:case 16777216:case 33554432:case 67108864:return-1;case 134217728:case 268435456:case 536870912:case 1073741824:return-1;default:return-1}}function Sf(e,t){for(var n=e.suspendedLanes,r=e.pingedLanes,l=e.expirationTimes,o=e.pendingLanes;0<o;){var i=31-je(o),a=1<<i,s=l[i];s===-1?(!(a&n)||a&r)&&(l[i]=Cf(a,t)):s<=t&&(e.expiredLanes|=a),o&=~a}}function Yo(e){return e=e.pendingLanes&-1073741825,e!==0?e:e&1073741824?1073741824:0}function Tu(){var e=Dr;return Dr<<=1,!(Dr&4194240)&&(Dr=64),e}function ho(e){for(var t=[],n=0;31>n;n++)t.push(e);return t}function vr(e,t,n){e.pendingLanes|=t,t!==536870912&&(e.suspendedLanes=0,e.pingedLanes=0),e=e.eventTimes,t=31-je(t),e[t]=n}function Ef(e,t){var n=e.pendingLanes&~t;e.pendingLanes=t,e.suspendedLanes=0,e.pingedLanes=0,e.expiredLanes&=t,e.mutableReadLanes&=t,e.entangledLanes&=t,t=e.entanglements;var r=e.eventTimes;for(e=e.expirationTimes;0<n;){var l=31-je(n),o=1<<l;t[l]=0,r[l]=-1,e[l]=-1,n&=~o}}function Ai(e,t){var n=e.entangledLanes|=t;for(e=e.entanglements;n;){var r=31-je(n),l=1<<r;l&t|e[r]&t&&(e[r]|=t),n&=~l}}var D=0;function Ru(e){return e&=-e,1<e?4<e?e&268435455?16:536870912:4:1}var Mu,Di,Au,Du,$u,Zo=!1,Or=[],gt=null,yt=null,vt=null,lr=new Map,or=new Map,ft=[],Nf="mousedown mouseup touchcancel touchend touchstart auxclick dblclick pointercancel pointerdown pointerup dragend dragstart drop compositionend compositionstart keydown keypress keyup input textInput copy cut paste click change contextmenu reset submit".split(" ");function ds(e,t){switch(e){case"focusin":case"focusout":gt=null;break;case"dragenter":case"dragleave":yt=null;break;case"mouseover":case"mouseout":vt=null;break;case"pointerover":case"pointerout":lr.delete(t.pointerId);break;case"gotpointercapture":case"lostpointercapture":or.delete(t.pointerId)}}function $n(e,t,n,r,l,o){return e===null||e.nativeEvent!==o?(e={blockedOn:t,domEventName:n,eventSystemFlags:r,nativeEvent:o,targetContainers:[l]},t!==null&&(t=xr(t),t!==null&&Di(t)),e):(e.eventSystemFlags|=r,t=e.targetContainers,l!==null&&t.indexOf(l)===-1&&t.push(l),e)}function Lf(e,t,n,r,l){switch(t){case"focusin":return gt=$n(gt,e,t,n,r,l),!0;case"dragenter":return yt=$n(yt,e,t,n,r,l),!0;case"mouseover":return vt=$n(vt,e,t,n,r,l),!0;case"pointerover":var o=l.pointerId;return lr.set(o,$n(lr.get(o)||null,e,t,n,r,l)),!0;case"gotpointercapture":return o=l.pointerId,or.set(o,$n(or.get(o)||null,e,t,n,r,l)),!0}return!1}function Ou(e){var t=$t(e.target);if(t!==null){var n=Qt(t);if(n!==null){if(t=n.tag,t===13){if(t=Eu(n),t!==null){e.blockedOn=t,$u(e.priority,function(){Au(n)});return}}else if(t===3&&n.stateNode.current.memoizedState.isDehydrated){e.blockedOn=n.tag===3?n.stateNode.containerInfo:null;return}}}e.blockedOn=null}function Zr(e){if(e.blockedOn!==null)return!1;for(var t=e.targetContainers;0<t.length;){var n=Xo(e.domEventName,e.eventSystemFlags,t[0],e.nativeEvent);if(n===null){n=e.nativeEvent;var r=new n.constructor(n.type,n);bo=r,n.target.dispatchEvent(r),bo=null}else return t=xr(n),t!==null&&Di(t),e.blockedOn=n,!1;t.shift()}return!0}function fs(e,t,n){Zr(e)&&n.delete(t)}function _f(){Zo=!1,gt!==null&&Zr(gt)&&(gt=null),yt!==null&&Zr(yt)&&(yt=null),vt!==null&&Zr(vt)&&(vt=null),lr.forEach(fs),or.forEach(fs)}function On(e,t){e.blockedOn===t&&(e.blockedOn=null,Zo||(Zo=!0,Ee.unstable_scheduleCallback(Ee.unstable_NormalPriority,_f)))}function ir(e){function t(l){return On(l,e)}if(0<Or.length){On(Or[0],e);for(var n=1;n<Or.length;n++){var r=Or[n];r.blockedOn===e&&(r.blockedOn=null)}}for(gt!==null&&On(gt,e),yt!==null&&On(yt,e),vt!==null&&On(vt,e),lr.forEach(t),or.forEach(t),n=0;n<ft.length;n++)r=ft[n],r.blockedOn===e&&(r.blockedOn=null);for(;0<ft.length&&(n=ft[0],n.blockedOn===null);)Ou(n),n.blockedOn===null&&ft.shift()}var pn=at.ReactCurrentBatchConfig,dl=!0;function zf(e,t,n,r){var l=D,o=pn.transition;pn.transition=null;try{D=1,$i(e,t,n,r)}finally{D=l,pn.transition=o}}function Pf(e,t,n,r){var l=D,o=pn.transition;pn.transition=null;try{D=4,$i(e,t,n,r)}finally{D=l,pn.transition=o}}function $i(e,t,n,r){if(dl){var l=Xo(e,t,n,r);if(l===null)Co(e,t,r,fl,n),ds(e,r);else if(Lf(l,e,t,n,r))r.stopPropagation();else if(ds(e,r),t&4&&-1<Nf.indexOf(e)){for(;l!==null;){var o=xr(l);if(o!==null&&Mu(o),o=Xo(e,t,n,r),o===null&&Co(e,t,r,fl,n),o===l)break;l=o}l!==null&&r.stopPropagation()}else Co(e,t,r,null,n)}}var fl=null;function Xo(e,t,n,r){if(fl=null,e=Ri(r),e=$t(e),e!==null)if(t=Qt(e),t===null)e=null;else if(n=t.tag,n===13){if(e=Eu(t),e!==null)return e;e=null}else if(n===3){if(t.stateNode.current.memoizedState.isDehydrated)return t.tag===3?t.stateNode.containerInfo:null;e=null}else t!==e&&(e=null);return fl=e,null}function Iu(e){switch(e){case"cancel":case"click":case"close":case"contextmenu":case"copy":case"cut":case"auxclick":case"dblclick":case"dragend":case"dragstart":case"drop":case"focusin":case"focusout":case"input":case"invalid":case"keydown":case"keypress":case"keyup":case"mousedown":case"mouseup":case"paste":case"pause":case"play":case"pointercancel":case"pointerdown":case"pointerup":case"ratechange":case"reset":case"resize":case"seeked":case"submit":case"touchcancel":case"touchend":case"touchstart":case"volumechange":case"change":case"selectionchange":case"textInput":case"compositionstart":case"compositionend":case"compositionupdate":case"beforeblur":case"afterblur":case"beforeinput":case"blur":case"fullscreenchange":case"focus":case"hashchange":case"popstate":case"select":case"selectstart":return 1;case"drag":case"dragenter":case"dragexit":case"dragleave":case"dragover":case"mousemove":case"mouseout":case"mouseover":case"pointermove":case"pointerout":case"pointerover":case"scroll":case"toggle":case"touchmove":case"wheel":case"mouseenter":case"mouseleave":case"pointerenter":case"pointerleave":return 4;case"message":switch(gf()){case Mi:return 1;case zu:return 4;case ul:case yf:return 16;case Pu:return 536870912;default:return 16}default:return 16}}var mt=null,Oi=null,Xr=null;function Fu(){if(Xr)return Xr;var e,t=Oi,n=t.length,r,l="value"in mt?mt.value:mt.textContent,o=l.length;for(e=0;e<n&&t[e]===l[e];e++);var i=n-e;for(r=1;r<=i&&t[n-r]===l[o-r];r++);return Xr=l.slice(e,1<r?1-r:void 0)}function Jr(e){var t=e.keyCode;return"charCode"in e?(e=e.charCode,e===0&&t===13&&(e=13)):e=t,e===10&&(e=13),32<=e||e===13?e:0}function Ir(){return!0}function ps(){return!1}function Ne(e){function t(n,r,l,o,i){this._reactName=n,this._targetInst=l,this.type=r,this.nativeEvent=o,this.target=i,this.currentTarget=null;for(var a in e)e.hasOwnProperty(a)&&(n=e[a],this[a]=n?n(o):o[a]);return this.isDefaultPrevented=(o.defaultPrevented!=null?o.defaultPrevented:o.returnValue===!1)?Ir:ps,this.isPropagationStopped=ps,this}return b(t.prototype,{preventDefault:function(){this.defaultPrevented=!0;var n=this.nativeEvent;n&&(n.preventDefault?n.preventDefault():typeof n.returnValue!="unknown"&&(n.returnValue=!1),this.isDefaultPrevented=Ir)},stopPropagation:function(){var n=this.nativeEvent;n&&(n.stopPropagation?n.stopPropagation():typeof n.cancelBubble!="unknown"&&(n.cancelBubble=!0),this.isPropagationStopped=Ir)},persist:function(){},isPersistent:Ir}),t}var Sn={eventPhase:0,bubbles:0,cancelable:0,timeStamp:function(e){return e.timeStamp||Date.now()},defaultPrevented:0,isTrusted:0},Ii=Ne(Sn),kr=b({},Sn,{view:0,detail:0}),Tf=Ne(kr),go,yo,In,Rl=b({},kr,{screenX:0,screenY:0,clientX:0,clientY:0,pageX:0,pageY:0,ctrlKey:0,shiftKey:0,altKey:0,metaKey:0,getModifierState:Fi,button:0,buttons:0,relatedTarget:function(e){return e.relatedTarget===void 0?e.fromElement===e.srcElement?e.toElement:e.fromElement:e.relatedTarget},movementX:function(e){return"movementX"in e?e.movementX:(e!==In&&(In&&e.type==="mousemove"?(go=e.screenX-In.screenX,yo=e.screenY-In.screenY):yo=go=0,In=e),go)},movementY:function(e){return"movementY"in e?e.movementY:yo}}),ms=Ne(Rl),Rf=b({},Rl,{dataTransfer:0}),Mf=Ne(Rf),Af=b({},kr,{relatedTarget:0}),vo=Ne(Af),Df=b({},Sn,{animationName:0,elapsedTime:0,pseudoElement:0}),$f=Ne(Df),Of=b({},Sn,{clipboardData:function(e){return"clipboardData"in e?e.clipboardData:window.clipboardData}}),If=Ne(Of),Ff=b({},Sn,{data:0}),hs=Ne(Ff),jf={Esc:"Escape",Spacebar:" ",Left:"ArrowLeft",Up:"ArrowUp",Right:"ArrowRight",Down:"ArrowDown",Del:"Delete",Win:"OS",Menu:"ContextMenu",Apps:"ContextMenu",Scroll:"ScrollLock",MozPrintableKey:"Unidentified"},Bf={8:"Backspace",9:"Tab",12:"Clear",13:"Enter",16:"Shift",17:"Control",18:"Alt",19:"Pause",20:"CapsLock",27:"Escape",32:" ",33:"PageUp",34:"PageDown",35:"End",36:"Home",37:"ArrowLeft",38:"ArrowUp",39:"ArrowRight",40:"ArrowDown",45:"Insert",46:"Delete",112:"F1",113:"F2",114:"F3",115:"F4",116:"F5",117:"F6",118:"F7",119:"F8",120:"F9",121:"F10",122:"F11",123:"F12",144:"NumLock",145:"ScrollLock",224:"Meta"},Uf={Alt:"altKey",Control:"ctrlKey",Meta:"metaKey",Shift:"shiftKey"};function Wf(e){var t=this.nativeEvent;return t.getModifierState?t.getModifierState(e):(e=Uf[e])?!!t[e]:!1}function Fi(){return Wf}var Hf=b({},kr,{key:function(e){if(e.key){var t=jf[e.key]||e.key;if(t!=="Unidentified")return t}return e.type==="keypress"?(e=Jr(e),e===13?"Enter":String.fromCharCode(e)):e.type==="keydown"||e.type==="keyup"?Bf[e.keyCode]||"Unidentified":""},code:0,location:0,ctrlKey:0,shiftKey:0,altKey:0,metaKey:0,repeat:0,locale:0,getModifierState:Fi,charCode:function(e){return e.type==="keypress"?Jr(e):0},keyCode:function(e){return e.type==="keydown"||e.type==="keyup"?e.keyCode:0},which:function(e){return e.type==="keypress"?Jr(e):e.type==="keydown"||e.type==="keyup"?e.keyCode:0}}),Vf=Ne(Hf),bf=b({},Rl,{pointerId:0,width:0,height:0,pressure:0,tangentialPressure:0,tiltX:0,tiltY:0,twist:0,pointerType:0,isPrimary:0}),gs=Ne(bf),Qf=b({},kr,{touches:0,targetTouches:0,changedTouches:0,altKey:0,metaKey:0,ctrlKey:0,shiftKey:0,getModifierState:Fi}),Gf=Ne(Qf),Kf=b({},Sn,{propertyName:0,elapsedTime:0,pseudoElement:0}),Yf=Ne(Kf),Zf=b({},Rl,{deltaX:function(e){return"deltaX"in e?e.deltaX:"wheelDeltaX"in e?-e.wheelDeltaX:0},deltaY:function(e){return"deltaY"in e?e.deltaY:"wheelDeltaY"in e?-e.wheelDeltaY:"wheelDelta"in e?-e.wheelDelta:0},deltaZ:0,deltaMode:0}),Xf=Ne(Zf),Jf=[9,13,27,32],ji=rt&&"CompositionEvent"in window,Kn=null;rt&&"documentMode"in document&&(Kn=document.documentMode);var qf=rt&&"TextEvent"in window&&!Kn,ju=rt&&(!ji||Kn&&8<Kn&&11>=Kn),ys=" ",vs=!1;function Bu(e,t){switch(e){case"keyup":return Jf.indexOf(t.keyCode)!==-1;case"keydown":return t.keyCode!==229;case"keypress":case"mousedown":case"focusout":return!0;default:return!1}}function Uu(e){return e=e.detail,typeof e=="object"&&"data"in e?e.data:null}var qt=!1;function ep(e,t){switch(e){case"compositionend":return Uu(t);case"keypress":return t.which!==32?null:(vs=!0,ys);case"textInput":return e=t.data,e===ys&&vs?null:e;default:return null}}function tp(e,t){if(qt)return e==="compositionend"||!ji&&Bu(e,t)?(e=Fu(),Xr=Oi=mt=null,qt=!1,e):null;switch(e){case"paste":return null;case"keypress":if(!(t.ctrlKey||t.altKey||t.metaKey)||t.ctrlKey&&t.altKey){if(t.char&&1<t.char.length)return t.char;if(t.which)return String.fromCharCode(t.which)}return null;case"compositionend":return ju&&t.locale!=="ko"?null:t.data;default:return null}}var np={color:!0,date:!0,datetime:!0,"datetime-local":!0,email:!0,month:!0,number:!0,password:!0,range:!0,search:!0,tel:!0,text:!0,time:!0,url:!0,week:!0};function ks(e){var t=e&&e.nodeName&&e.nodeName.toLowerCase();return t==="input"?!!np[e.type]:t==="textarea"}function Wu(e,t,n,r){ku(r),t=pl(t,"onChange"),0<t.length&&(n=new Ii("onChange","change",null,n,r),e.push({event:n,listeners:t}))}var Yn=null,ar=null;function rp(e){qu(e,0)}function Ml(e){var t=nn(e);if(fu(t))return e}function lp(e,t){if(e==="change")return t}var Hu=!1;rt&&(rt?(jr="oninput"in document,jr||(ko=document.createElement("div"),ko.setAttribute("oninput","return;"),jr=typeof ko.oninput=="function"),Fr=jr):Fr=!1,Hu=Fr&&(!document.documentMode||9<document.documentMode));var Fr,jr,ko;function xs(){Yn&&(Yn.detachEvent("onpropertychange",Vu),ar=Yn=null)}function Vu(e){if(e.propertyName==="value"&&Ml(ar)){var t=[];Wu(t,ar,e,Ri(e)),Su(rp,t)}}function op(e,t,n){e==="focusin"?(xs(),Yn=t,ar=n,Yn.attachEvent("onpropertychange",Vu)):e==="focusout"&&xs()}function ip(e){if(e==="selectionchange"||e==="keyup"||e==="keydown")return Ml(ar)}function ap(e,t){if(e==="click")return Ml(t)}function sp(e,t){if(e==="input"||e==="change")return Ml(t)}function up(e,t){return e===t&&(e!==0||1/e===1/t)||e!==e&&t!==t}var Ue=typeof Object.is=="function"?Object.is:up;function sr(e,t){if(Ue(e,t))return!0;if(typeof e!="object"||e===null||typeof t!="object"||t===null)return!1;var n=Object.keys(e),r=Object.keys(t);if(n.length!==r.length)return!1;for(r=0;r<n.length;r++){var l=n[r];if(!Ao.call(t,l)||!Ue(e[l],t[l]))return!1}return!0}function ws(e){for(;e&&e.firstChild;)e=e.firstChild;return e}function Cs(e,t){var n=ws(e);e=0;for(var r;n;){if(n.nodeType===3){if(r=e+n.textContent.length,e<=t&&r>=t)return{node:n,offset:t-e};e=r}e:{for(;n;){if(n.nextSibling){n=n.nextSibling;break e}n=n.parentNode}n=void 0}n=ws(n)}}function bu(e,t){return e&&t?e===t?!0:e&&e.nodeType===3?!1:t&&t.nodeType===3?bu(e,t.parentNode):"contains"in e?e.contains(t):e.compareDocumentPosition?!!(e.compareDocumentPosition(t)&16):!1:!1}function Qu(){for(var e=window,t=il();t instanceof e.HTMLIFrameElement;){try{var n=typeof t.contentWindow.location.href=="string"}catch{n=!1}if(n)e=t.contentWindow;else break;t=il(e.document)}return t}function Bi(e){var t=e&&e.nodeName&&e.nodeName.toLowerCase();return t&&(t==="input"&&(e.type==="text"||e.type==="search"||e.type==="tel"||e.type==="url"||e.type==="password")||t==="textarea"||e.contentEditable==="true")}function cp(e){var t=Qu(),n=e.focusedElem,r=e.selectionRange;if(t!==n&&n&&n.ownerDocument&&bu(n.ownerDocument.documentElement,n)){if(r!==null&&Bi(n)){if(t=r.start,e=r.end,e===void 0&&(e=t),"selectionStart"in n)n.selectionStart=t,n.selectionEnd=Math.min(e,n.value.length);else if(e=(t=n.ownerDocument||document)&&t.defaultView||window,e.getSelection){e=e.getSelection();var l=n.textContent.length,o=Math.min(r.start,l);r=r.end===void 0?o:Math.min(r.end,l),!e.extend&&o>r&&(l=r,r=o,o=l),l=Cs(n,o);var i=Cs(n,r);l&&i&&(e.rangeCount!==1||e.anchorNode!==l.node||e.anchorOffset!==l.offset||e.focusNode!==i.node||e.focusOffset!==i.offset)&&(t=t.createRange(),t.setStart(l.node,l.offset),e.removeAllRanges(),o>r?(e.addRange(t),e.extend(i.node,i.offset)):(t.setEnd(i.node,i.offset),e.addRange(t)))}}for(t=[],e=n;e=e.parentNode;)e.nodeType===1&&t.push({element:e,left:e.scrollLeft,top:e.scrollTop});for(typeof n.focus=="function"&&n.focus(),n=0;n<t.length;n++)e=t[n],e.element.scrollLeft=e.left,e.element.scrollTop=e.top}}var dp=rt&&"documentMode"in document&&11>=document.documentMode,en=null,Jo=null,Zn=null,qo=!1;function Ss(e,t,n){var r=n.window===n?n.document:n.nodeType===9?n:n.ownerDocument;qo||en==null||en!==il(r)||(r=en,"selectionStart"in r&&Bi(r)?r={start:r.selectionStart,end:r.selectionEnd}:(r=(r.ownerDocument&&r.ownerDocument.defaultView||window).getSelection(),r={anchorNode:r.anchorNode,anchorOffset:r.anchorOffset,focusNode:r.focusNode,focusOffset:r.focusOffset}),Zn&&sr(Zn,r)||(Zn=r,r=pl(Jo,"onSelect"),0<r.length&&(t=new Ii("onSelect","select",null,t,n),e.push({event:t,listeners:r}),t.target=en)))}function Br(e,t){var n={};return n[e.toLowerCase()]=t.toLowerCase(),n["Webkit"+e]="webkit"+t,n["Moz"+e]="moz"+t,n}var tn={animationend:Br("Animation","AnimationEnd"),animationiteration:Br("Animation","AnimationIteration"),animationstart:Br("Animation","AnimationStart"),transitionend:Br("Transition","TransitionEnd")},xo={},Gu={};rt&&(Gu=document.createElement("div").style,"AnimationEvent"in window||(delete tn.animationend.animation,delete tn.animationiteration.animation,delete tn.animationstart.animation),"TransitionEvent"in window||delete tn.transitionend.transition);function Al(e){if(xo[e])return xo[e];if(!tn[e])return e;var t=tn[e],n;for(n in t)if(t.hasOwnProperty(n)&&n in Gu)return xo[e]=t[n];return e}var Ku=Al("animationend"),Yu=Al("animationiteration"),Zu=Al("animationstart"),Xu=Al("transitionend"),Ju=new Map,Es="abort auxClick cancel canPlay canPlayThrough click close contextMenu copy cut drag dragEnd dragEnter dragExit dragLeave dragOver dragStart drop durationChange emptied encrypted ended error gotPointerCapture input invalid keyDown keyPress keyUp load loadedData loadedMetadata loadStart lostPointerCapture mouseDown mouseMove mouseOut mouseOver mouseUp paste pause play playing pointerCancel pointerDown pointerMove pointerOut pointerOver pointerUp progress rateChange reset resize seeked seeking stalled submit suspend timeUpdate touchCancel touchEnd touchStart volumeChange scroll toggle touchMove waiting wheel".split(" ");function Lt(e,t){Ju.set(e,t),bt(t,[e])}for(Ur=0;Ur<Es.length;Ur++)Wr=Es[Ur],Ns=Wr.toLowerCase(),Ls=Wr[0].toUpperCase()+Wr.slice(1),Lt(Ns,"on"+Ls);var Wr,Ns,Ls,Ur;Lt(Ku,"onAnimationEnd");Lt(Yu,"onAnimationIteration");Lt(Zu,"onAnimationStart");Lt("dblclick","onDoubleClick");Lt("focusin","onFocus");Lt("focusout","onBlur");Lt(Xu,"onTransitionEnd");gn("onMouseEnter",["mouseout","mouseover"]);gn("onMouseLeave",["mouseout","mouseover"]);gn("onPointerEnter",["pointerout","pointerover"]);gn("onPointerLeave",["pointerout","pointerover"]);bt("onChange","change click focusin focusout input keydown keyup selectionchange".split(" "));bt("onSelect","focusout contextmenu dragend focusin keydown keyup mousedown mouseup selectionchange".split(" "));bt("onBeforeInput",["compositionend","keypress","textInput","paste"]);bt("onCompositionEnd","compositionend focusout keydown keypress keyup mousedown".split(" "));bt("onCompositionStart","compositionstart focusout keydown keypress keyup mousedown".split(" "));bt("onCompositionUpdate","compositionupdate focusout keydown keypress keyup mousedown".split(" "));var bn="abort canplay canplaythrough durationchange emptied encrypted ended error loadeddata loadedmetadata loadstart pause play playing progress ratechange resize seeked seeking stalled suspend timeupdate volumechange waiting".split(" "),fp=new Set("cancel close invalid load scroll toggle".split(" ").concat(bn));function _s(e,t,n){var r=e.type||"unknown-event";e.currentTarget=n,ff(r,t,void 0,e),e.currentTarget=null}function qu(e,t){t=(t&4)!==0;for(var n=0;n<e.length;n++){var r=e[n],l=r.event;r=r.listeners;e:{var o=void 0;if(t)for(var i=r.length-1;0<=i;i--){var a=r[i],s=a.instance,d=a.currentTarget;if(a=a.listener,s!==o&&l.isPropagationStopped())break e;_s(l,a,d),o=s}else for(i=0;i<r.length;i++){if(a=r[i],s=a.instance,d=a.currentTarget,a=a.listener,s!==o&&l.isPropagationStopped())break e;_s(l,a,d),o=s}}}if(sl)throw e=Ko,sl=!1,Ko=null,e}function j(e,t){var n=t[li];n===void 0&&(n=t[li]=new Set);var r=e+"__bubble";n.has(r)||(ec(t,e,2,!1),n.add(r))}function wo(e,t,n){var r=0;t&&(r|=4),ec(n,e,r,t)}var Hr="_reactListening"+Math.random().toString(36).slice(2);function ur(e){if(!e[Hr]){e[Hr]=!0,au.forEach(function(n){n!=="selectionchange"&&(fp.has(n)||wo(n,!1,e),wo(n,!0,e))});var t=e.nodeType===9?e:e.ownerDocument;t===null||t[Hr]||(t[Hr]=!0,wo("selectionchange",!1,t))}}function ec(e,t,n,r){switch(Iu(t)){case 1:var l=zf;break;case 4:l=Pf;break;default:l=$i}n=l.bind(null,t,n,e),l=void 0,!Go||t!=="touchstart"&&t!=="touchmove"&&t!=="wheel"||(l=!0),r?l!==void 0?e.addEventListener(t,n,{capture:!0,passive:l}):e.addEventListener(t,n,!0):l!==void 0?e.addEventListener(t,n,{passive:l}):e.addEventListener(t,n,!1)}function Co(e,t,n,r,l){var o=r;if(!(t&1)&&!(t&2)&&r!==null)e:for(;;){if(r===null)return;var i=r.tag;if(i===3||i===4){var a=r.stateNode.containerInfo;if(a===l||a.nodeType===8&&a.parentNode===l)break;if(i===4)for(i=r.return;i!==null;){var s=i.tag;if((s===3||s===4)&&(s=i.stateNode.containerInfo,s===l||s.nodeType===8&&s.parentNode===l))return;i=i.return}for(;a!==null;){if(i=$t(a),i===null)return;if(s=i.tag,s===5||s===6){r=o=i;continue e}a=a.parentNode}}r=r.return}Su(function(){var d=o,g=Ri(n),v=[];e:{var y=Ju.get(e);if(y!==void 0){var w=Ii,S=e;switch(e){case"keypress":if(Jr(n)===0)break e;case"keydown":case"keyup":w=Vf;break;case"focusin":S="focus",w=vo;break;case"focusout":S="blur",w=vo;break;case"beforeblur":case"afterblur":w=vo;break;case"click":if(n.button===2)break e;case"auxclick":case"dblclick":case"mousedown":case"mousemove":case"mouseup":case"mouseout":case"mouseover":case"contextmenu":w=ms;break;case"drag":case"dragend":case"dragenter":case"dragexit":case"dragleave":case"dragover":case"dragstart":case"drop":w=Mf;break;case"touchcancel":case"touchend":case"touchmove":case"touchstart":w=Gf;break;case Ku:case Yu:case Zu:w=$f;break;case Xu:w=Yf;break;case"scroll":w=Tf;break;case"wheel":w=Xf;break;case"copy":case"cut":case"paste":w=If;break;case"gotpointercapture":case"lostpointercapture":case"pointercancel":case"pointerdown":case"pointermove":case"pointerout":case"pointerover":case"pointerup":w=gs}var C=(t&4)!==0,W=!C&&e==="scroll",f=C?y!==null?y+"Capture":null:y;C=[];for(var c=d,p;c!==null;){p=c;var x=p.stateNode;if(p.tag===5&&x!==null&&(p=x,f!==null&&(x=rr(c,f),x!=null&&C.push(cr(c,x,p)))),W)break;c=c.return}0<C.length&&(y=new w(y,S,null,n,g),v.push({event:y,listeners:C}))}}if(!(t&7)){e:{if(y=e==="mouseover"||e==="pointerover",w=e==="mouseout"||e==="pointerout",y&&n!==bo&&(S=n.relatedTarget||n.fromElement)&&($t(S)||S[lt]))break e;if((w||y)&&(y=g.window===g?g:(y=g.ownerDocument)?y.defaultView||y.parentWindow:window,w?(S=n.relatedTarget||n.toElement,w=d,S=S?$t(S):null,S!==null&&(W=Qt(S),S!==W||S.tag!==5&&S.tag!==6)&&(S=null)):(w=null,S=d),w!==S)){if(C=ms,x="onMouseLeave",f="onMouseEnter",c="mouse",(e==="pointerout"||e==="pointerover")&&(C=gs,x="onPointerLeave",f="onPointerEnter",c="pointer"),W=w==null?y:nn(w),p=S==null?y:nn(S),y=new C(x,c+"leave",w,n,g),y.target=W,y.relatedTarget=p,x=null,$t(g)===d&&(C=new C(f,c+"enter",S,n,g),C.target=p,C.relatedTarget=W,x=C),W=x,w&&S)t:{for(C=w,f=S,c=0,p=C;p;p=Zt(p))c++;for(p=0,x=f;x;x=Zt(x))p++;for(;0<c-p;)C=Zt(C),c--;for(;0<p-c;)f=Zt(f),p--;for(;c--;){if(C===f||f!==null&&C===f.alternate)break t;C=Zt(C),f=Zt(f)}C=null}else C=null;w!==null&&zs(v,y,w,C,!1),S!==null&&W!==null&&zs(v,W,S,C,!0)}}e:{if(y=d?nn(d):window,w=y.nodeName&&y.nodeName.toLowerCase(),w==="select"||w==="input"&&y.type==="file")var E=lp;else if(ks(y))if(Hu)E=sp;else{E=ip;var P=op}else(w=y.nodeName)&&w.toLowerCase()==="input"&&(y.type==="checkbox"||y.type==="radio")&&(E=ap);if(E&&(E=E(e,d))){Wu(v,E,n,g);break e}P&&P(e,y,d),e==="focusout"&&(P=y._wrapperState)&&P.controlled&&y.type==="number"&&Bo(y,"number",y.value)}switch(P=d?nn(d):window,e){case"focusin":(ks(P)||P.contentEditable==="true")&&(en=P,Jo=d,Zn=null);break;case"focusout":Zn=Jo=en=null;break;case"mousedown":qo=!0;break;case"contextmenu":case"mouseup":case"dragend":qo=!1,Ss(v,n,g);break;case"selectionchange":if(dp)break;case"keydown":case"keyup":Ss(v,n,g)}var _;if(ji)e:{switch(e){case"compositionstart":var T="onCompositionStart";break e;case"compositionend":T="onCompositionEnd";break e;case"compositionupdate":T="onCompositionUpdate";break e}T=void 0}else qt?Bu(e,n)&&(T="onCompositionEnd"):e==="keydown"&&n.keyCode===229&&(T="onCompositionStart");T&&(ju&&n.locale!=="ko"&&(qt||T!=="onCompositionStart"?T==="onCompositionEnd"&&qt&&(_=Fu()):(mt=g,Oi="value"in mt?mt.value:mt.textContent,qt=!0)),P=pl(d,T),0<P.length&&(T=new hs(T,e,null,n,g),v.push({event:T,listeners:P}),_?T.data=_:(_=Uu(n),_!==null&&(T.data=_)))),(_=qf?ep(e,n):tp(e,n))&&(d=pl(d,"onBeforeInput"),0<d.length&&(g=new hs("onBeforeInput","beforeinput",null,n,g),v.push({event:g,listeners:d}),g.data=_))}qu(v,t)})}function cr(e,t,n){return{instance:e,listener:t,currentTarget:n}}function pl(e,t){for(var n=t+"Capture",r=[];e!==null;){var l=e,o=l.stateNode;l.tag===5&&o!==null&&(l=o,o=rr(e,n),o!=null&&r.unshift(cr(e,o,l)),o=rr(e,t),o!=null&&r.push(cr(e,o,l))),e=e.return}return r}function Zt(e){if(e===null)return null;do e=e.return;while(e&&e.tag!==5);return e||null}function zs(e,t,n,r,l){for(var o=t._reactName,i=[];n!==null&&n!==r;){var a=n,s=a.alternate,d=a.stateNode;if(s!==null&&s===r)break;a.tag===5&&d!==null&&(a=d,l?(s=rr(n,o),s!=null&&i.unshift(cr(n,s,a))):l||(s=rr(n,o),s!=null&&i.push(cr(n,s,a)))),n=n.return}i.length!==0&&e.push({event:t,listeners:i})}var pp=/\r\n?/g,mp=/\u0000|\uFFFD/g;function Ps(e){return(typeof e=="string"?e:""+e).replace(pp,`
`).replace(mp,"")}function Vr(e,t,n){if(t=Ps(t),Ps(e)!==t&&n)throw Error(k(425))}function ml(){}var ei=null,ti=null;function ni(e,t){return e==="textarea"||e==="noscript"||typeof t.children=="string"||typeof t.children=="number"||typeof t.dangerouslySetInnerHTML=="object"&&t.dangerouslySetInnerHTML!==null&&t.dangerouslySetInnerHTML.__html!=null}var ri=typeof setTimeout=="function"?setTimeout:void 0,hp=typeof clearTimeout=="function"?clearTimeout:void 0,Ts=typeof Promise=="function"?Promise:void 0,gp=typeof queueMicrotask=="function"?queueMicrotask:typeof Ts<"u"?function(e){return Ts.resolve(null).then(e).catch(yp)}:ri;function yp(e){setTimeout(function(){throw e})}function So(e,t){var n=t,r=0;do{var l=n.nextSibling;if(e.removeChild(n),l&&l.nodeType===8)if(n=l.data,n==="/$"){if(r===0){e.removeChild(l),ir(t);return}r--}else n!=="$"&&n!=="$?"&&n!=="$!"||r++;n=l}while(n);ir(t)}function kt(e){for(;e!=null;e=e.nextSibling){var t=e.nodeType;if(t===1||t===3)break;if(t===8){if(t=e.data,t==="$"||t==="$!"||t==="$?")break;if(t==="/$")return null}}return e}function Rs(e){e=e.previousSibling;for(var t=0;e;){if(e.nodeType===8){var n=e.data;if(n==="$"||n==="$!"||n==="$?"){if(t===0)return e;t--}else n==="/$"&&t++}e=e.previousSibling}return null}var En=Math.random().toString(36).slice(2),be="__reactFiber$"+En,dr="__reactProps$"+En,lt="__reactContainer$"+En,li="__reactEvents$"+En,vp="__reactListeners$"+En,kp="__reactHandles$"+En;function $t(e){var t=e[be];if(t)return t;for(var n=e.parentNode;n;){if(t=n[lt]||n[be]){if(n=t.alternate,t.child!==null||n!==null&&n.child!==null)for(e=Rs(e);e!==null;){if(n=e[be])return n;e=Rs(e)}return t}e=n,n=e.parentNode}return null}function xr(e){return e=e[be]||e[lt],!e||e.tag!==5&&e.tag!==6&&e.tag!==13&&e.tag!==3?null:e}function nn(e){if(e.tag===5||e.tag===6)return e.stateNode;throw Error(k(33))}function Dl(e){return e[dr]||null}var oi=[],rn=-1;function _t(e){return{current:e}}function B(e){0>rn||(e.current=oi[rn],oi[rn]=null,rn--)}function F(e,t){rn++,oi[rn]=e.current,e.current=t}var Nt={},ce=_t(Nt),ye=_t(!1),Bt=Nt;function yn(e,t){var n=e.type.contextTypes;if(!n)return Nt;var r=e.stateNode;if(r&&r.__reactInternalMemoizedUnmaskedChildContext===t)return r.__reactInternalMemoizedMaskedChildContext;var l={},o;for(o in n)l[o]=t[o];return r&&(e=e.stateNode,e.__reactInternalMemoizedUnmaskedChildContext=t,e.__reactInternalMemoizedMaskedChildContext=l),l}function ve(e){return e=e.childContextTypes,e!=null}function hl(){B(ye),B(ce)}function Ms(e,t,n){if(ce.current!==Nt)throw Error(k(168));F(ce,t),F(ye,n)}function tc(e,t,n){var r=e.stateNode;if(t=t.childContextTypes,typeof r.getChildContext!="function")return n;r=r.getChildContext();for(var l in r)if(!(l in t))throw Error(k(108,lf(e)||"Unknown",l));return b({},n,r)}function gl(e){return e=(e=e.stateNode)&&e.__reactInternalMemoizedMergedChildContext||Nt,Bt=ce.current,F(ce,e),F(ye,ye.current),!0}function As(e,t,n){var r=e.stateNode;if(!r)throw Error(k(169));n?(e=tc(e,t,Bt),r.__reactInternalMemoizedMergedChildContext=e,B(ye),B(ce),F(ce,e)):B(ye),F(ye,n)}var qe=null,$l=!1,Eo=!1;function nc(e){qe===null?qe=[e]:qe.push(e)}function xp(e){$l=!0,nc(e)}function zt(){if(!Eo&&qe!==null){Eo=!0;var e=0,t=D;try{var n=qe;for(D=1;e<n.length;e++){var r=n[e];do r=r(!0);while(r!==null)}qe=null,$l=!1}catch(l){throw qe!==null&&(qe=qe.slice(e+1)),_u(Mi,zt),l}finally{D=t,Eo=!1}}return null}var ln=[],on=0,yl=null,vl=0,ze=[],Pe=0,Ut=null,et=1,tt="";function At(e,t){ln[on++]=vl,ln[on++]=yl,yl=e,vl=t}function rc(e,t,n){ze[Pe++]=et,ze[Pe++]=tt,ze[Pe++]=Ut,Ut=e;var r=et;e=tt;var l=32-je(r)-1;r&=~(1<<l),n+=1;var o=32-je(t)+l;if(30<o){var i=l-l%5;o=(r&(1<<i)-1).toString(32),r>>=i,l-=i,et=1<<32-je(t)+l|n<<l|r,tt=o+e}else et=1<<o|n<<l|r,tt=e}function Ui(e){e.return!==null&&(At(e,1),rc(e,1,0))}function Wi(e){for(;e===yl;)yl=ln[--on],ln[on]=null,vl=ln[--on],ln[on]=null;for(;e===Ut;)Ut=ze[--Pe],ze[Pe]=null,tt=ze[--Pe],ze[Pe]=null,et=ze[--Pe],ze[Pe]=null}var Se=null,Ce=null,U=!1,Fe=null;function lc(e,t){var n=Te(5,null,null,0);n.elementType="DELETED",n.stateNode=t,n.return=e,t=e.deletions,t===null?(e.deletions=[n],e.flags|=16):t.push(n)}function Ds(e,t){switch(e.tag){case 5:var n=e.type;return t=t.nodeType!==1||n.toLowerCase()!==t.nodeName.toLowerCase()?null:t,t!==null?(e.stateNode=t,Se=e,Ce=kt(t.firstChild),!0):!1;case 6:return t=e.pendingProps===""||t.nodeType!==3?null:t,t!==null?(e.stateNode=t,Se=e,Ce=null,!0):!1;case 13:return t=t.nodeType!==8?null:t,t!==null?(n=Ut!==null?{id:et,overflow:tt}:null,e.memoizedState={dehydrated:t,treeContext:n,retryLane:1073741824},n=Te(18,null,null,0),n.stateNode=t,n.return=e,e.child=n,Se=e,Ce=null,!0):!1;default:return!1}}function ii(e){return(e.mode&1)!==0&&(e.flags&128)===0}function ai(e){if(U){var t=Ce;if(t){var n=t;if(!Ds(e,t)){if(ii(e))throw Error(k(418));t=kt(n.nextSibling);var r=Se;t&&Ds(e,t)?lc(r,n):(e.flags=e.flags&-4097|2,U=!1,Se=e)}}else{if(ii(e))throw Error(k(418));e.flags=e.flags&-4097|2,U=!1,Se=e}}}function $s(e){for(e=e.return;e!==null&&e.tag!==5&&e.tag!==3&&e.tag!==13;)e=e.return;Se=e}function br(e){if(e!==Se)return!1;if(!U)return $s(e),U=!0,!1;var t;if((t=e.tag!==3)&&!(t=e.tag!==5)&&(t=e.type,t=t!=="head"&&t!=="body"&&!ni(e.type,e.memoizedProps)),t&&(t=Ce)){if(ii(e))throw oc(),Error(k(418));for(;t;)lc(e,t),t=kt(t.nextSibling)}if($s(e),e.tag===13){if(e=e.memoizedState,e=e!==null?e.dehydrated:null,!e)throw Error(k(317));e:{for(e=e.nextSibling,t=0;e;){if(e.nodeType===8){var n=e.data;if(n==="/$"){if(t===0){Ce=kt(e.nextSibling);break e}t--}else n!=="$"&&n!=="$!"&&n!=="$?"||t++}e=e.nextSibling}Ce=null}}else Ce=Se?kt(e.stateNode.nextSibling):null;return!0}function oc(){for(var e=Ce;e;)e=kt(e.nextSibling)}function vn(){Ce=Se=null,U=!1}function Hi(e){Fe===null?Fe=[e]:Fe.push(e)}var wp=at.ReactCurrentBatchConfig;function Fn(e,t,n){if(e=n.ref,e!==null&&typeof e!="function"&&typeof e!="object"){if(n._owner){if(n=n._owner,n){if(n.tag!==1)throw Error(k(309));var r=n.stateNode}if(!r)throw Error(k(147,e));var l=r,o=""+e;return t!==null&&t.ref!==null&&typeof t.ref=="function"&&t.ref._stringRef===o?t.ref:(t=function(i){var a=l.refs;i===null?delete a[o]:a[o]=i},t._stringRef=o,t)}if(typeof e!="string")throw Error(k(284));if(!n._owner)throw Error(k(290,e))}return e}function Qr(e,t){throw e=Object.prototype.toString.call(t),Error(k(31,e==="[object Object]"?"object with keys {"+Object.keys(t).join(", ")+"}":e))}function Os(e){var t=e._init;return t(e._payload)}function ic(e){function t(f,c){if(e){var p=f.deletions;p===null?(f.deletions=[c],f.flags|=16):p.push(c)}}function n(f,c){if(!e)return null;for(;c!==null;)t(f,c),c=c.sibling;return null}function r(f,c){for(f=new Map;c!==null;)c.key!==null?f.set(c.key,c):f.set(c.index,c),c=c.sibling;return f}function l(f,c){return f=St(f,c),f.index=0,f.sibling=null,f}function o(f,c,p){return f.index=p,e?(p=f.alternate,p!==null?(p=p.index,p<c?(f.flags|=2,c):p):(f.flags|=2,c)):(f.flags|=1048576,c)}function i(f){return e&&f.alternate===null&&(f.flags|=2),f}function a(f,c,p,x){return c===null||c.tag!==6?(c=Ro(p,f.mode,x),c.return=f,c):(c=l(c,p),c.return=f,c)}function s(f,c,p,x){var E=p.type;return E===Jt?g(f,c,p.props.children,x,p.key):c!==null&&(c.elementType===E||typeof E=="object"&&E!==null&&E.$$typeof===ct&&Os(E)===c.type)?(x=l(c,p.props),x.ref=Fn(f,c,p),x.return=f,x):(x=ol(p.type,p.key,p.props,null,f.mode,x),x.ref=Fn(f,c,p),x.return=f,x)}function d(f,c,p,x){return c===null||c.tag!==4||c.stateNode.containerInfo!==p.containerInfo||c.stateNode.implementation!==p.implementation?(c=Mo(p,f.mode,x),c.return=f,c):(c=l(c,p.children||[]),c.return=f,c)}function g(f,c,p,x,E){return c===null||c.tag!==7?(c=jt(p,f.mode,x,E),c.return=f,c):(c=l(c,p),c.return=f,c)}function v(f,c,p){if(typeof c=="string"&&c!==""||typeof c=="number")return c=Ro(""+c,f.mode,p),c.return=f,c;if(typeof c=="object"&&c!==null){switch(c.$$typeof){case Rr:return p=ol(c.type,c.key,c.props,null,f.mode,p),p.ref=Fn(f,null,c),p.return=f,p;case Xt:return c=Mo(c,f.mode,p),c.return=f,c;case ct:var x=c._init;return v(f,x(c._payload),p)}if(Hn(c)||Dn(c))return c=jt(c,f.mode,p,null),c.return=f,c;Qr(f,c)}return null}function y(f,c,p,x){var E=c!==null?c.key:null;if(typeof p=="string"&&p!==""||typeof p=="number")return E!==null?null:a(f,c,""+p,x);if(typeof p=="object"&&p!==null){switch(p.$$typeof){case Rr:return p.key===E?s(f,c,p,x):null;case Xt:return p.key===E?d(f,c,p,x):null;case ct:return E=p._init,y(f,c,E(p._payload),x)}if(Hn(p)||Dn(p))return E!==null?null:g(f,c,p,x,null);Qr(f,p)}return null}function w(f,c,p,x,E){if(typeof x=="string"&&x!==""||typeof x=="number")return f=f.get(p)||null,a(c,f,""+x,E);if(typeof x=="object"&&x!==null){switch(x.$$typeof){case Rr:return f=f.get(x.key===null?p:x.key)||null,s(c,f,x,E);case Xt:return f=f.get(x.key===null?p:x.key)||null,d(c,f,x,E);case ct:var P=x._init;return w(f,c,p,P(x._payload),E)}if(Hn(x)||Dn(x))return f=f.get(p)||null,g(c,f,x,E,null);Qr(c,x)}return null}function S(f,c,p,x){for(var E=null,P=null,_=c,T=c=0,$=null;_!==null&&T<p.length;T++){_.index>T?($=_,_=null):$=_.sibling;var L=y(f,_,p[T],x);if(L===null){_===null&&(_=$);break}e&&_&&L.alternate===null&&t(f,_),c=o(L,c,T),P===null?E=L:P.sibling=L,P=L,_=$}if(T===p.length)return n(f,_),U&&At(f,T),E;if(_===null){for(;T<p.length;T++)_=v(f,p[T],x),_!==null&&(c=o(_,c,T),P===null?E=_:P.sibling=_,P=_);return U&&At(f,T),E}for(_=r(f,_);T<p.length;T++)$=w(_,f,T,p[T],x),$!==null&&(e&&$.alternate!==null&&_.delete($.key===null?T:$.key),c=o($,c,T),P===null?E=$:P.sibling=$,P=$);return e&&_.forEach(function(Y){return t(f,Y)}),U&&At(f,T),E}function C(f,c,p,x){var E=Dn(p);if(typeof E!="function")throw Error(k(150));if(p=E.call(p),p==null)throw Error(k(151));for(var P=E=null,_=c,T=c=0,$=null,L=p.next();_!==null&&!L.done;T++,L=p.next()){_.index>T?($=_,_=null):$=_.sibling;var Y=y(f,_,L.value,x);if(Y===null){_===null&&(_=$);break}e&&_&&Y.alternate===null&&t(f,_),c=o(Y,c,T),P===null?E=Y:P.sibling=Y,P=Y,_=$}if(L.done)return n(f,_),U&&At(f,T),E;if(_===null){for(;!L.done;T++,L=p.next())L=v(f,L.value,x),L!==null&&(c=o(L,c,T),P===null?E=L:P.sibling=L,P=L);return U&&At(f,T),E}for(_=r(f,_);!L.done;T++,L=p.next())L=w(_,f,T,L.value,x),L!==null&&(e&&L.alternate!==null&&_.delete(L.key===null?T:L.key),c=o(L,c,T),P===null?E=L:P.sibling=L,P=L);return e&&_.forEach(function(Ke){return t(f,Ke)}),U&&At(f,T),E}function W(f,c,p,x){if(typeof p=="object"&&p!==null&&p.type===Jt&&p.key===null&&(p=p.props.children),typeof p=="object"&&p!==null){switch(p.$$typeof){case Rr:e:{for(var E=p.key,P=c;P!==null;){if(P.key===E){if(E=p.type,E===Jt){if(P.tag===7){n(f,P.sibling),c=l(P,p.props.children),c.return=f,f=c;break e}}else if(P.elementType===E||typeof E=="object"&&E!==null&&E.$$typeof===ct&&Os(E)===P.type){n(f,P.sibling),c=l(P,p.props),c.ref=Fn(f,P,p),c.return=f,f=c;break e}n(f,P);break}else t(f,P);P=P.sibling}p.type===Jt?(c=jt(p.props.children,f.mode,x,p.key),c.return=f,f=c):(x=ol(p.type,p.key,p.props,null,f.mode,x),x.ref=Fn(f,c,p),x.return=f,f=x)}return i(f);case Xt:e:{for(P=p.key;c!==null;){if(c.key===P)if(c.tag===4&&c.stateNode.containerInfo===p.containerInfo&&c.stateNode.implementation===p.implementation){n(f,c.sibling),c=l(c,p.children||[]),c.return=f,f=c;break e}else{n(f,c);break}else t(f,c);c=c.sibling}c=Mo(p,f.mode,x),c.return=f,f=c}return i(f);case ct:return P=p._init,W(f,c,P(p._payload),x)}if(Hn(p))return S(f,c,p,x);if(Dn(p))return C(f,c,p,x);Qr(f,p)}return typeof p=="string"&&p!==""||typeof p=="number"?(p=""+p,c!==null&&c.tag===6?(n(f,c.sibling),c=l(c,p),c.return=f,f=c):(n(f,c),c=Ro(p,f.mode,x),c.return=f,f=c),i(f)):n(f,c)}return W}var kn=ic(!0),ac=ic(!1),kl=_t(null),xl=null,an=null,Vi=null;function bi(){Vi=an=xl=null}function Qi(e){var t=kl.current;B(kl),e._currentValue=t}function si(e,t,n){for(;e!==null;){var r=e.alternate;if((e.childLanes&t)!==t?(e.childLanes|=t,r!==null&&(r.childLanes|=t)):r!==null&&(r.childLanes&t)!==t&&(r.childLanes|=t),e===n)break;e=e.return}}function mn(e,t){xl=e,Vi=an=null,e=e.dependencies,e!==null&&e.firstContext!==null&&(e.lanes&t&&(ge=!0),e.firstContext=null)}function Me(e){var t=e._currentValue;if(Vi!==e)if(e={context:e,memoizedValue:t,next:null},an===null){if(xl===null)throw Error(k(308));an=e,xl.dependencies={lanes:0,firstContext:e}}else an=an.next=e;return t}var Ot=null;function Gi(e){Ot===null?Ot=[e]:Ot.push(e)}function sc(e,t,n,r){var l=t.interleaved;return l===null?(n.next=n,Gi(t)):(n.next=l.next,l.next=n),t.interleaved=n,ot(e,r)}function ot(e,t){e.lanes|=t;var n=e.alternate;for(n!==null&&(n.lanes|=t),n=e,e=e.return;e!==null;)e.childLanes|=t,n=e.alternate,n!==null&&(n.childLanes|=t),n=e,e=e.return;return n.tag===3?n.stateNode:null}var dt=!1;function Ki(e){e.updateQueue={baseState:e.memoizedState,firstBaseUpdate:null,lastBaseUpdate:null,shared:{pending:null,interleaved:null,lanes:0},effects:null}}function uc(e,t){e=e.updateQueue,t.updateQueue===e&&(t.updateQueue={baseState:e.baseState,firstBaseUpdate:e.firstBaseUpdate,lastBaseUpdate:e.lastBaseUpdate,shared:e.shared,effects:e.effects})}function nt(e,t){return{eventTime:e,lane:t,tag:0,payload:null,callback:null,next:null}}function xt(e,t,n){var r=e.updateQueue;if(r===null)return null;if(r=r.shared,A&2){var l=r.pending;return l===null?t.next=t:(t.next=l.next,l.next=t),r.pending=t,ot(e,n)}return l=r.interleaved,l===null?(t.next=t,Gi(r)):(t.next=l.next,l.next=t),r.interleaved=t,ot(e,n)}function qr(e,t,n){if(t=t.updateQueue,t!==null&&(t=t.shared,(n&4194240)!==0)){var r=t.lanes;r&=e.pendingLanes,n|=r,t.lanes=n,Ai(e,n)}}function Is(e,t){var n=e.updateQueue,r=e.alternate;if(r!==null&&(r=r.updateQueue,n===r)){var l=null,o=null;if(n=n.firstBaseUpdate,n!==null){do{var i={eventTime:n.eventTime,lane:n.lane,tag:n.tag,payload:n.payload,callback:n.callback,next:null};o===null?l=o=i:o=o.next=i,n=n.next}while(n!==null);o===null?l=o=t:o=o.next=t}else l=o=t;n={baseState:r.baseState,firstBaseUpdate:l,lastBaseUpdate:o,shared:r.shared,effects:r.effects},e.updateQueue=n;return}e=n.lastBaseUpdate,e===null?n.firstBaseUpdate=t:e.next=t,n.lastBaseUpdate=t}function wl(e,t,n,r){var l=e.updateQueue;dt=!1;var o=l.firstBaseUpdate,i=l.lastBaseUpdate,a=l.shared.pending;if(a!==null){l.shared.pending=null;var s=a,d=s.next;s.next=null,i===null?o=d:i.next=d,i=s;var g=e.alternate;g!==null&&(g=g.updateQueue,a=g.lastBaseUpdate,a!==i&&(a===null?g.firstBaseUpdate=d:a.next=d,g.lastBaseUpdate=s))}if(o!==null){var v=l.baseState;i=0,g=d=s=null,a=o;do{var y=a.lane,w=a.eventTime;if((r&y)===y){g!==null&&(g=g.next={eventTime:w,lane:0,tag:a.tag,payload:a.payload,callback:a.callback,next:null});e:{var S=e,C=a;switch(y=t,w=n,C.tag){case 1:if(S=C.payload,typeof S=="function"){v=S.call(w,v,y);break e}v=S;break e;case 3:S.flags=S.flags&-65537|128;case 0:if(S=C.payload,y=typeof S=="function"?S.call(w,v,y):S,y==null)break e;v=b({},v,y);break e;case 2:dt=!0}}a.callback!==null&&a.lane!==0&&(e.flags|=64,y=l.effects,y===null?l.effects=[a]:y.push(a))}else w={eventTime:w,lane:y,tag:a.tag,payload:a.payload,callback:a.callback,next:null},g===null?(d=g=w,s=v):g=g.next=w,i|=y;if(a=a.next,a===null){if(a=l.shared.pending,a===null)break;y=a,a=y.next,y.next=null,l.lastBaseUpdate=y,l.shared.pending=null}}while(!0);if(g===null&&(s=v),l.baseState=s,l.firstBaseUpdate=d,l.lastBaseUpdate=g,t=l.shared.interleaved,t!==null){l=t;do i|=l.lane,l=l.next;while(l!==t)}else o===null&&(l.shared.lanes=0);Ht|=i,e.lanes=i,e.memoizedState=v}}function Fs(e,t,n){if(e=t.effects,t.effects=null,e!==null)for(t=0;t<e.length;t++){var r=e[t],l=r.callback;if(l!==null){if(r.callback=null,r=n,typeof l!="function")throw Error(k(191,l));l.call(r)}}}var wr={},Ge=_t(wr),fr=_t(wr),pr=_t(wr);function It(e){if(e===wr)throw Error(k(174));return e}function Yi(e,t){switch(F(pr,t),F(fr,e),F(Ge,wr),e=t.nodeType,e){case 9:case 11:t=(t=t.documentElement)?t.namespaceURI:Wo(null,"");break;default:e=e===8?t.parentNode:t,t=e.namespaceURI||null,e=e.tagName,t=Wo(t,e)}B(Ge),F(Ge,t)}function xn(){B(Ge),B(fr),B(pr)}function cc(e){It(pr.current);var t=It(Ge.current),n=Wo(t,e.type);t!==n&&(F(fr,e),F(Ge,n))}function Zi(e){fr.current===e&&(B(Ge),B(fr))}var H=_t(0);function Cl(e){for(var t=e;t!==null;){if(t.tag===13){var n=t.memoizedState;if(n!==null&&(n=n.dehydrated,n===null||n.data==="$?"||n.data==="$!"))return t}else if(t.tag===19&&t.memoizedProps.revealOrder!==void 0){if(t.flags&128)return t}else if(t.child!==null){t.child.return=t,t=t.child;continue}if(t===e)break;for(;t.sibling===null;){if(t.return===null||t.return===e)return null;t=t.return}t.sibling.return=t.return,t=t.sibling}return null}var No=[];function Xi(){for(var e=0;e<No.length;e++)No[e]._workInProgressVersionPrimary=null;No.length=0}var el=at.ReactCurrentDispatcher,Lo=at.ReactCurrentBatchConfig,Wt=0,V=null,J=null,ee=null,Sl=!1,Xn=!1,mr=0,Cp=0;function ae(){throw Error(k(321))}function Ji(e,t){if(t===null)return!1;for(var n=0;n<t.length&&n<e.length;n++)if(!Ue(e[n],t[n]))return!1;return!0}function qi(e,t,n,r,l,o){if(Wt=o,V=t,t.memoizedState=null,t.updateQueue=null,t.lanes=0,el.current=e===null||e.memoizedState===null?Lp:_p,e=n(r,l),Xn){o=0;do{if(Xn=!1,mr=0,25<=o)throw Error(k(301));o+=1,ee=J=null,t.updateQueue=null,el.current=zp,e=n(r,l)}while(Xn)}if(el.current=El,t=J!==null&&J.next!==null,Wt=0,ee=J=V=null,Sl=!1,t)throw Error(k(300));return e}function ea(){var e=mr!==0;return mr=0,e}function Ve(){var e={memoizedState:null,baseState:null,baseQueue:null,queue:null,next:null};return ee===null?V.memoizedState=ee=e:ee=ee.next=e,ee}function Ae(){if(J===null){var e=V.alternate;e=e!==null?e.memoizedState:null}else e=J.next;var t=ee===null?V.memoizedState:ee.next;if(t!==null)ee=t,J=e;else{if(e===null)throw Error(k(310));J=e,e={memoizedState:J.memoizedState,baseState:J.baseState,baseQueue:J.baseQueue,queue:J.queue,next:null},ee===null?V.memoizedState=ee=e:ee=ee.next=e}return ee}function hr(e,t){return typeof t=="function"?t(e):t}function _o(e){var t=Ae(),n=t.queue;if(n===null)throw Error(k(311));n.lastRenderedReducer=e;var r=J,l=r.baseQueue,o=n.pending;if(o!==null){if(l!==null){var i=l.next;l.next=o.next,o.next=i}r.baseQueue=l=o,n.pending=null}if(l!==null){o=l.next,r=r.baseState;var a=i=null,s=null,d=o;do{var g=d.lane;if((Wt&g)===g)s!==null&&(s=s.next={lane:0,action:d.action,hasEagerState:d.hasEagerState,eagerState:d.eagerState,next:null}),r=d.hasEagerState?d.eagerState:e(r,d.action);else{var v={lane:g,action:d.action,hasEagerState:d.hasEagerState,eagerState:d.eagerState,next:null};s===null?(a=s=v,i=r):s=s.next=v,V.lanes|=g,Ht|=g}d=d.next}while(d!==null&&d!==o);s===null?i=r:s.next=a,Ue(r,t.memoizedState)||(ge=!0),t.memoizedState=r,t.baseState=i,t.baseQueue=s,n.lastRenderedState=r}if(e=n.interleaved,e!==null){l=e;do o=l.lane,V.lanes|=o,Ht|=o,l=l.next;while(l!==e)}else l===null&&(n.lanes=0);return[t.memoizedState,n.dispatch]}function zo(e){var t=Ae(),n=t.queue;if(n===null)throw Error(k(311));n.lastRenderedReducer=e;var r=n.dispatch,l=n.pending,o=t.memoizedState;if(l!==null){n.pending=null;var i=l=l.next;do o=e(o,i.action),i=i.next;while(i!==l);Ue(o,t.memoizedState)||(ge=!0),t.memoizedState=o,t.baseQueue===null&&(t.baseState=o),n.lastRenderedState=o}return[o,r]}function dc(){}function fc(e,t){var n=V,r=Ae(),l=t(),o=!Ue(r.memoizedState,l);if(o&&(r.memoizedState=l,ge=!0),r=r.queue,ta(hc.bind(null,n,r,e),[e]),r.getSnapshot!==t||o||ee!==null&&ee.memoizedState.tag&1){if(n.flags|=2048,gr(9,mc.bind(null,n,r,l,t),void 0,null),te===null)throw Error(k(349));Wt&30||pc(n,t,l)}return l}function pc(e,t,n){e.flags|=16384,e={getSnapshot:t,value:n},t=V.updateQueue,t===null?(t={lastEffect:null,stores:null},V.updateQueue=t,t.stores=[e]):(n=t.stores,n===null?t.stores=[e]:n.push(e))}function mc(e,t,n,r){t.value=n,t.getSnapshot=r,gc(t)&&yc(e)}function hc(e,t,n){return n(function(){gc(t)&&yc(e)})}function gc(e){var t=e.getSnapshot;e=e.value;try{var n=t();return!Ue(e,n)}catch{return!0}}function yc(e){var t=ot(e,1);t!==null&&Be(t,e,1,-1)}function js(e){var t=Ve();return typeof e=="function"&&(e=e()),t.memoizedState=t.baseState=e,e={pending:null,interleaved:null,lanes:0,dispatch:null,lastRenderedReducer:hr,lastRenderedState:e},t.queue=e,e=e.dispatch=Np.bind(null,V,e),[t.memoizedState,e]}function gr(e,t,n,r){return e={tag:e,create:t,destroy:n,deps:r,next:null},t=V.updateQueue,t===null?(t={lastEffect:null,stores:null},V.updateQueue=t,t.lastEffect=e.next=e):(n=t.lastEffect,n===null?t.lastEffect=e.next=e:(r=n.next,n.next=e,e.next=r,t.lastEffect=e)),e}function vc(){return Ae().memoizedState}function tl(e,t,n,r){var l=Ve();V.flags|=e,l.memoizedState=gr(1|t,n,void 0,r===void 0?null:r)}function Ol(e,t,n,r){var l=Ae();r=r===void 0?null:r;var o=void 0;if(J!==null){var i=J.memoizedState;if(o=i.destroy,r!==null&&Ji(r,i.deps)){l.memoizedState=gr(t,n,o,r);return}}V.flags|=e,l.memoizedState=gr(1|t,n,o,r)}function Bs(e,t){return tl(8390656,8,e,t)}function ta(e,t){return Ol(2048,8,e,t)}function kc(e,t){return Ol(4,2,e,t)}function xc(e,t){return Ol(4,4,e,t)}function wc(e,t){if(typeof t=="function")return e=e(),t(e),function(){t(null)};if(t!=null)return e=e(),t.current=e,function(){t.current=null}}function Cc(e,t,n){return n=n!=null?n.concat([e]):null,Ol(4,4,wc.bind(null,t,e),n)}function na(){}function Sc(e,t){var n=Ae();t=t===void 0?null:t;var r=n.memoizedState;return r!==null&&t!==null&&Ji(t,r[1])?r[0]:(n.memoizedState=[e,t],e)}function Ec(e,t){var n=Ae();t=t===void 0?null:t;var r=n.memoizedState;return r!==null&&t!==null&&Ji(t,r[1])?r[0]:(e=e(),n.memoizedState=[e,t],e)}function Nc(e,t,n){return Wt&21?(Ue(n,t)||(n=Tu(),V.lanes|=n,Ht|=n,e.baseState=!0),t):(e.baseState&&(e.baseState=!1,ge=!0),e.memoizedState=n)}function Sp(e,t){var n=D;D=n!==0&&4>n?n:4,e(!0);var r=Lo.transition;Lo.transition={};try{e(!1),t()}finally{D=n,Lo.transition=r}}function Lc(){return Ae().memoizedState}function Ep(e,t,n){var r=Ct(e);if(n={lane:r,action:n,hasEagerState:!1,eagerState:null,next:null},_c(e))zc(t,n);else if(n=sc(e,t,n,r),n!==null){var l=pe();Be(n,e,r,l),Pc(n,t,r)}}function Np(e,t,n){var r=Ct(e),l={lane:r,action:n,hasEagerState:!1,eagerState:null,next:null};if(_c(e))zc(t,l);else{var o=e.alternate;if(e.lanes===0&&(o===null||o.lanes===0)&&(o=t.lastRenderedReducer,o!==null))try{var i=t.lastRenderedState,a=o(i,n);if(l.hasEagerState=!0,l.eagerState=a,Ue(a,i)){var s=t.interleaved;s===null?(l.next=l,Gi(t)):(l.next=s.next,s.next=l),t.interleaved=l;return}}catch{}finally{}n=sc(e,t,l,r),n!==null&&(l=pe(),Be(n,e,r,l),Pc(n,t,r))}}function _c(e){var t=e.alternate;return e===V||t!==null&&t===V}function zc(e,t){Xn=Sl=!0;var n=e.pending;n===null?t.next=t:(t.next=n.next,n.next=t),e.pending=t}function Pc(e,t,n){if(n&4194240){var r=t.lanes;r&=e.pendingLanes,n|=r,t.lanes=n,Ai(e,n)}}var El={readContext:Me,useCallback:ae,useContext:ae,useEffect:ae,useImperativeHandle:ae,useInsertionEffect:ae,useLayoutEffect:ae,useMemo:ae,useReducer:ae,useRef:ae,useState:ae,useDebugValue:ae,useDeferredValue:ae,useTransition:ae,useMutableSource:ae,useSyncExternalStore:ae,useId:ae,unstable_isNewReconciler:!1},Lp={readContext:Me,useCallback:function(e,t){return Ve().memoizedState=[e,t===void 0?null:t],e},useContext:Me,useEffect:Bs,useImperativeHandle:function(e,t,n){return n=n!=null?n.concat([e]):null,tl(4194308,4,wc.bind(null,t,e),n)},useLayoutEffect:function(e,t){return tl(4194308,4,e,t)},useInsertionEffect:function(e,t){return tl(4,2,e,t)},useMemo:function(e,t){var n=Ve();return t=t===void 0?null:t,e=e(),n.memoizedState=[e,t],e},useReducer:function(e,t,n){var r=Ve();return t=n!==void 0?n(t):t,r.memoizedState=r.baseState=t,e={pending:null,interleaved:null,lanes:0,dispatch:null,lastRenderedReducer:e,lastRenderedState:t},r.queue=e,e=e.dispatch=Ep.bind(null,V,e),[r.memoizedState,e]},useRef:function(e){var t=Ve();return e={current:e},t.memoizedState=e},useState:js,useDebugValue:na,useDeferredValue:function(e){return Ve().memoizedState=e},useTransition:function(){var e=js(!1),t=e[0];return e=Sp.bind(null,e[1]),Ve().memoizedState=e,[t,e]},useMutableSource:function(){},useSyncExternalStore:function(e,t,n){var r=V,l=Ve();if(U){if(n===void 0)throw Error(k(407));n=n()}else{if(n=t(),te===null)throw Error(k(349));Wt&30||pc(r,t,n)}l.memoizedState=n;var o={value:n,getSnapshot:t};return l.queue=o,Bs(hc.bind(null,r,o,e),[e]),r.flags|=2048,gr(9,mc.bind(null,r,o,n,t),void 0,null),n},useId:function(){var e=Ve(),t=te.identifierPrefix;if(U){var n=tt,r=et;n=(r&~(1<<32-je(r)-1)).toString(32)+n,t=":"+t+"R"+n,n=mr++,0<n&&(t+="H"+n.toString(32)),t+=":"}else n=Cp++,t=":"+t+"r"+n.toString(32)+":";return e.memoizedState=t},unstable_isNewReconciler:!1},_p={readContext:Me,useCallback:Sc,useContext:Me,useEffect:ta,useImperativeHandle:Cc,useInsertionEffect:kc,useLayoutEffect:xc,useMemo:Ec,useReducer:_o,useRef:vc,useState:function(){return _o(hr)},useDebugValue:na,useDeferredValue:function(e){var t=Ae();return Nc(t,J.memoizedState,e)},useTransition:function(){var e=_o(hr)[0],t=Ae().memoizedState;return[e,t]},useMutableSource:dc,useSyncExternalStore:fc,useId:Lc,unstable_isNewReconciler:!1},zp={readContext:Me,useCallback:Sc,useContext:Me,useEffect:ta,useImperativeHandle:Cc,useInsertionEffect:kc,useLayoutEffect:xc,useMemo:Ec,useReducer:zo,useRef:vc,useState:function(){return zo(hr)},useDebugValue:na,useDeferredValue:function(e){var t=Ae();return J===null?t.memoizedState=e:Nc(t,J.memoizedState,e)},useTransition:function(){var e=zo(hr)[0],t=Ae().memoizedState;return[e,t]},useMutableSource:dc,useSyncExternalStore:fc,useId:Lc,unstable_isNewReconciler:!1};function Oe(e,t){if(e&&e.defaultProps){t=b({},t),e=e.defaultProps;for(var n in e)t[n]===void 0&&(t[n]=e[n]);return t}return t}function ui(e,t,n,r){t=e.memoizedState,n=n(r,t),n=n==null?t:b({},t,n),e.memoizedState=n,e.lanes===0&&(e.updateQueue.baseState=n)}var Il={isMounted:function(e){return(e=e._reactInternals)?Qt(e)===e:!1},enqueueSetState:function(e,t,n){e=e._reactInternals;var r=pe(),l=Ct(e),o=nt(r,l);o.payload=t,n!=null&&(o.callback=n),t=xt(e,o,l),t!==null&&(Be(t,e,l,r),qr(t,e,l))},enqueueReplaceState:function(e,t,n){e=e._reactInternals;var r=pe(),l=Ct(e),o=nt(r,l);o.tag=1,o.payload=t,n!=null&&(o.callback=n),t=xt(e,o,l),t!==null&&(Be(t,e,l,r),qr(t,e,l))},enqueueForceUpdate:function(e,t){e=e._reactInternals;var n=pe(),r=Ct(e),l=nt(n,r);l.tag=2,t!=null&&(l.callback=t),t=xt(e,l,r),t!==null&&(Be(t,e,r,n),qr(t,e,r))}};function Us(e,t,n,r,l,o,i){return e=e.stateNode,typeof e.shouldComponentUpdate=="function"?e.shouldComponentUpdate(r,o,i):t.prototype&&t.prototype.isPureReactComponent?!sr(n,r)||!sr(l,o):!0}function Tc(e,t,n){var r=!1,l=Nt,o=t.contextType;return typeof o=="object"&&o!==null?o=Me(o):(l=ve(t)?Bt:ce.current,r=t.contextTypes,o=(r=r!=null)?yn(e,l):Nt),t=new t(n,o),e.memoizedState=t.state!==null&&t.state!==void 0?t.state:null,t.updater=Il,e.stateNode=t,t._reactInternals=e,r&&(e=e.stateNode,e.__reactInternalMemoizedUnmaskedChildContext=l,e.__reactInternalMemoizedMaskedChildContext=o),t}function Ws(e,t,n,r){e=t.state,typeof t.componentWillReceiveProps=="function"&&t.componentWillReceiveProps(n,r),typeof t.UNSAFE_componentWillReceiveProps=="function"&&t.UNSAFE_componentWillReceiveProps(n,r),t.state!==e&&Il.enqueueReplaceState(t,t.state,null)}function ci(e,t,n,r){var l=e.stateNode;l.props=n,l.state=e.memoizedState,l.refs={},Ki(e);var o=t.contextType;typeof o=="object"&&o!==null?l.context=Me(o):(o=ve(t)?Bt:ce.current,l.context=yn(e,o)),l.state=e.memoizedState,o=t.getDerivedStateFromProps,typeof o=="function"&&(ui(e,t,o,n),l.state=e.memoizedState),typeof t.getDerivedStateFromProps=="function"||typeof l.getSnapshotBeforeUpdate=="function"||typeof l.UNSAFE_componentWillMount!="function"&&typeof l.componentWillMount!="function"||(t=l.state,typeof l.componentWillMount=="function"&&l.componentWillMount(),typeof l.UNSAFE_componentWillMount=="function"&&l.UNSAFE_componentWillMount(),t!==l.state&&Il.enqueueReplaceState(l,l.state,null),wl(e,n,l,r),l.state=e.memoizedState),typeof l.componentDidMount=="function"&&(e.flags|=4194308)}function wn(e,t){try{var n="",r=t;do n+=rf(r),r=r.return;while(r);var l=n}catch(o){l=`
Error generating stack: `+o.message+`
`+o.stack}return{value:e,source:t,stack:l,digest:null}}function Po(e,t,n){return{value:e,source:null,stack:n??null,digest:t??null}}function di(e,t){try{console.error(t.value)}catch(n){setTimeout(function(){throw n})}}var Pp=typeof WeakMap=="function"?WeakMap:Map;function Rc(e,t,n){n=nt(-1,n),n.tag=3,n.payload={element:null};var r=t.value;return n.callback=function(){Ll||(Ll=!0,wi=r),di(e,t)},n}function Mc(e,t,n){n=nt(-1,n),n.tag=3;var r=e.type.getDerivedStateFromError;if(typeof r=="function"){var l=t.value;n.payload=function(){return r(l)},n.callback=function(){di(e,t)}}var o=e.stateNode;return o!==null&&typeof o.componentDidCatch=="function"&&(n.callback=function(){di(e,t),typeof r!="function"&&(wt===null?wt=new Set([this]):wt.add(this));var i=t.stack;this.componentDidCatch(t.value,{componentStack:i!==null?i:""})}),n}function Hs(e,t,n){var r=e.pingCache;if(r===null){r=e.pingCache=new Pp;var l=new Set;r.set(t,l)}else l=r.get(t),l===void 0&&(l=new Set,r.set(t,l));l.has(n)||(l.add(n),e=Hp.bind(null,e,t,n),t.then(e,e))}function Vs(e){do{var t;if((t=e.tag===13)&&(t=e.memoizedState,t=t!==null?t.dehydrated!==null:!0),t)return e;e=e.return}while(e!==null);return null}function bs(e,t,n,r,l){return e.mode&1?(e.flags|=65536,e.lanes=l,e):(e===t?e.flags|=65536:(e.flags|=128,n.flags|=131072,n.flags&=-52805,n.tag===1&&(n.alternate===null?n.tag=17:(t=nt(-1,1),t.tag=2,xt(n,t,1))),n.lanes|=1),e)}var Tp=at.ReactCurrentOwner,ge=!1;function fe(e,t,n,r){t.child=e===null?ac(t,null,n,r):kn(t,e.child,n,r)}function Qs(e,t,n,r,l){n=n.render;var o=t.ref;return mn(t,l),r=qi(e,t,n,r,o,l),n=ea(),e!==null&&!ge?(t.updateQueue=e.updateQueue,t.flags&=-2053,e.lanes&=~l,it(e,t,l)):(U&&n&&Ui(t),t.flags|=1,fe(e,t,r,l),t.child)}function Gs(e,t,n,r,l){if(e===null){var o=n.type;return typeof o=="function"&&!ca(o)&&o.defaultProps===void 0&&n.compare===null&&n.defaultProps===void 0?(t.tag=15,t.type=o,Ac(e,t,o,r,l)):(e=ol(n.type,null,r,t,t.mode,l),e.ref=t.ref,e.return=t,t.child=e)}if(o=e.child,!(e.lanes&l)){var i=o.memoizedProps;if(n=n.compare,n=n!==null?n:sr,n(i,r)&&e.ref===t.ref)return it(e,t,l)}return t.flags|=1,e=St(o,r),e.ref=t.ref,e.return=t,t.child=e}function Ac(e,t,n,r,l){if(e!==null){var o=e.memoizedProps;if(sr(o,r)&&e.ref===t.ref)if(ge=!1,t.pendingProps=r=o,(e.lanes&l)!==0)e.flags&131072&&(ge=!0);else return t.lanes=e.lanes,it(e,t,l)}return fi(e,t,n,r,l)}function Dc(e,t,n){var r=t.pendingProps,l=r.children,o=e!==null?e.memoizedState:null;if(r.mode==="hidden")if(!(t.mode&1))t.memoizedState={baseLanes:0,cachePool:null,transitions:null},F(un,we),we|=n;else{if(!(n&1073741824))return e=o!==null?o.baseLanes|n:n,t.lanes=t.childLanes=1073741824,t.memoizedState={baseLanes:e,cachePool:null,transitions:null},t.updateQueue=null,F(un,we),we|=e,null;t.memoizedState={baseLanes:0,cachePool:null,transitions:null},r=o!==null?o.baseLanes:n,F(un,we),we|=r}else o!==null?(r=o.baseLanes|n,t.memoizedState=null):r=n,F(un,we),we|=r;return fe(e,t,l,n),t.child}function $c(e,t){var n=t.ref;(e===null&&n!==null||e!==null&&e.ref!==n)&&(t.flags|=512,t.flags|=2097152)}function fi(e,t,n,r,l){var o=ve(n)?Bt:ce.current;return o=yn(t,o),mn(t,l),n=qi(e,t,n,r,o,l),r=ea(),e!==null&&!ge?(t.updateQueue=e.updateQueue,t.flags&=-2053,e.lanes&=~l,it(e,t,l)):(U&&r&&Ui(t),t.flags|=1,fe(e,t,n,l),t.child)}function Ks(e,t,n,r,l){if(ve(n)){var o=!0;gl(t)}else o=!1;if(mn(t,l),t.stateNode===null)nl(e,t),Tc(t,n,r),ci(t,n,r,l),r=!0;else if(e===null){var i=t.stateNode,a=t.memoizedProps;i.props=a;var s=i.context,d=n.contextType;typeof d=="object"&&d!==null?d=Me(d):(d=ve(n)?Bt:ce.current,d=yn(t,d));var g=n.getDerivedStateFromProps,v=typeof g=="function"||typeof i.getSnapshotBeforeUpdate=="function";v||typeof i.UNSAFE_componentWillReceiveProps!="function"&&typeof i.componentWillReceiveProps!="function"||(a!==r||s!==d)&&Ws(t,i,r,d),dt=!1;var y=t.memoizedState;i.state=y,wl(t,r,i,l),s=t.memoizedState,a!==r||y!==s||ye.current||dt?(typeof g=="function"&&(ui(t,n,g,r),s=t.memoizedState),(a=dt||Us(t,n,a,r,y,s,d))?(v||typeof i.UNSAFE_componentWillMount!="function"&&typeof i.componentWillMount!="function"||(typeof i.componentWillMount=="function"&&i.componentWillMount(),typeof i.UNSAFE_componentWillMount=="function"&&i.UNSAFE_componentWillMount()),typeof i.componentDidMount=="function"&&(t.flags|=4194308)):(typeof i.componentDidMount=="function"&&(t.flags|=4194308),t.memoizedProps=r,t.memoizedState=s),i.props=r,i.state=s,i.context=d,r=a):(typeof i.componentDidMount=="function"&&(t.flags|=4194308),r=!1)}else{i=t.stateNode,uc(e,t),a=t.memoizedProps,d=t.type===t.elementType?a:Oe(t.type,a),i.props=d,v=t.pendingProps,y=i.context,s=n.contextType,typeof s=="object"&&s!==null?s=Me(s):(s=ve(n)?Bt:ce.current,s=yn(t,s));var w=n.getDerivedStateFromProps;(g=typeof w=="function"||typeof i.getSnapshotBeforeUpdate=="function")||typeof i.UNSAFE_componentWillReceiveProps!="function"&&typeof i.componentWillReceiveProps!="function"||(a!==v||y!==s)&&Ws(t,i,r,s),dt=!1,y=t.memoizedState,i.state=y,wl(t,r,i,l);var S=t.memoizedState;a!==v||y!==S||ye.current||dt?(typeof w=="function"&&(ui(t,n,w,r),S=t.memoizedState),(d=dt||Us(t,n,d,r,y,S,s)||!1)?(g||typeof i.UNSAFE_componentWillUpdate!="function"&&typeof i.componentWillUpdate!="function"||(typeof i.componentWillUpdate=="function"&&i.componentWillUpdate(r,S,s),typeof i.UNSAFE_componentWillUpdate=="function"&&i.UNSAFE_componentWillUpdate(r,S,s)),typeof i.componentDidUpdate=="function"&&(t.flags|=4),typeof i.getSnapshotBeforeUpdate=="function"&&(t.flags|=1024)):(typeof i.componentDidUpdate!="function"||a===e.memoizedProps&&y===e.memoizedState||(t.flags|=4),typeof i.getSnapshotBeforeUpdate!="function"||a===e.memoizedProps&&y===e.memoizedState||(t.flags|=1024),t.memoizedProps=r,t.memoizedState=S),i.props=r,i.state=S,i.context=s,r=d):(typeof i.componentDidUpdate!="function"||a===e.memoizedProps&&y===e.memoizedState||(t.flags|=4),typeof i.getSnapshotBeforeUpdate!="function"||a===e.memoizedProps&&y===e.memoizedState||(t.flags|=1024),r=!1)}return pi(e,t,n,r,o,l)}function pi(e,t,n,r,l,o){$c(e,t);var i=(t.flags&128)!==0;if(!r&&!i)return l&&As(t,n,!1),it(e,t,o);r=t.stateNode,Tp.current=t;var a=i&&typeof n.getDerivedStateFromError!="function"?null:r.render();return t.flags|=1,e!==null&&i?(t.child=kn(t,e.child,null,o),t.child=kn(t,null,a,o)):fe(e,t,a,o),t.memoizedState=r.state,l&&As(t,n,!0),t.child}function Oc(e){var t=e.stateNode;t.pendingContext?Ms(e,t.pendingContext,t.pendingContext!==t.context):t.context&&Ms(e,t.context,!1),Yi(e,t.containerInfo)}function Ys(e,t,n,r,l){return vn(),Hi(l),t.flags|=256,fe(e,t,n,r),t.child}var mi={dehydrated:null,treeContext:null,retryLane:0};function hi(e){return{baseLanes:e,cachePool:null,transitions:null}}function Ic(e,t,n){var r=t.pendingProps,l=H.current,o=!1,i=(t.flags&128)!==0,a;if((a=i)||(a=e!==null&&e.memoizedState===null?!1:(l&2)!==0),a?(o=!0,t.flags&=-129):(e===null||e.memoizedState!==null)&&(l|=1),F(H,l&1),e===null)return ai(t),e=t.memoizedState,e!==null&&(e=e.dehydrated,e!==null)?(t.mode&1?e.data==="$!"?t.lanes=8:t.lanes=1073741824:t.lanes=1,null):(i=r.children,e=r.fallback,o?(r=t.mode,o=t.child,i={mode:"hidden",children:i},!(r&1)&&o!==null?(o.childLanes=0,o.pendingProps=i):o=Bl(i,r,0,null),e=jt(e,r,n,null),o.return=t,e.return=t,o.sibling=e,t.child=o,t.child.memoizedState=hi(n),t.memoizedState=mi,e):ra(t,i));if(l=e.memoizedState,l!==null&&(a=l.dehydrated,a!==null))return Rp(e,t,i,r,a,l,n);if(o){o=r.fallback,i=t.mode,l=e.child,a=l.sibling;var s={mode:"hidden",children:r.children};return!(i&1)&&t.child!==l?(r=t.child,r.childLanes=0,r.pendingProps=s,t.deletions=null):(r=St(l,s),r.subtreeFlags=l.subtreeFlags&14680064),a!==null?o=St(a,o):(o=jt(o,i,n,null),o.flags|=2),o.return=t,r.return=t,r.sibling=o,t.child=r,r=o,o=t.child,i=e.child.memoizedState,i=i===null?hi(n):{baseLanes:i.baseLanes|n,cachePool:null,transitions:i.transitions},o.memoizedState=i,o.childLanes=e.childLanes&~n,t.memoizedState=mi,r}return o=e.child,e=o.sibling,r=St(o,{mode:"visible",children:r.children}),!(t.mode&1)&&(r.lanes=n),r.return=t,r.sibling=null,e!==null&&(n=t.deletions,n===null?(t.deletions=[e],t.flags|=16):n.push(e)),t.child=r,t.memoizedState=null,r}function ra(e,t){return t=Bl({mode:"visible",children:t},e.mode,0,null),t.return=e,e.child=t}function Gr(e,t,n,r){return r!==null&&Hi(r),kn(t,e.child,null,n),e=ra(t,t.pendingProps.children),e.flags|=2,t.memoizedState=null,e}function Rp(e,t,n,r,l,o,i){if(n)return t.flags&256?(t.flags&=-257,r=Po(Error(k(422))),Gr(e,t,i,r)):t.memoizedState!==null?(t.child=e.child,t.flags|=128,null):(o=r.fallback,l=t.mode,r=Bl({mode:"visible",children:r.children},l,0,null),o=jt(o,l,i,null),o.flags|=2,r.return=t,o.return=t,r.sibling=o,t.child=r,t.mode&1&&kn(t,e.child,null,i),t.child.memoizedState=hi(i),t.memoizedState=mi,o);if(!(t.mode&1))return Gr(e,t,i,null);if(l.data==="$!"){if(r=l.nextSibling&&l.nextSibling.dataset,r)var a=r.dgst;return r=a,o=Error(k(419)),r=Po(o,r,void 0),Gr(e,t,i,r)}if(a=(i&e.childLanes)!==0,ge||a){if(r=te,r!==null){switch(i&-i){case 4:l=2;break;case 16:l=8;break;case 64:case 128:case 256:case 512:case 1024:case 2048:case 4096:case 8192:case 16384:case 32768:case 65536:case 131072:case 262144:case 524288:case 1048576:case 2097152:case 4194304:case 8388608:case 16777216:case 33554432:case 67108864:l=32;break;case 536870912:l=268435456;break;default:l=0}l=l&(r.suspendedLanes|i)?0:l,l!==0&&l!==o.retryLane&&(o.retryLane=l,ot(e,l),Be(r,e,l,-1))}return ua(),r=Po(Error(k(421))),Gr(e,t,i,r)}return l.data==="$?"?(t.flags|=128,t.child=e.child,t=Vp.bind(null,e),l._reactRetry=t,null):(e=o.treeContext,Ce=kt(l.nextSibling),Se=t,U=!0,Fe=null,e!==null&&(ze[Pe++]=et,ze[Pe++]=tt,ze[Pe++]=Ut,et=e.id,tt=e.overflow,Ut=t),t=ra(t,r.children),t.flags|=4096,t)}function Zs(e,t,n){e.lanes|=t;var r=e.alternate;r!==null&&(r.lanes|=t),si(e.return,t,n)}function To(e,t,n,r,l){var o=e.memoizedState;o===null?e.memoizedState={isBackwards:t,rendering:null,renderingStartTime:0,last:r,tail:n,tailMode:l}:(o.isBackwards=t,o.rendering=null,o.renderingStartTime=0,o.last=r,o.tail=n,o.tailMode=l)}function Fc(e,t,n){var r=t.pendingProps,l=r.revealOrder,o=r.tail;if(fe(e,t,r.children,n),r=H.current,r&2)r=r&1|2,t.flags|=128;else{if(e!==null&&e.flags&128)e:for(e=t.child;e!==null;){if(e.tag===13)e.memoizedState!==null&&Zs(e,n,t);else if(e.tag===19)Zs(e,n,t);else if(e.child!==null){e.child.return=e,e=e.child;continue}if(e===t)break e;for(;e.sibling===null;){if(e.return===null||e.return===t)break e;e=e.return}e.sibling.return=e.return,e=e.sibling}r&=1}if(F(H,r),!(t.mode&1))t.memoizedState=null;else switch(l){case"forwards":for(n=t.child,l=null;n!==null;)e=n.alternate,e!==null&&Cl(e)===null&&(l=n),n=n.sibling;n=l,n===null?(l=t.child,t.child=null):(l=n.sibling,n.sibling=null),To(t,!1,l,n,o);break;case"backwards":for(n=null,l=t.child,t.child=null;l!==null;){if(e=l.alternate,e!==null&&Cl(e)===null){t.child=l;break}e=l.sibling,l.sibling=n,n=l,l=e}To(t,!0,n,null,o);break;case"together":To(t,!1,null,null,void 0);break;default:t.memoizedState=null}return t.child}function nl(e,t){!(t.mode&1)&&e!==null&&(e.alternate=null,t.alternate=null,t.flags|=2)}function it(e,t,n){if(e!==null&&(t.dependencies=e.dependencies),Ht|=t.lanes,!(n&t.childLanes))return null;if(e!==null&&t.child!==e.child)throw Error(k(153));if(t.child!==null){for(e=t.child,n=St(e,e.pendingProps),t.child=n,n.return=t;e.sibling!==null;)e=e.sibling,n=n.sibling=St(e,e.pendingProps),n.return=t;n.sibling=null}return t.child}function Mp(e,t,n){switch(t.tag){case 3:Oc(t),vn();break;case 5:cc(t);break;case 1:ve(t.type)&&gl(t);break;case 4:Yi(t,t.stateNode.containerInfo);break;case 10:var r=t.type._context,l=t.memoizedProps.value;F(kl,r._currentValue),r._currentValue=l;break;case 13:if(r=t.memoizedState,r!==null)return r.dehydrated!==null?(F(H,H.current&1),t.flags|=128,null):n&t.child.childLanes?Ic(e,t,n):(F(H,H.current&1),e=it(e,t,n),e!==null?e.sibling:null);F(H,H.current&1);break;case 19:if(r=(n&t.childLanes)!==0,e.flags&128){if(r)return Fc(e,t,n);t.flags|=128}if(l=t.memoizedState,l!==null&&(l.rendering=null,l.tail=null,l.lastEffect=null),F(H,H.current),r)break;return null;case 22:case 23:return t.lanes=0,Dc(e,t,n)}return it(e,t,n)}var jc,gi,Bc,Uc;jc=function(e,t){for(var n=t.child;n!==null;){if(n.tag===5||n.tag===6)e.appendChild(n.stateNode);else if(n.tag!==4&&n.child!==null){n.child.return=n,n=n.child;continue}if(n===t)break;for(;n.sibling===null;){if(n.return===null||n.return===t)return;n=n.return}n.sibling.return=n.return,n=n.sibling}};gi=function(){};Bc=function(e,t,n,r){var l=e.memoizedProps;if(l!==r){e=t.stateNode,It(Ge.current);var o=null;switch(n){case"input":l=Fo(e,l),r=Fo(e,r),o=[];break;case"select":l=b({},l,{value:void 0}),r=b({},r,{value:void 0}),o=[];break;case"textarea":l=Uo(e,l),r=Uo(e,r),o=[];break;default:typeof l.onClick!="function"&&typeof r.onClick=="function"&&(e.onclick=ml)}Ho(n,r);var i;n=null;for(d in l)if(!r.hasOwnProperty(d)&&l.hasOwnProperty(d)&&l[d]!=null)if(d==="style"){var a=l[d];for(i in a)a.hasOwnProperty(i)&&(n||(n={}),n[i]="")}else d!=="dangerouslySetInnerHTML"&&d!=="children"&&d!=="suppressContentEditableWarning"&&d!=="suppressHydrationWarning"&&d!=="autoFocus"&&(tr.hasOwnProperty(d)?o||(o=[]):(o=o||[]).push(d,null));for(d in r){var s=r[d];if(a=l?.[d],r.hasOwnProperty(d)&&s!==a&&(s!=null||a!=null))if(d==="style")if(a){for(i in a)!a.hasOwnProperty(i)||s&&s.hasOwnProperty(i)||(n||(n={}),n[i]="");for(i in s)s.hasOwnProperty(i)&&a[i]!==s[i]&&(n||(n={}),n[i]=s[i])}else n||(o||(o=[]),o.push(d,n)),n=s;else d==="dangerouslySetInnerHTML"?(s=s?s.__html:void 0,a=a?a.__html:void 0,s!=null&&a!==s&&(o=o||[]).push(d,s)):d==="children"?typeof s!="string"&&typeof s!="number"||(o=o||[]).push(d,""+s):d!=="suppressContentEditableWarning"&&d!=="suppressHydrationWarning"&&(tr.hasOwnProperty(d)?(s!=null&&d==="onScroll"&&j("scroll",e),o||a===s||(o=[])):(o=o||[]).push(d,s))}n&&(o=o||[]).push("style",n);var d=o;(t.updateQueue=d)&&(t.flags|=4)}};Uc=function(e,t,n,r){n!==r&&(t.flags|=4)};function jn(e,t){if(!U)switch(e.tailMode){case"hidden":t=e.tail;for(var n=null;t!==null;)t.alternate!==null&&(n=t),t=t.sibling;n===null?e.tail=null:n.sibling=null;break;case"collapsed":n=e.tail;for(var r=null;n!==null;)n.alternate!==null&&(r=n),n=n.sibling;r===null?t||e.tail===null?e.tail=null:e.tail.sibling=null:r.sibling=null}}function se(e){var t=e.alternate!==null&&e.alternate.child===e.child,n=0,r=0;if(t)for(var l=e.child;l!==null;)n|=l.lanes|l.childLanes,r|=l.subtreeFlags&14680064,r|=l.flags&14680064,l.return=e,l=l.sibling;else for(l=e.child;l!==null;)n|=l.lanes|l.childLanes,r|=l.subtreeFlags,r|=l.flags,l.return=e,l=l.sibling;return e.subtreeFlags|=r,e.childLanes=n,t}function Ap(e,t,n){var r=t.pendingProps;switch(Wi(t),t.tag){case 2:case 16:case 15:case 0:case 11:case 7:case 8:case 12:case 9:case 14:return se(t),null;case 1:return ve(t.type)&&hl(),se(t),null;case 3:return r=t.stateNode,xn(),B(ye),B(ce),Xi(),r.pendingContext&&(r.context=r.pendingContext,r.pendingContext=null),(e===null||e.child===null)&&(br(t)?t.flags|=4:e===null||e.memoizedState.isDehydrated&&!(t.flags&256)||(t.flags|=1024,Fe!==null&&(Ei(Fe),Fe=null))),gi(e,t),se(t),null;case 5:Zi(t);var l=It(pr.current);if(n=t.type,e!==null&&t.stateNode!=null)Bc(e,t,n,r,l),e.ref!==t.ref&&(t.flags|=512,t.flags|=2097152);else{if(!r){if(t.stateNode===null)throw Error(k(166));return se(t),null}if(e=It(Ge.current),br(t)){r=t.stateNode,n=t.type;var o=t.memoizedProps;switch(r[be]=t,r[dr]=o,e=(t.mode&1)!==0,n){case"dialog":j("cancel",r),j("close",r);break;case"iframe":case"object":case"embed":j("load",r);break;case"video":case"audio":for(l=0;l<bn.length;l++)j(bn[l],r);break;case"source":j("error",r);break;case"img":case"image":case"link":j("error",r),j("load",r);break;case"details":j("toggle",r);break;case"input":ls(r,o),j("invalid",r);break;case"select":r._wrapperState={wasMultiple:!!o.multiple},j("invalid",r);break;case"textarea":is(r,o),j("invalid",r)}Ho(n,o),l=null;for(var i in o)if(o.hasOwnProperty(i)){var a=o[i];i==="children"?typeof a=="string"?r.textContent!==a&&(o.suppressHydrationWarning!==!0&&Vr(r.textContent,a,e),l=["children",a]):typeof a=="number"&&r.textContent!==""+a&&(o.suppressHydrationWarning!==!0&&Vr(r.textContent,a,e),l=["children",""+a]):tr.hasOwnProperty(i)&&a!=null&&i==="onScroll"&&j("scroll",r)}switch(n){case"input":Mr(r),os(r,o,!0);break;case"textarea":Mr(r),as(r);break;case"select":case"option":break;default:typeof o.onClick=="function"&&(r.onclick=ml)}r=l,t.updateQueue=r,r!==null&&(t.flags|=4)}else{i=l.nodeType===9?l:l.ownerDocument,e==="http://www.w3.org/1999/xhtml"&&(e=hu(n)),e==="http://www.w3.org/1999/xhtml"?n==="script"?(e=i.createElement("div"),e.innerHTML="<script><\/script>",e=e.removeChild(e.firstChild)):typeof r.is=="string"?e=i.createElement(n,{is:r.is}):(e=i.createElement(n),n==="select"&&(i=e,r.multiple?i.multiple=!0:r.size&&(i.size=r.size))):e=i.createElementNS(e,n),e[be]=t,e[dr]=r,jc(e,t,!1,!1),t.stateNode=e;e:{switch(i=Vo(n,r),n){case"dialog":j("cancel",e),j("close",e),l=r;break;case"iframe":case"object":case"embed":j("load",e),l=r;break;case"video":case"audio":for(l=0;l<bn.length;l++)j(bn[l],e);l=r;break;case"source":j("error",e),l=r;break;case"img":case"image":case"link":j("error",e),j("load",e),l=r;break;case"details":j("toggle",e),l=r;break;case"input":ls(e,r),l=Fo(e,r),j("invalid",e);break;case"option":l=r;break;case"select":e._wrapperState={wasMultiple:!!r.multiple},l=b({},r,{value:void 0}),j("invalid",e);break;case"textarea":is(e,r),l=Uo(e,r),j("invalid",e);break;default:l=r}Ho(n,l),a=l;for(o in a)if(a.hasOwnProperty(o)){var s=a[o];o==="style"?vu(e,s):o==="dangerouslySetInnerHTML"?(s=s?s.__html:void 0,s!=null&&gu(e,s)):o==="children"?typeof s=="string"?(n!=="textarea"||s!=="")&&nr(e,s):typeof s=="number"&&nr(e,""+s):o!=="suppressContentEditableWarning"&&o!=="suppressHydrationWarning"&&o!=="autoFocus"&&(tr.hasOwnProperty(o)?s!=null&&o==="onScroll"&&j("scroll",e):s!=null&&_i(e,o,s,i))}switch(n){case"input":Mr(e),os(e,r,!1);break;case"textarea":Mr(e),as(e);break;case"option":r.value!=null&&e.setAttribute("value",""+Et(r.value));break;case"select":e.multiple=!!r.multiple,o=r.value,o!=null?cn(e,!!r.multiple,o,!1):r.defaultValue!=null&&cn(e,!!r.multiple,r.defaultValue,!0);break;default:typeof l.onClick=="function"&&(e.onclick=ml)}switch(n){case"button":case"input":case"select":case"textarea":r=!!r.autoFocus;break e;case"img":r=!0;break e;default:r=!1}}r&&(t.flags|=4)}t.ref!==null&&(t.flags|=512,t.flags|=2097152)}return se(t),null;case 6:if(e&&t.stateNode!=null)Uc(e,t,e.memoizedProps,r);else{if(typeof r!="string"&&t.stateNode===null)throw Error(k(166));if(n=It(pr.current),It(Ge.current),br(t)){if(r=t.stateNode,n=t.memoizedProps,r[be]=t,(o=r.nodeValue!==n)&&(e=Se,e!==null))switch(e.tag){case 3:Vr(r.nodeValue,n,(e.mode&1)!==0);break;case 5:e.memoizedProps.suppressHydrationWarning!==!0&&Vr(r.nodeValue,n,(e.mode&1)!==0)}o&&(t.flags|=4)}else r=(n.nodeType===9?n:n.ownerDocument).createTextNode(r),r[be]=t,t.stateNode=r}return se(t),null;case 13:if(B(H),r=t.memoizedState,e===null||e.memoizedState!==null&&e.memoizedState.dehydrated!==null){if(U&&Ce!==null&&t.mode&1&&!(t.flags&128))oc(),vn(),t.flags|=98560,o=!1;else if(o=br(t),r!==null&&r.dehydrated!==null){if(e===null){if(!o)throw Error(k(318));if(o=t.memoizedState,o=o!==null?o.dehydrated:null,!o)throw Error(k(317));o[be]=t}else vn(),!(t.flags&128)&&(t.memoizedState=null),t.flags|=4;se(t),o=!1}else Fe!==null&&(Ei(Fe),Fe=null),o=!0;if(!o)return t.flags&65536?t:null}return t.flags&128?(t.lanes=n,t):(r=r!==null,r!==(e!==null&&e.memoizedState!==null)&&r&&(t.child.flags|=8192,t.mode&1&&(e===null||H.current&1?q===0&&(q=3):ua())),t.updateQueue!==null&&(t.flags|=4),se(t),null);case 4:return xn(),gi(e,t),e===null&&ur(t.stateNode.containerInfo),se(t),null;case 10:return Qi(t.type._context),se(t),null;case 17:return ve(t.type)&&hl(),se(t),null;case 19:if(B(H),o=t.memoizedState,o===null)return se(t),null;if(r=(t.flags&128)!==0,i=o.rendering,i===null)if(r)jn(o,!1);else{if(q!==0||e!==null&&e.flags&128)for(e=t.child;e!==null;){if(i=Cl(e),i!==null){for(t.flags|=128,jn(o,!1),r=i.updateQueue,r!==null&&(t.updateQueue=r,t.flags|=4),t.subtreeFlags=0,r=n,n=t.child;n!==null;)o=n,e=r,o.flags&=14680066,i=o.alternate,i===null?(o.childLanes=0,o.lanes=e,o.child=null,o.subtreeFlags=0,o.memoizedProps=null,o.memoizedState=null,o.updateQueue=null,o.dependencies=null,o.stateNode=null):(o.childLanes=i.childLanes,o.lanes=i.lanes,o.child=i.child,o.subtreeFlags=0,o.deletions=null,o.memoizedProps=i.memoizedProps,o.memoizedState=i.memoizedState,o.updateQueue=i.updateQueue,o.type=i.type,e=i.dependencies,o.dependencies=e===null?null:{lanes:e.lanes,firstContext:e.firstContext}),n=n.sibling;return F(H,H.current&1|2),t.child}e=e.sibling}o.tail!==null&&K()>Cn&&(t.flags|=128,r=!0,jn(o,!1),t.lanes=4194304)}else{if(!r)if(e=Cl(i),e!==null){if(t.flags|=128,r=!0,n=e.updateQueue,n!==null&&(t.updateQueue=n,t.flags|=4),jn(o,!0),o.tail===null&&o.tailMode==="hidden"&&!i.alternate&&!U)return se(t),null}else 2*K()-o.renderingStartTime>Cn&&n!==1073741824&&(t.flags|=128,r=!0,jn(o,!1),t.lanes=4194304);o.isBackwards?(i.sibling=t.child,t.child=i):(n=o.last,n!==null?n.sibling=i:t.child=i,o.last=i)}return o.tail!==null?(t=o.tail,o.rendering=t,o.tail=t.sibling,o.renderingStartTime=K(),t.sibling=null,n=H.current,F(H,r?n&1|2:n&1),t):(se(t),null);case 22:case 23:return sa(),r=t.memoizedState!==null,e!==null&&e.memoizedState!==null!==r&&(t.flags|=8192),r&&t.mode&1?we&1073741824&&(se(t),t.subtreeFlags&6&&(t.flags|=8192)):se(t),null;case 24:return null;case 25:return null}throw Error(k(156,t.tag))}function Dp(e,t){switch(Wi(t),t.tag){case 1:return ve(t.type)&&hl(),e=t.flags,e&65536?(t.flags=e&-65537|128,t):null;case 3:return xn(),B(ye),B(ce),Xi(),e=t.flags,e&65536&&!(e&128)?(t.flags=e&-65537|128,t):null;case 5:return Zi(t),null;case 13:if(B(H),e=t.memoizedState,e!==null&&e.dehydrated!==null){if(t.alternate===null)throw Error(k(340));vn()}return e=t.flags,e&65536?(t.flags=e&-65537|128,t):null;case 19:return B(H),null;case 4:return xn(),null;case 10:return Qi(t.type._context),null;case 22:case 23:return sa(),null;case 24:return null;default:return null}}var Kr=!1,ue=!1,$p=typeof WeakSet=="function"?WeakSet:Set,N=null;function sn(e,t){var n=e.ref;if(n!==null)if(typeof n=="function")try{n(null)}catch(r){Q(e,t,r)}else n.current=null}function yi(e,t,n){try{n()}catch(r){Q(e,t,r)}}var Xs=!1;function Op(e,t){if(ei=dl,e=Qu(),Bi(e)){if("selectionStart"in e)var n={start:e.selectionStart,end:e.selectionEnd};else e:{n=(n=e.ownerDocument)&&n.defaultView||window;var r=n.getSelection&&n.getSelection();if(r&&r.rangeCount!==0){n=r.anchorNode;var l=r.anchorOffset,o=r.focusNode;r=r.focusOffset;try{n.nodeType,o.nodeType}catch{n=null;break e}var i=0,a=-1,s=-1,d=0,g=0,v=e,y=null;t:for(;;){for(var w;v!==n||l!==0&&v.nodeType!==3||(a=i+l),v!==o||r!==0&&v.nodeType!==3||(s=i+r),v.nodeType===3&&(i+=v.nodeValue.length),(w=v.firstChild)!==null;)y=v,v=w;for(;;){if(v===e)break t;if(y===n&&++d===l&&(a=i),y===o&&++g===r&&(s=i),(w=v.nextSibling)!==null)break;v=y,y=v.parentNode}v=w}n=a===-1||s===-1?null:{start:a,end:s}}else n=null}n=n||{start:0,end:0}}else n=null;for(ti={focusedElem:e,selectionRange:n},dl=!1,N=t;N!==null;)if(t=N,e=t.child,(t.subtreeFlags&1028)!==0&&e!==null)e.return=t,N=e;else for(;N!==null;){t=N;try{var S=t.alternate;if(t.flags&1024)switch(t.tag){case 0:case 11:case 15:break;case 1:if(S!==null){var C=S.memoizedProps,W=S.memoizedState,f=t.stateNode,c=f.getSnapshotBeforeUpdate(t.elementType===t.type?C:Oe(t.type,C),W);f.__reactInternalSnapshotBeforeUpdate=c}break;case 3:var p=t.stateNode.containerInfo;p.nodeType===1?p.textContent="":p.nodeType===9&&p.documentElement&&p.removeChild(p.documentElement);break;case 5:case 6:case 4:case 17:break;default:throw Error(k(163))}}catch(x){Q(t,t.return,x)}if(e=t.sibling,e!==null){e.return=t.return,N=e;break}N=t.return}return S=Xs,Xs=!1,S}function Jn(e,t,n){var r=t.updateQueue;if(r=r!==null?r.lastEffect:null,r!==null){var l=r=r.next;do{if((l.tag&e)===e){var o=l.destroy;l.destroy=void 0,o!==void 0&&yi(t,n,o)}l=l.next}while(l!==r)}}function Fl(e,t){if(t=t.updateQueue,t=t!==null?t.lastEffect:null,t!==null){var n=t=t.next;do{if((n.tag&e)===e){var r=n.create;n.destroy=r()}n=n.next}while(n!==t)}}function vi(e){var t=e.ref;if(t!==null){var n=e.stateNode;switch(e.tag){case 5:e=n;break;default:e=n}typeof t=="function"?t(e):t.current=e}}function Wc(e){var t=e.alternate;t!==null&&(e.alternate=null,Wc(t)),e.child=null,e.deletions=null,e.sibling=null,e.tag===5&&(t=e.stateNode,t!==null&&(delete t[be],delete t[dr],delete t[li],delete t[vp],delete t[kp])),e.stateNode=null,e.return=null,e.dependencies=null,e.memoizedProps=null,e.memoizedState=null,e.pendingProps=null,e.stateNode=null,e.updateQueue=null}function Hc(e){return e.tag===5||e.tag===3||e.tag===4}function Js(e){e:for(;;){for(;e.sibling===null;){if(e.return===null||Hc(e.return))return null;e=e.return}for(e.sibling.return=e.return,e=e.sibling;e.tag!==5&&e.tag!==6&&e.tag!==18;){if(e.flags&2||e.child===null||e.tag===4)continue e;e.child.return=e,e=e.child}if(!(e.flags&2))return e.stateNode}}function ki(e,t,n){var r=e.tag;if(r===5||r===6)e=e.stateNode,t?n.nodeType===8?n.parentNode.insertBefore(e,t):n.insertBefore(e,t):(n.nodeType===8?(t=n.parentNode,t.insertBefore(e,n)):(t=n,t.appendChild(e)),n=n._reactRootContainer,n!=null||t.onclick!==null||(t.onclick=ml));else if(r!==4&&(e=e.child,e!==null))for(ki(e,t,n),e=e.sibling;e!==null;)ki(e,t,n),e=e.sibling}function xi(e,t,n){var r=e.tag;if(r===5||r===6)e=e.stateNode,t?n.insertBefore(e,t):n.appendChild(e);else if(r!==4&&(e=e.child,e!==null))for(xi(e,t,n),e=e.sibling;e!==null;)xi(e,t,n),e=e.sibling}var re=null,Ie=!1;function ut(e,t,n){for(n=n.child;n!==null;)Vc(e,t,n),n=n.sibling}function Vc(e,t,n){if(Qe&&typeof Qe.onCommitFiberUnmount=="function")try{Qe.onCommitFiberUnmount(Tl,n)}catch{}switch(n.tag){case 5:ue||sn(n,t);case 6:var r=re,l=Ie;re=null,ut(e,t,n),re=r,Ie=l,re!==null&&(Ie?(e=re,n=n.stateNode,e.nodeType===8?e.parentNode.removeChild(n):e.removeChild(n)):re.removeChild(n.stateNode));break;case 18:re!==null&&(Ie?(e=re,n=n.stateNode,e.nodeType===8?So(e.parentNode,n):e.nodeType===1&&So(e,n),ir(e)):So(re,n.stateNode));break;case 4:r=re,l=Ie,re=n.stateNode.containerInfo,Ie=!0,ut(e,t,n),re=r,Ie=l;break;case 0:case 11:case 14:case 15:if(!ue&&(r=n.updateQueue,r!==null&&(r=r.lastEffect,r!==null))){l=r=r.next;do{var o=l,i=o.destroy;o=o.tag,i!==void 0&&(o&2||o&4)&&yi(n,t,i),l=l.next}while(l!==r)}ut(e,t,n);break;case 1:if(!ue&&(sn(n,t),r=n.stateNode,typeof r.componentWillUnmount=="function"))try{r.props=n.memoizedProps,r.state=n.memoizedState,r.componentWillUnmount()}catch(a){Q(n,t,a)}ut(e,t,n);break;case 21:ut(e,t,n);break;case 22:n.mode&1?(ue=(r=ue)||n.memoizedState!==null,ut(e,t,n),ue=r):ut(e,t,n);break;default:ut(e,t,n)}}function qs(e){var t=e.updateQueue;if(t!==null){e.updateQueue=null;var n=e.stateNode;n===null&&(n=e.stateNode=new $p),t.forEach(function(r){var l=bp.bind(null,e,r);n.has(r)||(n.add(r),r.then(l,l))})}}function $e(e,t){var n=t.deletions;if(n!==null)for(var r=0;r<n.length;r++){var l=n[r];try{var o=e,i=t,a=i;e:for(;a!==null;){switch(a.tag){case 5:re=a.stateNode,Ie=!1;break e;case 3:re=a.stateNode.containerInfo,Ie=!0;break e;case 4:re=a.stateNode.containerInfo,Ie=!0;break e}a=a.return}if(re===null)throw Error(k(160));Vc(o,i,l),re=null,Ie=!1;var s=l.alternate;s!==null&&(s.return=null),l.return=null}catch(d){Q(l,t,d)}}if(t.subtreeFlags&12854)for(t=t.child;t!==null;)bc(t,e),t=t.sibling}function bc(e,t){var n=e.alternate,r=e.flags;switch(e.tag){case 0:case 11:case 14:case 15:if($e(t,e),He(e),r&4){try{Jn(3,e,e.return),Fl(3,e)}catch(C){Q(e,e.return,C)}try{Jn(5,e,e.return)}catch(C){Q(e,e.return,C)}}break;case 1:$e(t,e),He(e),r&512&&n!==null&&sn(n,n.return);break;case 5:if($e(t,e),He(e),r&512&&n!==null&&sn(n,n.return),e.flags&32){var l=e.stateNode;try{nr(l,"")}catch(C){Q(e,e.return,C)}}if(r&4&&(l=e.stateNode,l!=null)){var o=e.memoizedProps,i=n!==null?n.memoizedProps:o,a=e.type,s=e.updateQueue;if(e.updateQueue=null,s!==null)try{a==="input"&&o.type==="radio"&&o.name!=null&&pu(l,o),Vo(a,i);var d=Vo(a,o);for(i=0;i<s.length;i+=2){var g=s[i],v=s[i+1];g==="style"?vu(l,v):g==="dangerouslySetInnerHTML"?gu(l,v):g==="children"?nr(l,v):_i(l,g,v,d)}switch(a){case"input":jo(l,o);break;case"textarea":mu(l,o);break;case"select":var y=l._wrapperState.wasMultiple;l._wrapperState.wasMultiple=!!o.multiple;var w=o.value;w!=null?cn(l,!!o.multiple,w,!1):y!==!!o.multiple&&(o.defaultValue!=null?cn(l,!!o.multiple,o.defaultValue,!0):cn(l,!!o.multiple,o.multiple?[]:"",!1))}l[dr]=o}catch(C){Q(e,e.return,C)}}break;case 6:if($e(t,e),He(e),r&4){if(e.stateNode===null)throw Error(k(162));l=e.stateNode,o=e.memoizedProps;try{l.nodeValue=o}catch(C){Q(e,e.return,C)}}break;case 3:if($e(t,e),He(e),r&4&&n!==null&&n.memoizedState.isDehydrated)try{ir(t.containerInfo)}catch(C){Q(e,e.return,C)}break;case 4:$e(t,e),He(e);break;case 13:$e(t,e),He(e),l=e.child,l.flags&8192&&(o=l.memoizedState!==null,l.stateNode.isHidden=o,!o||l.alternate!==null&&l.alternate.memoizedState!==null||(ia=K())),r&4&&qs(e);break;case 22:if(g=n!==null&&n.memoizedState!==null,e.mode&1?(ue=(d=ue)||g,$e(t,e),ue=d):$e(t,e),He(e),r&8192){if(d=e.memoizedState!==null,(e.stateNode.isHidden=d)&&!g&&e.mode&1)for(N=e,g=e.child;g!==null;){for(v=N=g;N!==null;){switch(y=N,w=y.child,y.tag){case 0:case 11:case 14:case 15:Jn(4,y,y.return);break;case 1:sn(y,y.return);var S=y.stateNode;if(typeof S.componentWillUnmount=="function"){r=y,n=y.return;try{t=r,S.props=t.memoizedProps,S.state=t.memoizedState,S.componentWillUnmount()}catch(C){Q(r,n,C)}}break;case 5:sn(y,y.return);break;case 22:if(y.memoizedState!==null){tu(v);continue}}w!==null?(w.return=y,N=w):tu(v)}g=g.sibling}e:for(g=null,v=e;;){if(v.tag===5){if(g===null){g=v;try{l=v.stateNode,d?(o=l.style,typeof o.setProperty=="function"?o.setProperty("display","none","important"):o.display="none"):(a=v.stateNode,s=v.memoizedProps.style,i=s!=null&&s.hasOwnProperty("display")?s.display:null,a.style.display=yu("display",i))}catch(C){Q(e,e.return,C)}}}else if(v.tag===6){if(g===null)try{v.stateNode.nodeValue=d?"":v.memoizedProps}catch(C){Q(e,e.return,C)}}else if((v.tag!==22&&v.tag!==23||v.memoizedState===null||v===e)&&v.child!==null){v.child.return=v,v=v.child;continue}if(v===e)break e;for(;v.sibling===null;){if(v.return===null||v.return===e)break e;g===v&&(g=null),v=v.return}g===v&&(g=null),v.sibling.return=v.return,v=v.sibling}}break;case 19:$e(t,e),He(e),r&4&&qs(e);break;case 21:break;default:$e(t,e),He(e)}}function He(e){var t=e.flags;if(t&2){try{e:{for(var n=e.return;n!==null;){if(Hc(n)){var r=n;break e}n=n.return}throw Error(k(160))}switch(r.tag){case 5:var l=r.stateNode;r.flags&32&&(nr(l,""),r.flags&=-33);var o=Js(e);xi(e,o,l);break;case 3:case 4:var i=r.stateNode.containerInfo,a=Js(e);ki(e,a,i);break;default:throw Error(k(161))}}catch(s){Q(e,e.return,s)}e.flags&=-3}t&4096&&(e.flags&=-4097)}function Ip(e,t,n){N=e,Qc(e,t,n)}function Qc(e,t,n){for(var r=(e.mode&1)!==0;N!==null;){var l=N,o=l.child;if(l.tag===22&&r){var i=l.memoizedState!==null||Kr;if(!i){var a=l.alternate,s=a!==null&&a.memoizedState!==null||ue;a=Kr;var d=ue;if(Kr=i,(ue=s)&&!d)for(N=l;N!==null;)i=N,s=i.child,i.tag===22&&i.memoizedState!==null?nu(l):s!==null?(s.return=i,N=s):nu(l);for(;o!==null;)N=o,Qc(o,t,n),o=o.sibling;N=l,Kr=a,ue=d}eu(e,t,n)}else l.subtreeFlags&8772&&o!==null?(o.return=l,N=o):eu(e,t,n)}}function eu(e){for(;N!==null;){var t=N;if(t.flags&8772){var n=t.alternate;try{if(t.flags&8772)switch(t.tag){case 0:case 11:case 15:ue||Fl(5,t);break;case 1:var r=t.stateNode;if(t.flags&4&&!ue)if(n===null)r.componentDidMount();else{var l=t.elementType===t.type?n.memoizedProps:Oe(t.type,n.memoizedProps);r.componentDidUpdate(l,n.memoizedState,r.__reactInternalSnapshotBeforeUpdate)}var o=t.updateQueue;o!==null&&Fs(t,o,r);break;case 3:var i=t.updateQueue;if(i!==null){if(n=null,t.child!==null)switch(t.child.tag){case 5:n=t.child.stateNode;break;case 1:n=t.child.stateNode}Fs(t,i,n)}break;case 5:var a=t.stateNode;if(n===null&&t.flags&4){n=a;var s=t.memoizedProps;switch(t.type){case"button":case"input":case"select":case"textarea":s.autoFocus&&n.focus();break;case"img":s.src&&(n.src=s.src)}}break;case 6:break;case 4:break;case 12:break;case 13:if(t.memoizedState===null){var d=t.alternate;if(d!==null){var g=d.memoizedState;if(g!==null){var v=g.dehydrated;v!==null&&ir(v)}}}break;case 19:case 17:case 21:case 22:case 23:case 25:break;default:throw Error(k(163))}ue||t.flags&512&&vi(t)}catch(y){Q(t,t.return,y)}}if(t===e){N=null;break}if(n=t.sibling,n!==null){n.return=t.return,N=n;break}N=t.return}}function tu(e){for(;N!==null;){var t=N;if(t===e){N=null;break}var n=t.sibling;if(n!==null){n.return=t.return,N=n;break}N=t.return}}function nu(e){for(;N!==null;){var t=N;try{switch(t.tag){case 0:case 11:case 15:var n=t.return;try{Fl(4,t)}catch(s){Q(t,n,s)}break;case 1:var r=t.stateNode;if(typeof r.componentDidMount=="function"){var l=t.return;try{r.componentDidMount()}catch(s){Q(t,l,s)}}var o=t.return;try{vi(t)}catch(s){Q(t,o,s)}break;case 5:var i=t.return;try{vi(t)}catch(s){Q(t,i,s)}}}catch(s){Q(t,t.return,s)}if(t===e){N=null;break}var a=t.sibling;if(a!==null){a.return=t.return,N=a;break}N=t.return}}var Fp=Math.ceil,Nl=at.ReactCurrentDispatcher,la=at.ReactCurrentOwner,Re=at.ReactCurrentBatchConfig,A=0,te=null,X=null,le=0,we=0,un=_t(0),q=0,yr=null,Ht=0,jl=0,oa=0,qn=null,he=null,ia=0,Cn=1/0,Je=null,Ll=!1,wi=null,wt=null,Yr=!1,ht=null,_l=0,er=0,Ci=null,rl=-1,ll=0;function pe(){return A&6?K():rl!==-1?rl:rl=K()}function Ct(e){return e.mode&1?A&2&&le!==0?le&-le:wp.transition!==null?(ll===0&&(ll=Tu()),ll):(e=D,e!==0||(e=window.event,e=e===void 0?16:Iu(e.type)),e):1}function Be(e,t,n,r){if(50<er)throw er=0,Ci=null,Error(k(185));vr(e,n,r),(!(A&2)||e!==te)&&(e===te&&(!(A&2)&&(jl|=n),q===4&&pt(e,le)),ke(e,r),n===1&&A===0&&!(t.mode&1)&&(Cn=K()+500,$l&&zt()))}function ke(e,t){var n=e.callbackNode;Sf(e,t);var r=cl(e,e===te?le:0);if(r===0)n!==null&&cs(n),e.callbackNode=null,e.callbackPriority=0;else if(t=r&-r,e.callbackPriority!==t){if(n!=null&&cs(n),t===1)e.tag===0?xp(ru.bind(null,e)):nc(ru.bind(null,e)),gp(function(){!(A&6)&&zt()}),n=null;else{switch(Ru(r)){case 1:n=Mi;break;case 4:n=zu;break;case 16:n=ul;break;case 536870912:n=Pu;break;default:n=ul}n=ed(n,Gc.bind(null,e))}e.callbackPriority=t,e.callbackNode=n}}function Gc(e,t){if(rl=-1,ll=0,A&6)throw Error(k(327));var n=e.callbackNode;if(hn()&&e.callbackNode!==n)return null;var r=cl(e,e===te?le:0);if(r===0)return null;if(r&30||r&e.expiredLanes||t)t=zl(e,r);else{t=r;var l=A;A|=2;var o=Yc();(te!==e||le!==t)&&(Je=null,Cn=K()+500,Ft(e,t));do try{Up();break}catch(a){Kc(e,a)}while(!0);bi(),Nl.current=o,A=l,X!==null?t=0:(te=null,le=0,t=q)}if(t!==0){if(t===2&&(l=Yo(e),l!==0&&(r=l,t=Si(e,l))),t===1)throw n=yr,Ft(e,0),pt(e,r),ke(e,K()),n;if(t===6)pt(e,r);else{if(l=e.current.alternate,!(r&30)&&!jp(l)&&(t=zl(e,r),t===2&&(o=Yo(e),o!==0&&(r=o,t=Si(e,o))),t===1))throw n=yr,Ft(e,0),pt(e,r),ke(e,K()),n;switch(e.finishedWork=l,e.finishedLanes=r,t){case 0:case 1:throw Error(k(345));case 2:Dt(e,he,Je);break;case 3:if(pt(e,r),(r&130023424)===r&&(t=ia+500-K(),10<t)){if(cl(e,0)!==0)break;if(l=e.suspendedLanes,(l&r)!==r){pe(),e.pingedLanes|=e.suspendedLanes&l;break}e.timeoutHandle=ri(Dt.bind(null,e,he,Je),t);break}Dt(e,he,Je);break;case 4:if(pt(e,r),(r&4194240)===r)break;for(t=e.eventTimes,l=-1;0<r;){var i=31-je(r);o=1<<i,i=t[i],i>l&&(l=i),r&=~o}if(r=l,r=K()-r,r=(120>r?120:480>r?480:1080>r?1080:1920>r?1920:3e3>r?3e3:4320>r?4320:1960*Fp(r/1960))-r,10<r){e.timeoutHandle=ri(Dt.bind(null,e,he,Je),r);break}Dt(e,he,Je);break;case 5:Dt(e,he,Je);break;default:throw Error(k(329))}}}return ke(e,K()),e.callbackNode===n?Gc.bind(null,e):null}function Si(e,t){var n=qn;return e.current.memoizedState.isDehydrated&&(Ft(e,t).flags|=256),e=zl(e,t),e!==2&&(t=he,he=n,t!==null&&Ei(t)),e}function Ei(e){he===null?he=e:he.push.apply(he,e)}function jp(e){for(var t=e;;){if(t.flags&16384){var n=t.updateQueue;if(n!==null&&(n=n.stores,n!==null))for(var r=0;r<n.length;r++){var l=n[r],o=l.getSnapshot;l=l.value;try{if(!Ue(o(),l))return!1}catch{return!1}}}if(n=t.child,t.subtreeFlags&16384&&n!==null)n.return=t,t=n;else{if(t===e)break;for(;t.sibling===null;){if(t.return===null||t.return===e)return!0;t=t.return}t.sibling.return=t.return,t=t.sibling}}return!0}function pt(e,t){for(t&=~oa,t&=~jl,e.suspendedLanes|=t,e.pingedLanes&=~t,e=e.expirationTimes;0<t;){var n=31-je(t),r=1<<n;e[n]=-1,t&=~r}}function ru(e){if(A&6)throw Error(k(327));hn();var t=cl(e,0);if(!(t&1))return ke(e,K()),null;var n=zl(e,t);if(e.tag!==0&&n===2){var r=Yo(e);r!==0&&(t=r,n=Si(e,r))}if(n===1)throw n=yr,Ft(e,0),pt(e,t),ke(e,K()),n;if(n===6)throw Error(k(345));return e.finishedWork=e.current.alternate,e.finishedLanes=t,Dt(e,he,Je),ke(e,K()),null}function aa(e,t){var n=A;A|=1;try{return e(t)}finally{A=n,A===0&&(Cn=K()+500,$l&&zt())}}function Vt(e){ht!==null&&ht.tag===0&&!(A&6)&&hn();var t=A;A|=1;var n=Re.transition,r=D;try{if(Re.transition=null,D=1,e)return e()}finally{D=r,Re.transition=n,A=t,!(A&6)&&zt()}}function sa(){we=un.current,B(un)}function Ft(e,t){e.finishedWork=null,e.finishedLanes=0;var n=e.timeoutHandle;if(n!==-1&&(e.timeoutHandle=-1,hp(n)),X!==null)for(n=X.return;n!==null;){var r=n;switch(Wi(r),r.tag){case 1:r=r.type.childContextTypes,r!=null&&hl();break;case 3:xn(),B(ye),B(ce),Xi();break;case 5:Zi(r);break;case 4:xn();break;case 13:B(H);break;case 19:B(H);break;case 10:Qi(r.type._context);break;case 22:case 23:sa()}n=n.return}if(te=e,X=e=St(e.current,null),le=we=t,q=0,yr=null,oa=jl=Ht=0,he=qn=null,Ot!==null){for(t=0;t<Ot.length;t++)if(n=Ot[t],r=n.interleaved,r!==null){n.interleaved=null;var l=r.next,o=n.pending;if(o!==null){var i=o.next;o.next=l,r.next=i}n.pending=r}Ot=null}return e}function Kc(e,t){do{var n=X;try{if(bi(),el.current=El,Sl){for(var r=V.memoizedState;r!==null;){var l=r.queue;l!==null&&(l.pending=null),r=r.next}Sl=!1}if(Wt=0,ee=J=V=null,Xn=!1,mr=0,la.current=null,n===null||n.return===null){q=1,yr=t,X=null;break}e:{var o=e,i=n.return,a=n,s=t;if(t=le,a.flags|=32768,s!==null&&typeof s=="object"&&typeof s.then=="function"){var d=s,g=a,v=g.tag;if(!(g.mode&1)&&(v===0||v===11||v===15)){var y=g.alternate;y?(g.updateQueue=y.updateQueue,g.memoizedState=y.memoizedState,g.lanes=y.lanes):(g.updateQueue=null,g.memoizedState=null)}var w=Vs(i);if(w!==null){w.flags&=-257,bs(w,i,a,o,t),w.mode&1&&Hs(o,d,t),t=w,s=d;var S=t.updateQueue;if(S===null){var C=new Set;C.add(s),t.updateQueue=C}else S.add(s);break e}else{if(!(t&1)){Hs(o,d,t),ua();break e}s=Error(k(426))}}else if(U&&a.mode&1){var W=Vs(i);if(W!==null){!(W.flags&65536)&&(W.flags|=256),bs(W,i,a,o,t),Hi(wn(s,a));break e}}o=s=wn(s,a),q!==4&&(q=2),qn===null?qn=[o]:qn.push(o),o=i;do{switch(o.tag){case 3:o.flags|=65536,t&=-t,o.lanes|=t;var f=Rc(o,s,t);Is(o,f);break e;case 1:a=s;var c=o.type,p=o.stateNode;if(!(o.flags&128)&&(typeof c.getDerivedStateFromError=="function"||p!==null&&typeof p.componentDidCatch=="function"&&(wt===null||!wt.has(p)))){o.flags|=65536,t&=-t,o.lanes|=t;var x=Mc(o,a,t);Is(o,x);break e}}o=o.return}while(o!==null)}Xc(n)}catch(E){t=E,X===n&&n!==null&&(X=n=n.return);continue}break}while(!0)}function Yc(){var e=Nl.current;return Nl.current=El,e===null?El:e}function ua(){(q===0||q===3||q===2)&&(q=4),te===null||!(Ht&268435455)&&!(jl&268435455)||pt(te,le)}function zl(e,t){var n=A;A|=2;var r=Yc();(te!==e||le!==t)&&(Je=null,Ft(e,t));do try{Bp();break}catch(l){Kc(e,l)}while(!0);if(bi(),A=n,Nl.current=r,X!==null)throw Error(k(261));return te=null,le=0,q}function Bp(){for(;X!==null;)Zc(X)}function Up(){for(;X!==null&&!mf();)Zc(X)}function Zc(e){var t=qc(e.alternate,e,we);e.memoizedProps=e.pendingProps,t===null?Xc(e):X=t,la.current=null}function Xc(e){var t=e;do{var n=t.alternate;if(e=t.return,t.flags&32768){if(n=Dp(n,t),n!==null){n.flags&=32767,X=n;return}if(e!==null)e.flags|=32768,e.subtreeFlags=0,e.deletions=null;else{q=6,X=null;return}}else if(n=Ap(n,t,we),n!==null){X=n;return}if(t=t.sibling,t!==null){X=t;return}X=t=e}while(t!==null);q===0&&(q=5)}function Dt(e,t,n){var r=D,l=Re.transition;try{Re.transition=null,D=1,Wp(e,t,n,r)}finally{Re.transition=l,D=r}return null}function Wp(e,t,n,r){do hn();while(ht!==null);if(A&6)throw Error(k(327));n=e.finishedWork;var l=e.finishedLanes;if(n===null)return null;if(e.finishedWork=null,e.finishedLanes=0,n===e.current)throw Error(k(177));e.callbackNode=null,e.callbackPriority=0;var o=n.lanes|n.childLanes;if(Ef(e,o),e===te&&(X=te=null,le=0),!(n.subtreeFlags&2064)&&!(n.flags&2064)||Yr||(Yr=!0,ed(ul,function(){return hn(),null})),o=(n.flags&15990)!==0,n.subtreeFlags&15990||o){o=Re.transition,Re.transition=null;var i=D;D=1;var a=A;A|=4,la.current=null,Op(e,n),bc(n,e),cp(ti),dl=!!ei,ti=ei=null,e.current=n,Ip(n,e,l),hf(),A=a,D=i,Re.transition=o}else e.current=n;if(Yr&&(Yr=!1,ht=e,_l=l),o=e.pendingLanes,o===0&&(wt=null),vf(n.stateNode,r),ke(e,K()),t!==null)for(r=e.onRecoverableError,n=0;n<t.length;n++)l=t[n],r(l.value,{componentStack:l.stack,digest:l.digest});if(Ll)throw Ll=!1,e=wi,wi=null,e;return _l&1&&e.tag!==0&&hn(),o=e.pendingLanes,o&1?e===Ci?er++:(er=0,Ci=e):er=0,zt(),null}function hn(){if(ht!==null){var e=Ru(_l),t=Re.transition,n=D;try{if(Re.transition=null,D=16>e?16:e,ht===null)var r=!1;else{if(e=ht,ht=null,_l=0,A&6)throw Error(k(331));var l=A;for(A|=4,N=e.current;N!==null;){var o=N,i=o.child;if(N.flags&16){var a=o.deletions;if(a!==null){for(var s=0;s<a.length;s++){var d=a[s];for(N=d;N!==null;){var g=N;switch(g.tag){case 0:case 11:case 15:Jn(8,g,o)}var v=g.child;if(v!==null)v.return=g,N=v;else for(;N!==null;){g=N;var y=g.sibling,w=g.return;if(Wc(g),g===d){N=null;break}if(y!==null){y.return=w,N=y;break}N=w}}}var S=o.alternate;if(S!==null){var C=S.child;if(C!==null){S.child=null;do{var W=C.sibling;C.sibling=null,C=W}while(C!==null)}}N=o}}if(o.subtreeFlags&2064&&i!==null)i.return=o,N=i;else e:for(;N!==null;){if(o=N,o.flags&2048)switch(o.tag){case 0:case 11:case 15:Jn(9,o,o.return)}var f=o.sibling;if(f!==null){f.return=o.return,N=f;break e}N=o.return}}var c=e.current;for(N=c;N!==null;){i=N;var p=i.child;if(i.subtreeFlags&2064&&p!==null)p.return=i,N=p;else e:for(i=c;N!==null;){if(a=N,a.flags&2048)try{switch(a.tag){case 0:case 11:case 15:Fl(9,a)}}catch(E){Q(a,a.return,E)}if(a===i){N=null;break e}var x=a.sibling;if(x!==null){x.return=a.return,N=x;break e}N=a.return}}if(A=l,zt(),Qe&&typeof Qe.onPostCommitFiberRoot=="function")try{Qe.onPostCommitFiberRoot(Tl,e)}catch{}r=!0}return r}finally{D=n,Re.transition=t}}return!1}function lu(e,t,n){t=wn(n,t),t=Rc(e,t,1),e=xt(e,t,1),t=pe(),e!==null&&(vr(e,1,t),ke(e,t))}function Q(e,t,n){if(e.tag===3)lu(e,e,n);else for(;t!==null;){if(t.tag===3){lu(t,e,n);break}else if(t.tag===1){var r=t.stateNode;if(typeof t.type.getDerivedStateFromError=="function"||typeof r.componentDidCatch=="function"&&(wt===null||!wt.has(r))){e=wn(n,e),e=Mc(t,e,1),t=xt(t,e,1),e=pe(),t!==null&&(vr(t,1,e),ke(t,e));break}}t=t.return}}function Hp(e,t,n){var r=e.pingCache;r!==null&&r.delete(t),t=pe(),e.pingedLanes|=e.suspendedLanes&n,te===e&&(le&n)===n&&(q===4||q===3&&(le&130023424)===le&&500>K()-ia?Ft(e,0):oa|=n),ke(e,t)}function Jc(e,t){t===0&&(e.mode&1?(t=$r,$r<<=1,!($r&130023424)&&($r=4194304)):t=1);var n=pe();e=ot(e,t),e!==null&&(vr(e,t,n),ke(e,n))}function Vp(e){var t=e.memoizedState,n=0;t!==null&&(n=t.retryLane),Jc(e,n)}function bp(e,t){var n=0;switch(e.tag){case 13:var r=e.stateNode,l=e.memoizedState;l!==null&&(n=l.retryLane);break;case 19:r=e.stateNode;break;default:throw Error(k(314))}r!==null&&r.delete(t),Jc(e,n)}var qc;qc=function(e,t,n){if(e!==null)if(e.memoizedProps!==t.pendingProps||ye.current)ge=!0;else{if(!(e.lanes&n)&&!(t.flags&128))return ge=!1,Mp(e,t,n);ge=!!(e.flags&131072)}else ge=!1,U&&t.flags&1048576&&rc(t,vl,t.index);switch(t.lanes=0,t.tag){case 2:var r=t.type;nl(e,t),e=t.pendingProps;var l=yn(t,ce.current);mn(t,n),l=qi(null,t,r,e,l,n);var o=ea();return t.flags|=1,typeof l=="object"&&l!==null&&typeof l.render=="function"&&l.$$typeof===void 0?(t.tag=1,t.memoizedState=null,t.updateQueue=null,ve(r)?(o=!0,gl(t)):o=!1,t.memoizedState=l.state!==null&&l.state!==void 0?l.state:null,Ki(t),l.updater=Il,t.stateNode=l,l._reactInternals=t,ci(t,r,e,n),t=pi(null,t,r,!0,o,n)):(t.tag=0,U&&o&&Ui(t),fe(null,t,l,n),t=t.child),t;case 16:r=t.elementType;e:{switch(nl(e,t),e=t.pendingProps,l=r._init,r=l(r._payload),t.type=r,l=t.tag=Gp(r),e=Oe(r,e),l){case 0:t=fi(null,t,r,e,n);break e;case 1:t=Ks(null,t,r,e,n);break e;case 11:t=Qs(null,t,r,e,n);break e;case 14:t=Gs(null,t,r,Oe(r.type,e),n);break e}throw Error(k(306,r,""))}return t;case 0:return r=t.type,l=t.pendingProps,l=t.elementType===r?l:Oe(r,l),fi(e,t,r,l,n);case 1:return r=t.type,l=t.pendingProps,l=t.elementType===r?l:Oe(r,l),Ks(e,t,r,l,n);case 3:e:{if(Oc(t),e===null)throw Error(k(387));r=t.pendingProps,o=t.memoizedState,l=o.element,uc(e,t),wl(t,r,null,n);var i=t.memoizedState;if(r=i.element,o.isDehydrated)if(o={element:r,isDehydrated:!1,cache:i.cache,pendingSuspenseBoundaries:i.pendingSuspenseBoundaries,transitions:i.transitions},t.updateQueue.baseState=o,t.memoizedState=o,t.flags&256){l=wn(Error(k(423)),t),t=Ys(e,t,r,n,l);break e}else if(r!==l){l=wn(Error(k(424)),t),t=Ys(e,t,r,n,l);break e}else for(Ce=kt(t.stateNode.containerInfo.firstChild),Se=t,U=!0,Fe=null,n=ac(t,null,r,n),t.child=n;n;)n.flags=n.flags&-3|4096,n=n.sibling;else{if(vn(),r===l){t=it(e,t,n);break e}fe(e,t,r,n)}t=t.child}return t;case 5:return cc(t),e===null&&ai(t),r=t.type,l=t.pendingProps,o=e!==null?e.memoizedProps:null,i=l.children,ni(r,l)?i=null:o!==null&&ni(r,o)&&(t.flags|=32),$c(e,t),fe(e,t,i,n),t.child;case 6:return e===null&&ai(t),null;case 13:return Ic(e,t,n);case 4:return Yi(t,t.stateNode.containerInfo),r=t.pendingProps,e===null?t.child=kn(t,null,r,n):fe(e,t,r,n),t.child;case 11:return r=t.type,l=t.pendingProps,l=t.elementType===r?l:Oe(r,l),Qs(e,t,r,l,n);case 7:return fe(e,t,t.pendingProps,n),t.child;case 8:return fe(e,t,t.pendingProps.children,n),t.child;case 12:return fe(e,t,t.pendingProps.children,n),t.child;case 10:e:{if(r=t.type._context,l=t.pendingProps,o=t.memoizedProps,i=l.value,F(kl,r._currentValue),r._currentValue=i,o!==null)if(Ue(o.value,i)){if(o.children===l.children&&!ye.current){t=it(e,t,n);break e}}else for(o=t.child,o!==null&&(o.return=t);o!==null;){var a=o.dependencies;if(a!==null){i=o.child;for(var s=a.firstContext;s!==null;){if(s.context===r){if(o.tag===1){s=nt(-1,n&-n),s.tag=2;var d=o.updateQueue;if(d!==null){d=d.shared;var g=d.pending;g===null?s.next=s:(s.next=g.next,g.next=s),d.pending=s}}o.lanes|=n,s=o.alternate,s!==null&&(s.lanes|=n),si(o.return,n,t),a.lanes|=n;break}s=s.next}}else if(o.tag===10)i=o.type===t.type?null:o.child;else if(o.tag===18){if(i=o.return,i===null)throw Error(k(341));i.lanes|=n,a=i.alternate,a!==null&&(a.lanes|=n),si(i,n,t),i=o.sibling}else i=o.child;if(i!==null)i.return=o;else for(i=o;i!==null;){if(i===t){i=null;break}if(o=i.sibling,o!==null){o.return=i.return,i=o;break}i=i.return}o=i}fe(e,t,l.children,n),t=t.child}return t;case 9:return l=t.type,r=t.pendingProps.children,mn(t,n),l=Me(l),r=r(l),t.flags|=1,fe(e,t,r,n),t.child;case 14:return r=t.type,l=Oe(r,t.pendingProps),l=Oe(r.type,l),Gs(e,t,r,l,n);case 15:return Ac(e,t,t.type,t.pendingProps,n);case 17:return r=t.type,l=t.pendingProps,l=t.elementType===r?l:Oe(r,l),nl(e,t),t.tag=1,ve(r)?(e=!0,gl(t)):e=!1,mn(t,n),Tc(t,r,l),ci(t,r,l,n),pi(null,t,r,!0,e,n);case 19:return Fc(e,t,n);case 22:return Dc(e,t,n)}throw Error(k(156,t.tag))};function ed(e,t){return _u(e,t)}function Qp(e,t,n,r){this.tag=e,this.key=n,this.sibling=this.child=this.return=this.stateNode=this.type=this.elementType=null,this.index=0,this.ref=null,this.pendingProps=t,this.dependencies=this.memoizedState=this.updateQueue=this.memoizedProps=null,this.mode=r,this.subtreeFlags=this.flags=0,this.deletions=null,this.childLanes=this.lanes=0,this.alternate=null}function Te(e,t,n,r){return new Qp(e,t,n,r)}function ca(e){return e=e.prototype,!(!e||!e.isReactComponent)}function Gp(e){if(typeof e=="function")return ca(e)?1:0;if(e!=null){if(e=e.$$typeof,e===Pi)return 11;if(e===Ti)return 14}return 2}function St(e,t){var n=e.alternate;return n===null?(n=Te(e.tag,t,e.key,e.mode),n.elementType=e.elementType,n.type=e.type,n.stateNode=e.stateNode,n.alternate=e,e.alternate=n):(n.pendingProps=t,n.type=e.type,n.flags=0,n.subtreeFlags=0,n.deletions=null),n.flags=e.flags&14680064,n.childLanes=e.childLanes,n.lanes=e.lanes,n.child=e.child,n.memoizedProps=e.memoizedProps,n.memoizedState=e.memoizedState,n.updateQueue=e.updateQueue,t=e.dependencies,n.dependencies=t===null?null:{lanes:t.lanes,firstContext:t.firstContext},n.sibling=e.sibling,n.index=e.index,n.ref=e.ref,n}function ol(e,t,n,r,l,o){var i=2;if(r=e,typeof e=="function")ca(e)&&(i=1);else if(typeof e=="string")i=5;else e:switch(e){case Jt:return jt(n.children,l,o,t);case zi:i=8,l|=8;break;case Do:return e=Te(12,n,t,l|2),e.elementType=Do,e.lanes=o,e;case $o:return e=Te(13,n,t,l),e.elementType=$o,e.lanes=o,e;case Oo:return e=Te(19,n,t,l),e.elementType=Oo,e.lanes=o,e;case cu:return Bl(n,l,o,t);default:if(typeof e=="object"&&e!==null)switch(e.$$typeof){case su:i=10;break e;case uu:i=9;break e;case Pi:i=11;break e;case Ti:i=14;break e;case ct:i=16,r=null;break e}throw Error(k(130,e==null?e:typeof e,""))}return t=Te(i,n,t,l),t.elementType=e,t.type=r,t.lanes=o,t}function jt(e,t,n,r){return e=Te(7,e,r,t),e.lanes=n,e}function Bl(e,t,n,r){return e=Te(22,e,r,t),e.elementType=cu,e.lanes=n,e.stateNode={isHidden:!1},e}function Ro(e,t,n){return e=Te(6,e,null,t),e.lanes=n,e}function Mo(e,t,n){return t=Te(4,e.children!==null?e.children:[],e.key,t),t.lanes=n,t.stateNode={containerInfo:e.containerInfo,pendingChildren:null,implementation:e.implementation},t}function Kp(e,t,n,r,l){this.tag=t,this.containerInfo=e,this.finishedWork=this.pingCache=this.current=this.pendingChildren=null,this.timeoutHandle=-1,this.callbackNode=this.pendingContext=this.context=null,this.callbackPriority=0,this.eventTimes=ho(0),this.expirationTimes=ho(-1),this.entangledLanes=this.finishedLanes=this.mutableReadLanes=this.expiredLanes=this.pingedLanes=this.suspendedLanes=this.pendingLanes=0,this.entanglements=ho(0),this.identifierPrefix=r,this.onRecoverableError=l,this.mutableSourceEagerHydrationData=null}function da(e,t,n,r,l,o,i,a,s){return e=new Kp(e,t,n,a,s),t===1?(t=1,o===!0&&(t|=8)):t=0,o=Te(3,null,null,t),e.current=o,o.stateNode=e,o.memoizedState={element:r,isDehydrated:n,cache:null,transitions:null,pendingSuspenseBoundaries:null},Ki(o),e}function Yp(e,t,n){var r=3<arguments.length&&arguments[3]!==void 0?arguments[3]:null;return{$$typeof:Xt,key:r==null?null:""+r,children:e,containerInfo:t,implementation:n}}function td(e){if(!e)return Nt;e=e._reactInternals;e:{if(Qt(e)!==e||e.tag!==1)throw Error(k(170));var t=e;do{switch(t.tag){case 3:t=t.stateNode.context;break e;case 1:if(ve(t.type)){t=t.stateNode.__reactInternalMemoizedMergedChildContext;break e}}t=t.return}while(t!==null);throw Error(k(171))}if(e.tag===1){var n=e.type;if(ve(n))return tc(e,n,t)}return t}function nd(e,t,n,r,l,o,i,a,s){return e=da(n,r,!0,e,l,o,i,a,s),e.context=td(null),n=e.current,r=pe(),l=Ct(n),o=nt(r,l),o.callback=t??null,xt(n,o,l),e.current.lanes=l,vr(e,l,r),ke(e,r),e}function Ul(e,t,n,r){var l=t.current,o=pe(),i=Ct(l);return n=td(n),t.context===null?t.context=n:t.pendingContext=n,t=nt(o,i),t.payload={element:e},r=r===void 0?null:r,r!==null&&(t.callback=r),e=xt(l,t,i),e!==null&&(Be(e,l,i,o),qr(e,l,i)),i}function Pl(e){if(e=e.current,!e.child)return null;switch(e.child.tag){case 5:return e.child.stateNode;default:return e.child.stateNode}}function ou(e,t){if(e=e.memoizedState,e!==null&&e.dehydrated!==null){var n=e.retryLane;e.retryLane=n!==0&&n<t?n:t}}function fa(e,t){ou(e,t),(e=e.alternate)&&ou(e,t)}function Zp(){return null}var rd=typeof reportError=="function"?reportError:function(e){console.error(e)};function pa(e){this._internalRoot=e}Wl.prototype.render=pa.prototype.render=function(e){var t=this._internalRoot;if(t===null)throw Error(k(409));Ul(e,t,null,null)};Wl.prototype.unmount=pa.prototype.unmount=function(){var e=this._internalRoot;if(e!==null){this._internalRoot=null;var t=e.containerInfo;Vt(function(){Ul(null,e,null,null)}),t[lt]=null}};function Wl(e){this._internalRoot=e}Wl.prototype.unstable_scheduleHydration=function(e){if(e){var t=Du();e={blockedOn:null,target:e,priority:t};for(var n=0;n<ft.length&&t!==0&&t<ft[n].priority;n++);ft.splice(n,0,e),n===0&&Ou(e)}};function ma(e){return!(!e||e.nodeType!==1&&e.nodeType!==9&&e.nodeType!==11)}function Hl(e){return!(!e||e.nodeType!==1&&e.nodeType!==9&&e.nodeType!==11&&(e.nodeType!==8||e.nodeValue!==" react-mount-point-unstable "))}function iu(){}function Xp(e,t,n,r,l){if(l){if(typeof r=="function"){var o=r;r=function(){var d=Pl(i);o.call(d)}}var i=nd(t,r,e,0,null,!1,!1,"",iu);return e._reactRootContainer=i,e[lt]=i.current,ur(e.nodeType===8?e.parentNode:e),Vt(),i}for(;l=e.lastChild;)e.removeChild(l);if(typeof r=="function"){var a=r;r=function(){var d=Pl(s);a.call(d)}}var s=da(e,0,!1,null,null,!1,!1,"",iu);return e._reactRootContainer=s,e[lt]=s.current,ur(e.nodeType===8?e.parentNode:e),Vt(function(){Ul(t,s,n,r)}),s}function Vl(e,t,n,r,l){var o=n._reactRootContainer;if(o){var i=o;if(typeof l=="function"){var a=l;l=function(){var s=Pl(i);a.call(s)}}Ul(t,i,e,l)}else i=Xp(n,t,e,l,r);return Pl(i)}Mu=function(e){switch(e.tag){case 3:var t=e.stateNode;if(t.current.memoizedState.isDehydrated){var n=Vn(t.pendingLanes);n!==0&&(Ai(t,n|1),ke(t,K()),!(A&6)&&(Cn=K()+500,zt()))}break;case 13:Vt(function(){var r=ot(e,1);if(r!==null){var l=pe();Be(r,e,1,l)}}),fa(e,1)}};Di=function(e){if(e.tag===13){var t=ot(e,134217728);if(t!==null){var n=pe();Be(t,e,134217728,n)}fa(e,134217728)}};Au=function(e){if(e.tag===13){var t=Ct(e),n=ot(e,t);if(n!==null){var r=pe();Be(n,e,t,r)}fa(e,t)}};Du=function(){return D};$u=function(e,t){var n=D;try{return D=e,t()}finally{D=n}};Qo=function(e,t,n){switch(t){case"input":if(jo(e,n),t=n.name,n.type==="radio"&&t!=null){for(n=e;n.parentNode;)n=n.parentNode;for(n=n.querySelectorAll("input[name="+JSON.stringify(""+t)+'][type="radio"]'),t=0;t<n.length;t++){var r=n[t];if(r!==e&&r.form===e.form){var l=Dl(r);if(!l)throw Error(k(90));fu(r),jo(r,l)}}}break;case"textarea":mu(e,n);break;case"select":t=n.value,t!=null&&cn(e,!!n.multiple,t,!1)}};wu=aa;Cu=Vt;var Jp={usingClientEntryPoint:!1,Events:[xr,nn,Dl,ku,xu,aa]},Bn={findFiberByHostInstance:$t,bundleType:0,version:"18.3.1",rendererPackageName:"react-dom"},qp={bundleType:Bn.bundleType,version:Bn.version,rendererPackageName:Bn.rendererPackageName,rendererConfig:Bn.rendererConfig,overrideHookState:null,overrideHookStateDeletePath:null,overrideHookStateRenamePath:null,overrideProps:null,overridePropsDeletePath:null,overridePropsRenamePath:null,setErrorHandler:null,setSuspenseHandler:null,scheduleUpdate:null,currentDispatcherRef:at.ReactCurrentDispatcher,findHostInstanceByFiber:function(e){return e=Nu(e),e===null?null:e.stateNode},findFiberByHostInstance:Bn.findFiberByHostInstance||Zp,findHostInstancesForRefresh:null,scheduleRefresh:null,scheduleRoot:null,setRefreshHandler:null,getCurrentFiber:null,reconcilerVersion:"18.3.1-next-f1338f8080-20240426"};if(typeof __REACT_DEVTOOLS_GLOBAL_HOOK__<"u"&&(Un=__REACT_DEVTOOLS_GLOBAL_HOOK__,!Un.isDisabled&&Un.supportsFiber))try{Tl=Un.inject(qp),Qe=Un}catch{}var Un;Le.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED=Jp;Le.createPortal=function(e,t){var n=2<arguments.length&&arguments[2]!==void 0?arguments[2]:null;if(!ma(t))throw Error(k(200));return Yp(e,t,null,n)};Le.createRoot=function(e,t){if(!ma(e))throw Error(k(299));var n=!1,r="",l=rd;return t!=null&&(t.unstable_strictMode===!0&&(n=!0),t.identifierPrefix!==void 0&&(r=t.identifierPrefix),t.onRecoverableError!==void 0&&(l=t.onRecoverableError)),t=da(e,1,!1,null,null,n,!1,r,l),e[lt]=t.current,ur(e.nodeType===8?e.parentNode:e),new pa(t)};Le.findDOMNode=function(e){if(e==null)return null;if(e.nodeType===1)return e;var t=e._reactInternals;if(t===void 0)throw typeof e.render=="function"?Error(k(188)):(e=Object.keys(e).join(","),Error(k(268,e)));return e=Nu(t),e=e===null?null:e.stateNode,e};Le.flushSync=function(e){return Vt(e)};Le.hydrate=function(e,t,n){if(!Hl(t))throw Error(k(200));return Vl(null,e,t,!0,n)};Le.hydrateRoot=function(e,t,n){if(!ma(e))throw Error(k(405));var r=n!=null&&n.hydratedSources||null,l=!1,o="",i=rd;if(n!=null&&(n.unstable_strictMode===!0&&(l=!0),n.identifierPrefix!==void 0&&(o=n.identifierPrefix),n.onRecoverableError!==void 0&&(i=n.onRecoverableError)),t=nd(t,null,e,1,n??null,l,!1,o,i),e[lt]=t.current,ur(e),r)for(e=0;e<r.length;e++)n=r[e],l=n._getVersion,l=l(n._source),t.mutableSourceEagerHydrationData==null?t.mutableSourceEagerHydrationData=[n,l]:t.mutableSourceEagerHydrationData.push(n,l);return new Wl(t)};Le.render=function(e,t,n){if(!Hl(t))throw Error(k(200));return Vl(null,e,t,!1,n)};Le.unmountComponentAtNode=function(e){if(!Hl(e))throw Error(k(40));return e._reactRootContainer?(Vt(function(){Vl(null,null,e,!1,function(){e._reactRootContainer=null,e[lt]=null})}),!0):!1};Le.unstable_batchedUpdates=aa;Le.unstable_renderSubtreeIntoContainer=function(e,t,n,r){if(!Hl(n))throw Error(k(200));if(e==null||e._reactInternals===void 0)throw Error(k(38));return Vl(e,t,n,!1,r)};Le.version="18.3.1-next-f1338f8080-20240426"});var ad=Xe((k1,id)=>{"use strict";function od(){if(!(typeof __REACT_DEVTOOLS_GLOBAL_HOOK__>"u"||typeof __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE!="function"))try{__REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE(od)}catch(e){console.error(e)}}od(),id.exports=ld()});var ud=Xe(ha=>{"use strict";var sd=ad();ha.createRoot=sd.createRoot,ha.hydrateRoot=sd.hydrateRoot;var x1});var dd=Xe(bl=>{"use strict";var e1=Tn(),t1=Symbol.for("react.element"),n1=Symbol.for("react.fragment"),r1=Object.prototype.hasOwnProperty,l1=e1.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED.ReactCurrentOwner,o1={key:!0,ref:!0,__self:!0,__source:!0};function cd(e,t,n){var r,l={},o=null,i=null;n!==void 0&&(o=""+n),t.key!==void 0&&(o=""+t.key),t.ref!==void 0&&(i=t.ref);for(r in t)r1.call(t,r)&&!o1.hasOwnProperty(r)&&(l[r]=t[r]);if(e&&e.defaultProps)for(r in t=e.defaultProps,t)l[r]===void 0&&(l[r]=t[r]);return{$$typeof:t1,type:e,key:o,ref:i,props:l,_owner:l1.current}}bl.Fragment=n1;bl.jsx=cd;bl.jsxs=cd});var ga=Xe((S1,fd)=>{"use strict";fd.exports=dd()});var yd=zn(Tn()),vd=zn(ud());var G=zn(Tn()),u=zn(ga()),Gl="#0205C6",Cr=({height:e=28,color:t="currentColor",markOnly:n=!1,style:r,className:l})=>(0,u.jsxs)("svg",{viewBox:n?"8 1 289 356":"0 0 1688 508",height:e,className:l,style:{display:"block",overflow:"visible",...r},role:"img","aria-label":"Gentrep",children:[!n&&(0,u.jsx)("path",{d:"M198.0 502.4C196.6 502.2 190.3 501.3 184.0 500.4C154.0 496.1 125.7 484.6 105.7 468.5C103.7 466.9 102.0 465.1 102.0 464.6C102.0 463.5 116.8 441.3 118.0 440.5C118.5 440.2 122.1 442.5 126.2 445.6C130.2 448.6 139.3 454.0 146.5 457.5C169.2 468.6 189.8 473.2 217.0 473.3C269.8 473.4 298.1 453.8 307.0 411.0C308.8 402.5 309.3 395.8 309.7 375.8C310.3 350.0 309.9 347.5 306.4 354.2C304.1 358.7 288.6 374.0 281.5 378.7C261.5 392.1 239.0 398.4 211.0 398.4C194.6 398.4 180.8 396.3 167.6 391.8C131.6 379.6 104.2 352.6 92.6 318.0C87.7 303.2 86.5 294.8 86.6 276.0C86.6 260.3 86.9 257.3 89.4 247.1C92.5 234.8 96.2 225.0 100.6 217.5L103.3 212.8L106.7 218.1C111.1 225.1 117.4 238.3 119.1 244.0C120.0 247.1 120.4 255.8 120.5 271.5C120.6 293.6 120.7 294.9 123.3 303.4C131.1 328.6 144.4 345.3 166.0 357.2C198.5 375.1 245.6 372.3 274.9 350.7C300.5 331.9 313.8 300.0 310.2 266.7C305.3 221.4 273.4 190.5 226.8 185.8C212.6 184.4 195.5 185.7 184.5 189.2C175.3 192.1 157.5 192.3 148.5 189.6C141.3 187.5 131.0 183.0 131.0 182.0C131.0 180.8 144.2 172.8 153.5 168.4C187.9 152.2 233.9 152.0 267.4 168.0C271.8 170.2 278.4 173.8 281.9 176.2C289.5 181.1 302.2 193.4 307.0 200.5L310.5 205.5L310.8 181.8L311.0 158.0L327.0 158.0L343.1 158.0L342.8 280.2L342.5 402.5L340.2 414.0C334.9 440.5 326.7 457.4 312.1 472.1C297.6 486.6 279.8 495.3 254.9 500.0C245.9 501.8 239.0 502.3 222.0 502.5C210.2 502.7 199.4 502.7 198.0 502.4ZM1448.7 468.4C1448.3 468.0 1448.0 398.2 1448.0 313.3L1448.0 159.0L1467.5 159.0L1487.0 159.0L1487.0 176.5C1487.0 186.1 1487.2 194.0 1487.4 194.0C1487.6 194.0 1490.9 190.8 1494.7 186.9C1502.6 178.6 1510.7 172.7 1520.6 167.7C1549.1 153.4 1591.9 153.9 1621.5 168.7C1651.6 183.8 1671.9 209.7 1679.8 243.4C1682.1 253.1 1682.4 256.7 1682.5 272.0C1682.5 286.8 1682.1 291.1 1680.2 300.0C1670.3 344.1 1641.0 374.5 1598.0 385.1C1589.7 387.2 1586.0 387.5 1569.5 387.5C1552.7 387.5 1549.4 387.2 1541.5 385.1C1524.0 380.6 1505.2 369.7 1494.8 358.1C1492.3 355.3 1489.9 353.0 1489.6 353.0C1489.3 353.0 1488.9 379.0 1488.8 410.8L1488.5 468.5L1468.9 468.8C1458.2 468.9 1449.1 468.7 1448.7 468.4ZM964.7 388.0C943.6 384.2 927.7 374.2 918.6 359.1C916.7 356.0 913.9 349.7 912.4 345.0L909.5 336.5L909.0 265.0L908.5 193.5L889.2 193.2L870.0 193.0L870.0 176.5L870.0 160.0L889.2 159.8L908.5 159.5L908.8 134.8L909.0 110.0L929.0 110.0L949.0 110.0L949.2 134.8L949.5 159.5L982.0 160.0L1014.5 160.5L1014.8 176.7L1015.0 193.0L982.3 193.2L949.5 193.5L949.5 259.5L949.5 325.5L951.9 332.5C955.0 341.4 960.7 347.7 969.3 351.6C974.9 354.2 976.5 354.4 986.0 354.3C997.4 354.2 1005.0 352.3 1012.2 347.5C1014.3 346.1 1016.3 345.0 1016.8 345.0C1017.2 345.0 1019.3 348.9 1021.4 353.8C1023.5 358.6 1026.3 364.9 1027.6 367.8L1030.0 373.2L1027.7 375.1C1023.7 378.6 1013.7 383.3 1005.0 385.7C995.6 388.4 973.7 389.7 964.7 388.0ZM474.0 387.4C445.4 382.3 430.4 376.0 412.0 361.4C393.5 346.7 381.3 326.8 374.9 301.0C372.9 292.8 372.6 289.0 372.5 273.0C372.5 257.2 372.8 253.0 374.8 244.0C383.9 203.7 411.7 173.7 450.9 162.1C472.8 155.6 499.5 155.6 521.5 162.2C557.3 173.0 583.1 200.7 593.5 239.5C595.8 248.1 596.3 252.1 596.7 267.8L597.2 286.0L505.1 286.0L413.0 286.0L413.0 288.3C413.0 289.5 413.9 293.8 415.0 297.8C426.3 338.5 469.7 360.5 518.0 350.0C532.2 346.9 544.4 340.5 554.8 330.7L560.2 325.5L564.2 330.0C573.9 340.8 582.0 350.8 582.0 352.0C582.0 353.8 573.3 362.0 565.7 367.3C554.1 375.6 540.5 381.5 524.5 385.2C517.3 386.9 511.6 387.3 496.0 387.6C485.3 387.7 475.4 387.6 474.0 387.4ZM1279.0 385.6C1255.2 380.7 1236.5 371.2 1220.6 355.9C1202.5 338.6 1191.8 318.1 1188.0 293.5C1185.1 275.2 1187.1 247.8 1192.4 232.2C1206.7 190.3 1242.6 162.2 1287.4 157.9C1349.2 151.9 1399.2 188.4 1409.5 247.0C1411.4 257.9 1412.5 275.3 1411.6 281.3L1410.9 286.0L1318.9 286.0L1227.0 286.0L1227.6 290.2C1227.9 292.6 1229.2 297.5 1230.5 301.2C1239.1 326.7 1260.8 345.1 1288.9 350.7C1299.7 352.9 1319.5 352.8 1330.2 350.7C1344.5 347.8 1358.7 340.6 1369.8 330.5C1372.7 327.9 1375.2 325.9 1375.4 326.1C1391.6 344.8 1397.0 351.3 1397.0 352.0C1397.0 353.5 1383.5 365.4 1376.6 369.9C1366.8 376.2 1353.5 381.7 1341.0 384.7C1332.1 386.9 1327.5 387.3 1310.5 387.6C1292.5 387.9 1289.4 387.7 1279.0 385.6ZM633.0 272.5L633.0 159.0L652.2 159.2L671.5 159.5L672.0 175.9L672.5 192.3L675.9 188.4C688.3 174.1 709.0 163.0 730.1 159.1C749.2 155.7 771.8 157.0 788.9 162.5C820.6 172.8 839.3 195.6 845.7 231.6C847.2 240.4 847.4 249.5 847.5 313.5L847.5 385.5L827.3 385.8L807.1 386.0L806.7 315.8C806.4 253.3 806.1 244.7 804.6 238.0C797.8 209.2 777.3 193.9 745.5 193.9C729.9 193.9 718.8 196.4 706.8 202.7C691.8 210.5 681.1 224.9 675.8 244.5C673.7 252.3 673.6 254.4 673.2 319.2L672.9 386.0L652.9 386.0L633.0 386.0L633.0 272.5ZM1059.5 384.8C1059.2 384.1 1059.1 333.1 1059.2 271.5L1059.5 159.5L1078.8 159.2L1098.0 159.0L1098.0 176.8C1098.0 186.6 1098.3 195.0 1098.6 195.3C1099.0 195.7 1100.6 194.0 1102.1 191.6C1108.1 182.6 1119.5 172.8 1130.6 167.2C1140.5 162.2 1164.8 157.0 1178.7 157.0L1181.0 157.0L1181.0 176.5L1181.0 196.0L1174.7 196.0C1166.0 196.0 1152.5 197.8 1146.5 199.7C1128.1 205.5 1113.6 218.7 1106.5 236.1C1100.7 250.4 1100.6 251.0 1100.0 321.0L1099.5 385.5L1079.7 385.8C1064.5 386.0 1059.8 385.8 1059.5 384.8ZM1584.1 350.5C1604.7 346.1 1623.6 331.1 1633.0 311.5C1637.7 301.7 1639.6 294.6 1641.1 281.4C1643.2 264.2 1639.2 243.8 1630.9 229.4C1617.9 206.5 1593.3 193.0 1565.0 193.0C1533.3 193.0 1507.5 209.5 1495.2 237.5C1487.0 256.2 1486.8 287.5 1494.7 306.4C1505.6 332.6 1526.2 347.9 1556.5 352.4C1561.6 353.1 1576.3 352.1 1584.1 350.5ZM557.7 251.1C556.3 238.3 548.2 222.4 537.6 212.0C529.5 204.1 521.1 198.9 510.5 195.3C502.9 192.6 501.5 192.5 485.0 192.5C468.3 192.6 467.1 192.7 460.0 195.4C443.0 201.8 428.9 213.8 421.2 228.8C417.0 236.7 413.0 249.3 413.0 254.2L413.0 257.0L485.6 257.0L558.3 257.0L557.7 251.1ZM1372.6 255.7C1373.3 253.7 1368.5 235.9 1365.7 230.4C1357.4 214.1 1343.2 201.7 1325.5 195.4C1317.9 192.6 1316.7 192.5 1300.0 192.5C1283.4 192.5 1282.1 192.7 1275.1 195.2C1254.0 203.1 1240.0 216.4 1232.0 236.4C1229.7 242.4 1227.0 252.8 1227.0 256.2C1227.0 256.6 1259.6 257.0 1299.5 257.0C1357.6 257.0 1372.2 256.7 1372.6 255.7Z",fill:t,fillRule:"evenodd"}),(0,u.jsx)("path",{d:"M201.0 351.6C172.3 345.2 151.1 326.4 142.0 299.3C138.8 289.7 138.7 289.1 138.0 265.0C137.0 233.8 135.5 227.6 126.2 214.5C120.2 206.2 114.8 200.1 109.1 195.5C102.2 189.7 98.8 189.6 88.8 194.6C78.6 199.7 73.7 201.0 63.5 201.0C49.0 201.0 38.5 196.7 28.4 186.6C17.3 175.5 11.2 157.5 13.9 144.3C14.6 141.1 15.3 137.8 15.4 137.0C15.9 134.0 19.0 128.0 23.0 122.1C31.4 109.6 47.9 101.0 63.5 101.0C70.1 101.0 78.1 103.1 90.6 108.0C98.6 111.2 98.8 111.2 102.3 109.5C107.2 107.2 132.7 80.8 135.1 75.6C137.5 70.2 137.5 64.7 134.9 57.4C133.3 52.8 132.9 49.8 133.2 43.5C133.9 28.9 142.0 16.7 155.4 9.7C161.2 6.7 162.1 6.5 172.5 6.5C183.0 6.5 183.9 6.7 190.2 9.8C206.1 17.6 215.2 35.0 212.1 51.6C211.4 55.3 209.7 60.8 208.3 63.7C205.0 70.4 196.7 78.3 189.3 81.8C183.7 84.4 182.9 84.5 166.0 84.5C151.5 84.5 148.0 84.8 145.4 86.2C137.6 90.5 111.9 113.3 109.4 118.2C107.4 122.1 107.7 125.4 110.7 133.9C114.3 144.2 114.5 157.3 111.1 167.2C109.9 170.9 108.4 174.2 107.9 174.5C107.4 174.9 107.0 176.9 107.0 179.2C107.0 182.4 107.6 183.8 110.1 186.1C115.0 190.7 128.8 199.5 137.5 203.6C144.3 206.9 146.6 207.5 154.0 207.8C165.0 208.3 174.5 206.8 187.8 202.5C208.2 195.8 224.7 195.7 242.8 202.2C264.2 210.0 282.0 228.2 289.6 250.5C292.0 257.4 292.5 260.4 292.8 272.6C293.1 284.8 292.9 287.9 291.0 294.6C281.5 329.6 250.6 353.3 215.2 352.9C210.4 352.8 204.0 352.2 201.0 351.6Z",fill:Gl,fillRule:"evenodd"})]}),m={navy:"#0e2249",navyD:"#07142e",blue:"#2569b8",sky:"#9DB8DE",paper:"#eef2f7",card:"#ffffff",ink:"#1a2740",mute:"#5a6b82",gold:"#f5b716",goldD:"#8a5a00",line:"#e2e8f0",good:"#157a43",goodBg:"#E4F4EC",warn:"#8a5a00",warnBg:"#FDF4E0",clay:"#a63a20",clayBg:"#FBEAE5",olive:"#3f4c37",oliveLt:"#EDEFE9",brand:"#1f5d99",brandD:"#163f66",tg:"#1373a2"},gd=`linear-gradient(160deg, ${m.brand}, ${m.brandD})`,Pt={name:"Rey Aquino",team:"Bravo",card:"0240 5578 9012 3456"},Ql={name:"Team Bravo",url:"https://t.me/",members:24},pd={bronze:{lo:"#8C5A2B",mid:"#B87A3D",hi:"#E2A96A",ink:"#3A2410"},silver:{lo:"#7E8A9C",mid:"#B9C4D2",hi:"#EDF1F6",ink:"#0e2249"},gold:{lo:"#B07E0A",mid:"#f5b716",hi:"#FFD968",ink:"#3A2A00"}},Nn={BASE:{kind:"seal",n:0,metal:"bronze"},TL:{kind:"bars",n:1,metal:"silver"},SL:{kind:"bars",n:2,metal:"silver"},PL:{kind:"bars",n:3,metal:"silver"},CC:{kind:"field",n:1,metal:"gold"}},Tt=[{k:"BASE",n:"BASE",full:"Base Activation",phase:"Member",eyebrow:"Activation",pin:"activated",opens:"My Team opens.",abbr:null,ref:"GA-BASE-0847",cite:"As an activated member of the Gutguard Lifestyle, having completed Admin and Compliance and all five activation events.",reqs:[{id:"b-orient",type:"document",title:"Gutguard Dashboard Orientation",mins:"4 min",blurb:"Where everything lives \u2014 content, sales, your team.",blurbTl:"Dito nakalagay ang lahat \u2014 content, sales, at ang team mo."},{id:"b-da",type:"document",title:"Distributor's Agreement",mins:"6 min",doc:"Agreement v3.1",docTl:"Kasunduan ng Distributor v3.1",blurb:"What you're agreeing to, in plain terms.",blurbTl:"Ang pinapasukan mo, sa simpleng salita.",body:"This Agreement is between Gutguard Philippines Inc. and you as an independent distributor. You are not an employee. You earn from product sold, never from recruitment alone. You may not make medical claims about any product. You may not require anyone below you to purchase stock. Either party may end this Agreement in writing at any time. Your card number and downline records remain the property of the company.",bodyTl:"Ang kasunduang ito ay sa pagitan ng Gutguard Philippines Inc. at ikaw bilang isang independent distributor. Hindi ka empleyado. Kumikita ka mula sa produktong nabenta, hindi mula sa pagre-recruit lamang. Bawal kang mag-claim ng anumang medikal na epekto ng produkto. Bawal mong pilitin ang sinumang nasa ilalim mo na bumili ng stock. Maaaring wakasan ninuman sa atin ang kasunduang ito sa pamamagitan ng sulat, anumang oras. Ang card number mo at ang talaan ng iyong downline ay pag-aari ng kompanya."},{id:"b-eth",type:"document",title:"Code of Ethics",mins:"5 min",doc:"Code v2.0",docTl:"Kodigo ng Etika v2.0",blurb:"How we speak about the product, and about each other.",blurbTl:"Kung paano tayo magsalita tungkol sa produkto, at sa isa't isa.",body:"Speak only to what the product is: food, taken daily. Never promise a cure, never diagnose, never discourage anyone from seeing a doctor. Show real testimonies with the person's consent and never edit them into a claim. Do not poach another distributor's prospect. Do not sell below the posted price. Do not present income as guaranteed, and never show earnings without showing the work behind them.",bodyTl:"Sabihin lamang kung ano talaga ang produkto: pagkain, iniinom araw-araw. Huwag mangakong may lunas, huwag mag-diagnose, at huwag pigilan ang sinuman na magpatingin sa doktor. Ipakita lamang ang totoong testimonya nang may pahintulot, at huwag itong baguhin para maging claim. Huwag agawin ang prospect ng ibang distributor. Huwag magbenta nang mas mababa sa nakatakdang presyo. Huwag sabihing garantisado ang kita."},{id:"b-creed",type:"document",title:"Gentrep Creed",mins:"2 min",doc:"The Creed",docTl:"Ang Gentrep Creed",blurb:"What we hold ourselves to.",blurbTl:"Ang pinanghahawakan natin sa sarili.",body:"I earn, I do not extract. I bring people in only when I would want to be brought in the same way. I tell the truth about the product, the money, and the work. I do not leave someone I signed up to figure it out alone. What I build should still stand if I stop building it.",bodyTl:"Kumikita ako, hindi ako nangungurakot. Isinasama ko lang ang tao kung paano ko rin gustong isama ako. Sinasabi ko ang totoo tungkol sa produkto, sa pera, at sa trabaho. Hindi ko iiwan ang taong isinama ko. Ang itinatayo ko ay dapat tumayo pa rin kahit tumigil na ako."},{id:"b-1",type:"attendance",title:"Ginhawa Talk",note:"Where it starts"},{id:"b-2",type:"attendance",title:"Product Presentation",note:"What it is, how to use it"},{id:"b-3",type:"attendance",title:"Testimonial Session",note:"Real members, real results"},{id:"b-4",type:"attendance",title:"Business Orientation",note:"How earning actually works"},{id:"b-5",type:"attendance",title:"Leaders' Training",note:"Running your own table"}]},{k:"TL",n:"TL",full:"Team Leader",phase:"Lead Generator",eyebrow:"Rank certification",pin:"pinned Team Leader",opens:"You'll be invited to a Recognition Night.",abbr:"2Lt",officer:"Academy Second Lieutenant",ref:"GA-TL-0847",cite:"As an official member of the Gutguard Corps of Officers, having passed all training requirements of the Team Leader course and demonstrated them in the field.",reqs:[{id:"t-1",type:"attendance",title:"Your First Twenty Names",note:"Where leads actually come from"},{id:"t-2",type:"attendance",title:"The Invite Conversation",note:"Asking without pressure"},{id:"t-3",type:"attendance",title:"Following Up",note:"Staying in touch, not chasing"},{id:"t-4",type:"attendance",title:"Handling a Guest",note:"From the door to the seat"},{id:"t-5",type:"attendance",title:"What You May Not Say",note:"Claims, income, and the line"},{id:"t-demo",type:"demonstration",title:"Bring three guests",note:"They check in, with a Platoon Leader in the room"}]},{k:"SL",n:"SL",full:"Squad Leader",phase:"Presenter",eyebrow:"Rank certification",pin:"pinned Squad Leader",opens:"You'll be invited to a Recognition Night.",abbr:"1Lt",officer:"Academy First Lieutenant",ref:"GA-SL-0847",cite:"As an official member of the Gutguard Corps of Officers, having passed all training requirements of the Squad Leader course and presented before a room.",reqs:[{id:"s-1",type:"attendance",title:"Opening a Room",note:"The first four minutes"},{id:"s-2",type:"attendance",title:"The Product Story",note:"What it is, without claims"},{id:"s-3",type:"attendance",title:"Handling Questions",note:"Including the hard ones"},{id:"s-4",type:"attendance",title:"Closing the Session",note:"Asking, and letting people choose"},{id:"s-demo",type:"demonstration",title:"Present a full session",note:"With a Platoon Leader watching"}]},{k:"PL",n:"PL",full:"Platoon Leader",phase:"Trains Team Leaders",eyebrow:"Rank certification",pin:"pinned Platoon Leader",opens:"You'll be invited to a Recognition Night.",abbr:"Capt",officer:"Academy Captain",ref:"GA-PL-0847",cite:"As an official member of the Gutguard Corps of Officers, having passed all training requirements of the Platoon Leader course and trained a Team Leader through to certification.",reqs:[{id:"p-1",type:"attendance",title:"Teaching, Not Telling",note:"How adults actually learn"},{id:"p-2",type:"attendance",title:"Running a Class",note:"Structure, pace, and the room"},{id:"p-3",type:"attendance",title:"Signing Someone Off",note:"What you are vouching for"},{id:"p-der",type:"derived",title:"A Team Leader you trained is certified",note:"Their certificate, not your word"}]},{k:"CC",n:"CC",full:"Company Commander",phase:"Trains Squad Leaders",eyebrow:"Rank certification",pin:"pinned Company Commander",opens:"You'll be invited to a Recognition Night.",abbr:"Maj",officer:"Academy Major",ref:"GA-CC-0847",cite:"As an official member of the Gutguard Corps of Officers, having passed all training requirements of the Company Commander course and trained a Squad Leader through to certification.",reqs:[{id:"c-1",type:"attendance",title:"Building a Bench",note:"Depth, not headcount"},{id:"c-2",type:"attendance",title:"Standards and Drift",note:"Keeping the teaching true"},{id:"c-der",type:"derived",title:"A Squad Leader you trained is certified",note:"Their certificate, not your word"}]}],md={document:"Watch and agree",attendance:"Attend",demonstration:"Show it",derived:"Earned by your trainee"},hd=[{id:11,type:"Testimonial Session",date:"Sat 2 Aug",time:"2:00 PM",place:"Robinsons, Davao",host:"Jesh M.",rank:"CC",seats:4},{id:12,type:"Product Presentation",date:"Sat 2 Aug",time:"4:00 PM",place:"Lagao Hall",host:"Ana R.",rank:"PL",seats:15},{id:13,type:"Business Orientation",date:"Sun 3 Aug",time:"3:00 PM",place:"Koronadal",host:"Rey T.",rank:"PL",seats:22},{id:14,type:"Testimonial Session",date:"Sat 9 Aug",time:"2:00 PM",place:"Lagao Hall",host:"Ana R.",rank:"PL",seats:0},{id:15,type:"Ginhawa Talk",date:"Sat 9 Aug",time:"9:00 AM",place:"Polomolok",host:"Ana R.",rank:"PL",seats:30},{id:16,type:"Business Orientation",date:"Sat 16 Aug",time:"4:00 PM",place:"Lagao Hall",host:"Ana R.",rank:"PL",seats:9},{id:17,type:"Leaders' Training",date:"Sat 16 Aug",time:"1:00 PM",place:"Robinsons, Davao",host:"Rey T.",rank:"PL",seats:8},{id:18,type:"Ginhawa Talk",date:"Sat 23 Aug",time:"9:00 AM",place:"Koronadal",host:"Jesh M.",rank:"CC",seats:20},{id:19,type:"Leaders' Training",date:"Sat 30 Aug",time:"1:00 PM",place:"Lagao Hall",host:"Ana R.",rank:"PL",seats:10},{id:21,type:"Your First Twenty Names",date:"Sat 2 Aug",time:"1:00 PM",place:"Koronadal",host:"Ana R.",rank:"PL",seats:8},{id:22,type:"The Invite Conversation",date:"Sat 9 Aug",time:"2:00 PM",place:"Polomolok",host:"Jesh M.",rank:"CC",seats:25},{id:23,type:"Following Up",date:"Sat 16 Aug",time:"1:00 PM",place:"Lagao Hall",host:"Rey T.",rank:"PL",seats:16},{id:24,type:"Handling a Guest",date:"Sat 23 Aug",time:"10:00 AM",place:"Koronadal",host:"Ana R.",rank:"PL",seats:12},{id:25,type:"What You May Not Say",date:"Sat 30 Aug",time:"9:00 AM",place:"Lagao Hall",host:"Jesh M.",rank:"CC",seats:30},{id:31,type:"Opening a Room",date:"Sat 6 Sep",time:"1:00 PM",place:"Lagao Hall",host:"Jesh M.",rank:"CC",seats:14},{id:32,type:"The Product Story",date:"Sat 13 Sep",time:"1:00 PM",place:"Koronadal",host:"Rey T.",rank:"PL",seats:18}];function va(){let[e,t]=(0,G.useState)("BASE"),[n,r]=(0,G.useState)({"b-orient":{s:"done",when:"28 Jul"},"b-da":{s:"done",when:"28 Jul",lang:"en"},"b-eth":{s:"done",when:"28 Jul",lang:"tl"},"b-creed":{s:"open"},"b-1":{s:"done",when:"19 Jul"},"b-2":{s:"missed",when:"26 Jul"},"b-3":{s:"booked",ev:11},"b-4":{s:"open"},"b-5":{s:"open"}}),[l,o]=(0,G.useState)(null),[i,a]=(0,G.useState)(null),[s,d]=(0,G.useState)({}),[g,v]=(0,G.useState)("en"),[y,w]=(0,G.useState)(null),[S,C]=(0,G.useState)(!1),[W,f]=(0,G.useState)(!1),[c,p]=(0,G.useState)(""),[x,E]=(0,G.useState)(""),[P,_]=(0,G.useState)(0),T=(0,G.useRef)({}),$=h=>{p(h),E(h),setTimeout(()=>p(""),2400)},L=Tt.find(h=>h.k===e),Y=L.reqs,Ke=h=>n[h]||{s:"open"},wa=h=>h.reqs.filter(R=>Ke(R.id).s==="done").length,Kl=h=>h.reqs.length>0&&wa(h)===h.reqs.length,_n=wa(L),Ye=Y.length,Ca=Y.filter(h=>Ke(h.id).s==="booked").length,Sa=Y.filter(h=>Ke(h.id).s==="missed").length,Rt=Kl(L),xe=Y.find(h=>["open","missed"].includes(Ke(h.id).s)),kd=h=>hd.find(R=>R.id===h),Ea=h=>{let R=Tt.indexOf(h);if(R<=0)return null;let z=Tt[R-1];return Kl(z)?null:"Finish "+z.full+" first"},xd=(h,R)=>{let z={...n,[h]:R};if(r(z),R.s==="done"){let ne=Y.every(Ze=>(z[Ze.id]||{}).s==="done");_(Date.now()),ne?(E("All requirements complete. Certificate ready."),setTimeout(()=>C(!0),420)):$("Recorded \xB7 "+Y.filter(Ze=>(z[Ze.id]||{}).s==="done").length+" of "+Ye)}},wd=(h,R)=>{r({...n,[h.id]:{s:"booked",ev:R.id}}),w(null),$("Seat reserved \xB7 "+R.date)},Cd=h=>{r({...n,[h.id]:{s:"open"}}),w(null),$("Seat released")},Sd=()=>{$("Opening "+Ql.name+" on Telegram\u2026");try{window.open(Ql.url,"_blank")}catch{}},Na=()=>{if(xe){if(xe.type==="document")return a(xe.id);o(xe.id),setTimeout(()=>T.current[xe.id]?.scrollIntoView({behavior:"smooth",block:"center"}),60)}},Ed=h=>{let R=Tt.find(ne=>ne.k===h),z={...n};R.reqs.forEach(ne=>{ne.type==="document"?z[ne.id]={s:"done",when:"28 Jul",lang:"en"}:ne.type==="attendance"?z[ne.id]={s:"done",when:"16 Aug",via:"scan"}:ne.type==="demonstration"?z[ne.id]={s:"done",when:"23 Aug",via:"signoff",by:"Rey T."}:z[ne.id]={s:"done",when:"30 Aug",via:"derived",trainee:"Marilou D."}}),r(z),t(h),o(null),_(Date.now()),E(R.full+" complete. Certificate ready."),setTimeout(()=>C(!0),420)},O=Y.find(h=>h.id===i);return(0,u.jsxs)("div",{className:"ga",lang:"en",children:[(0,u.jsx)(f1,{}),(0,u.jsx)(d1,{fire:P}),(0,u.jsx)("span",{className:"sr-only",role:"status","aria-live":"polite",children:x}),(0,u.jsx)("a",{className:"skip",href:"#reqs",children:"Skip to what it takes"}),(0,u.jsxs)("div",{className:"shell",children:[(0,u.jsxs)("aside",{className:"side","aria-label":"Academy navigation",children:[(0,u.jsxs)("div",{className:"brand",children:[(0,u.jsx)(Cr,{height:24,color:m.navy}),(0,u.jsx)("span",{className:"serif",children:"Academy"})]}),(0,u.jsxs)("div",{className:"who",children:[(0,u.jsx)("span",{className:"avatar",children:Pt.name.split(" ").map(h=>h[0]).join("").slice(0,2)}),(0,u.jsxs)("span",{children:[(0,u.jsx)("b",{children:Pt.name}),(0,u.jsxs)("em",{children:["Team ",Pt.team]})]})]}),(0,u.jsx)("nav",{"aria-label":"Ranks",className:"side-nav",children:Tt.map(h=>{let R=Ea(h),z=h.k===e;return(0,u.jsxs)("button",{className:"tap side-rank"+(z?" on":""),"aria-current":z?"page":void 0,onClick:()=>R?$(R):(t(h.k),o(null)),children:[(0,u.jsx)(Ln,{...Nn[h.k],size:h.k==="CC"?20:h.k==="BASE"?22:13,mark:!1}),(0,u.jsxs)("span",{className:"grow",children:[(0,u.jsx)("b",{children:h.full}),(0,u.jsx)("em",{children:h.phase})]}),R&&(0,u.jsx)("span",{className:"lock",children:"Locked"}),Kl(h)&&(0,u.jsx)("span",{className:"tickmini",children:"\u2713"})]},h.k)})}),(0,u.jsx)("button",{className:"tap side-btn",onClick:()=>f(!0),children:"About Gentrep Academy"}),!Rt&&xe&&(0,u.jsxs)("div",{className:"side-next",children:[(0,u.jsx)("div",{className:"eyebrow-dark",children:"Do this next"}),(0,u.jsx)("b",{children:xe.title}),(0,u.jsx)("button",{className:"tap btn primary wide",onClick:Na,children:xe.type==="document"?"Watch the video":"Pick a date"})]})]}),(0,u.jsxs)("main",{className:"col",children:[(0,u.jsxs)("header",{className:"mast only-mobile",children:[(0,u.jsxs)("div",{className:"brand",children:[(0,u.jsx)(Cr,{height:26,color:m.navy}),(0,u.jsx)("span",{className:"serif big",children:"Academy"})]}),(0,u.jsx)("button",{className:"tap pill sm",onClick:()=>f(!0),children:"About"})]}),(0,u.jsxs)("p",{className:"sub only-mobile",children:[Pt.name," \xB7 Team ",Pt.team]}),(0,u.jsx)("nav",{className:"ladder noscroll only-mobile","aria-label":"Ranks",children:Tt.map(h=>{let R=Ea(h),z=h.k===e;return(0,u.jsxs)("button",{className:"tap rung"+(z?" on":""),"aria-current":z?"page":void 0,onClick:()=>R?$(R):(t(h.k),o(null)),children:[(0,u.jsx)(Ln,{...Nn[h.k],size:h.k==="CC"?17:h.k==="BASE"?18:11,mark:!1}),(0,u.jsx)("span",{className:"ant",children:h.n}),(0,u.jsxs)("span",{className:"sr-only",children:[h.full,", ",h.phase,R?", locked. "+R:""]}),R&&(0,u.jsx)("span",{className:"lock",children:"Locked"})]},h.k)})}),(0,u.jsxs)("section",{className:"plate hatch"+(Rt?" done":""),children:[(0,u.jsx)(Cr,{markOnly:!0,height:210,"aria-hidden":"true",className:"plate-mark",style:{position:"absolute",top:"50%",left:"72%",transform:"translateY(-50%)",opacity:.16,zIndex:-1,pointerEvents:"none",maxWidth:"none"}}),(0,u.jsxs)("div",{className:"rule-row",children:[(0,u.jsx)("i",{}),(0,u.jsx)("span",{children:L.eyebrow})]}),(0,u.jsx)("h1",{className:"ant plate-title",children:L.full}),(0,u.jsxs)("div",{className:"plate-sub",children:[L.phase,L.abbr?" \xB7 "+L.abbr:""]}),(0,u.jsxs)("div",{className:"plate-foot",children:[(0,u.jsx)("b",{children:Rt?"All done.":_n+" of "+Ye+" done"}),(0,u.jsx)("span",{className:"pips",children:Y.map(h=>(0,u.jsx)("i",{className:"pip "+Ke(h.id).s},h.id))})]}),(0,u.jsx)("div",{className:"bar",role:"progressbar","aria-valuenow":_n,"aria-valuemin":0,"aria-valuemax":Ye,"aria-label":L.full+" progress","aria-valuetext":_n+" of "+Ye+" complete",children:(0,u.jsx)("i",{style:{width:(Ye?_n/Ye*100:0)+"%"}})}),(0,u.jsx)("div",{className:"plate-note",children:[Ca?Ca+" booked":null,Sa?Sa+" missed":null].filter(Boolean).join(" \xB7 ")||"\xA0"})]}),(0,u.jsxs)("button",{className:"tap chat",onClick:Sd,children:[(0,u.jsx)("span",{className:"tg",children:(0,u.jsx)(c1,{})}),(0,u.jsxs)("span",{className:"grow left",children:[(0,u.jsxs)("b",{children:[Ql.name," chat"]}),(0,u.jsxs)("em",{children:[Ql.members," members \xB7 ask before you go"]})]})]}),(0,u.jsx)("div",{className:"bar-title",children:(0,u.jsx)("h2",{className:"sec",id:"reqs",tabIndex:-1,children:"What it takes"})}),(0,u.jsxs)("p",{className:"sr-only",children:[_n," of ",Ye," requirements complete."]}),(0,u.jsx)("ol",{className:"reqs",children:Y.map((h,R)=>{let z=Ke(h.id),ne=l===h.id,Ze=hd.filter(Z=>Z.type===h.title),La=z.ev?kd(z.ev):null,Yl=xe&&xe.id===h.id,Nd=R>0&&Ke(Y[R-1].id).s==="done",Ld=z.s==="done"?m.good:z.s==="booked"?m.warn:z.s==="missed"?m.clay:m.mute,_a=z.s==="done"?h.type==="document"?"Agreed"+(z.lang==="tl"?" sa Tagalog":"")+" \xB7 "+z.when:z.via==="signoff"?"Signed off \xB7 "+z.by:z.via==="derived"?z.trainee+" certified":"Attended \xB7 "+z.when:z.s==="booked"?"Booked \xB7 "+La.date+", "+La.place:z.s==="missed"?"Missed \xB7 "+z.when+" \u2014 pick another date":h.type==="attendance"?Ze.length?Ze.length+" dates posted":"No dates posted yet":h.type==="document"?"Video "+h.mins+(h.doc?" \xB7 then read and agree":""):h.note;return(0,u.jsxs)("li",{className:"req",children:[(0,u.jsxs)("div",{className:"spine","aria-hidden":"true",children:[(0,u.jsx)("span",{className:"rail",style:{background:Nd&&z.s==="done"?m.gold:m.line,top:R===0?30:0,bottom:R===Y.length-1?"calc(100% - 30px)":-10}}),(0,u.jsx)("span",{className:"node "+z.s,children:z.s==="done"?"\u2713":z.s==="missed"?"!":""})]}),(0,u.jsxs)("article",{ref:Z=>T.current[h.id]=Z,className:"req-card"+(z.s==="missed"?" missed":ne||Yl?" active":""),children:[(0,u.jsxs)("div",{className:"req-head",children:[(0,u.jsx)("div",{className:"req-type",style:{color:Yl?m.blue:m.mute},children:Yl?"Do this next \xB7 "+md[h.type]:md[h.type]}),(0,u.jsxs)("h3",{children:[h.title,(0,u.jsxs)("span",{className:"sr-only",children:[". Requirement ",R+1," of ",Ye,". ",_a]})]}),(0,u.jsx)("p",{style:{color:Ld,fontWeight:z.s==="open"?400:600},children:_a})]}),h.type==="document"&&z.s!=="done"&&(0,u.jsx)("div",{className:"req-act",children:(0,u.jsx)("button",{className:"tap btn primary wide flat",onClick:()=>a(h.id),children:"Watch the video"})}),h.type==="attendance"&&z.s!=="done"&&(0,u.jsx)("div",{className:"req-act",children:(0,u.jsx)("button",{className:"tap btn primary wide flat","aria-expanded":ne,"aria-controls":"d-"+h.id,onClick:()=>o(ne?null:h.id),style:z.s==="booked"?{background:"#fff",border:`1.5px solid ${m.line}`,color:m.navy}:void 0,children:ne?"Hide dates":z.s==="booked"?"Change date":z.s==="missed"?"Pick another date":"See "+Ze.length+" dates"})}),ne&&(0,u.jsxs)("div",{className:"dates fade",id:"d-"+h.id,role:"group","aria-label":"Dates for "+h.title,children:[Ze.length===0&&(0,u.jsx)("p",{className:"fine pad",children:"GEMA hasn't posted a date for this yet. You'll be told when one appears."}),Ze.map(Z=>{let za=z.ev===Z.id,Gt=Z.seats===0,[_d,zd,Pd]=Z.date.split(" ");return(0,u.jsxs)("div",{className:"ev"+(za?" mine":""),children:[(0,u.jsxs)("div",{className:"datebox",children:[(0,u.jsx)("em",{children:_d}),(0,u.jsx)("b",{children:zd}),(0,u.jsx)("em",{children:Pd})]}),(0,u.jsxs)("div",{className:"grow",children:[(0,u.jsx)("div",{className:"ev-place",children:Z.place}),(0,u.jsxs)("div",{className:"ev-meta",children:[Z.time," \xB7 ",(0,u.jsx)(Ln,{...Nn[Z.rank],size:Z.rank==="CC"?12:8,mark:!1})," ",Z.host]}),(0,u.jsx)("div",{className:"ev-seats",style:{color:Gt?m.clay:Z.seats<=5?m.warn:m.mute},children:Gt?"Full \u2014 join the waitlist":Z.seats+" seats left"})]}),za?y===Z.id?(0,u.jsxs)("div",{className:"confirm",children:[(0,u.jsx)("button",{className:"tap btn danger sm",onClick:()=>Cd(h),children:"Give it up"}),(0,u.jsx)("button",{className:"tap btn navy sm",onClick:()=>w(null),children:"Keep"})]}):(0,u.jsx)("button",{className:"tap btn booked sm",onClick:()=>w(Z.id),children:"Booked \xB7 cancel"}):(0,u.jsx)("button",{className:"tap btn sm ev-act","aria-label":(Gt?"Join waitlist for ":"Reserve seat for ")+h.title+", "+Z.date+", "+Z.place,onClick:()=>Gt?$("Added to the waitlist"):wd(h,Z),style:Gt?{background:"#fff",border:`1.5px solid ${m.line}`,color:m.navy}:{background:m.blue,color:"#fff"},children:Gt?"Waitlist":z.s==="booked"?"Switch":"Reserve"})]},Z.id)})]}),h.type==="demonstration"&&z.s!=="done"&&(0,u.jsx)("div",{className:"req-act",children:(0,u.jsx)("p",{className:"fine",children:"Your upline records this on the day. Nothing to do here."})}),h.type==="derived"&&z.s!=="done"&&(0,u.jsx)("div",{className:"req-act",children:(0,u.jsx)("p",{className:"fine",children:"This completes when they certify. Their certificate, not your word."})})]})]},h.id)})}),(0,u.jsx)("div",{className:"bar-title",children:(0,u.jsx)("span",{className:"sec",children:"Then"})}),(0,u.jsxs)("div",{className:"outcome"+(Rt?" done":""),children:[(0,u.jsx)(Ln,{...Nn[L.k],size:L.k==="CC"?26:L.k==="BASE"?28:17}),(0,u.jsx)("p",{children:Rt?"Done \u2014 "+L.opens:"Finish all "+Ye+" and you're "+L.pin+". "+L.opens})]}),Rt&&(0,u.jsx)("button",{className:"tap btn navy wide",onClick:()=>C(!0),children:"See my certificate"}),(0,u.jsxs)("div",{className:"demo no-print",children:[(0,u.jsx)("div",{className:"demo-label",children:"Demo \xB7 walk the ladder"}),(0,u.jsx)("p",{className:"demo-note",children:"Completes a rank the way it would really be earned \u2014 documents agreed, events scanned, demonstrations signed off, derived ones by a trainee's certificate \u2014 then issues the certificate."}),(0,u.jsx)("div",{className:"demo-row",children:Tt.map(h=>(0,u.jsxs)("button",{className:"tap demo-btn",onClick:()=>Ed(h.k),children:["Complete ",h.n]},h.k))}),(0,u.jsxs)("div",{className:"demo-row",children:[(0,u.jsxs)("button",{className:"tap demo-btn",onClick:()=>C(!0),children:["Certificate for ",L.n]}),(0,u.jsx)("button",{className:"tap demo-btn",onClick:()=>{r({}),t("BASE"),E("Reset")},children:"Reset all"})]})]})]})]}),!Rt&&xe&&(0,u.jsx)("div",{className:"foot only-mobile",children:(0,u.jsxs)("div",{className:"foot-in",children:[(0,u.jsxs)("div",{className:"grow",children:[(0,u.jsx)("div",{className:"eyebrow-dark",children:"Next"}),(0,u.jsx)("b",{className:"foot-title",children:xe.title})]}),(0,u.jsx)("button",{className:"tap btn primary",onClick:Na,children:xe.type==="document"?"Watch":"Pick a date"})]})}),O&&(0,u.jsxs)(ya,{label:O.title,onClose:()=>a(null),children:[(0,u.jsxs)("div",{className:"sheet-head",children:[(0,u.jsxs)("div",{children:[(0,u.jsx)("h2",{className:"h2",children:O.title}),(0,u.jsx)("p",{className:"fine",children:g==="tl"&&O.blurbTl?O.blurbTl:O.blurb})]}),(0,u.jsx)("button",{className:"tap pill",onClick:()=>a(null),"aria-label":"Close",children:"Close"})]}),(0,u.jsx)("div",{className:"langs",role:"group","aria-label":"Language",children:[["en","English"],["tl","Tagalog"]].map(([h,R])=>(0,u.jsx)("button",{className:"tap lang"+(g===h?" on":""),onClick:()=>v(h),"aria-pressed":g===h,children:R},h))}),(0,u.jsx)("div",{className:"video tap",role:"button",tabIndex:0,"aria-pressed":!!s[O.id],onClick:()=>d({...s,[O.id]:!0}),onKeyDown:h=>{(h.key==="Enter"||h.key===" ")&&(h.preventDefault(),d({...s,[O.id]:!0}))},style:{background:s[O.id]?m.goodBg:gd},children:(0,u.jsxs)("div",{children:[(0,u.jsx)("span",{className:"play",style:{background:s[O.id]?m.good:"rgba(255,255,255,.25)"},children:s[O.id]?"\u2713":"\u25B6"}),(0,u.jsx)("em",{style:{color:s[O.id]?m.good:"#fff"},children:s[O.id]?g==="tl"?"Napanood na":"Watched":(g==="tl"?"I-play \xB7 ":"Play \xB7 ")+O.mins})]})}),O.doc&&(0,u.jsxs)(u.Fragment,{children:[(0,u.jsx)("div",{className:"eyebrow-dark mt",children:g==="tl"&&O.docTl?O.docTl:O.doc}),(0,u.jsx)("div",{className:"doc",lang:g,style:{opacity:s[O.id]?1:.5},children:g==="tl"&&O.bodyTl?O.bodyTl:O.body}),!s[O.id]&&(0,u.jsx)("p",{className:"fine",children:g==="tl"?"Panoorin muna ang video.":"Watch the video first."})]}),(0,u.jsx)("button",{className:"tap btn primary wide",disabled:!s[O.id],onClick:()=>{a(null),xd(O.id,{s:"done",when:"28 Jul",lang:g})},children:O.doc?g==="tl"?"Nabasa ko ito at sumasang-ayon ako":"I have read this and I agree":g==="tl"?"Tapos \u2014 napanood ko na":"Done \u2014 I've watched it"}),O.doc&&(0,u.jsx)("p",{className:"fine center",children:g==="tl"?"Ang pangalan mo, ang petsa, ang bersyon, at kung anong wika mo ito binasa ay nakatala.":"Your name, the date, the version, and the language you read it in are kept on file."})]}),S&&(0,u.jsxs)(ya,{label:"Certificate",onClose:()=>C(!1),children:[(0,u.jsx)("div",{className:"printroot",children:(0,u.jsxs)("div",{className:"cert",children:[(0,u.jsx)(Cr,{markOnly:!0,height:260,"aria-hidden":"true",className:"cert-mark",style:{position:"absolute",top:"50%",left:"50%",transform:"translate(-50%,-50%)",opacity:.05,zIndex:-1,pointerEvents:"none",maxWidth:"none"}}),(0,u.jsxs)("div",{className:"cert-brand",children:[(0,u.jsx)(Cr,{height:20,color:m.navy}),(0,u.jsx)("span",{className:"serif",children:"Academy"})]}),(0,u.jsx)("div",{className:"cert-eyebrow",children:"Certification"}),(0,u.jsx)("div",{className:"cert-ins",children:(0,u.jsx)(Ln,{...Nn[L.k],size:L.k==="CC"?50:L.k==="BASE"?52:42})}),(0,u.jsxs)("div",{className:"cert-name",children:[L.abbr?L.abbr+" ":"",Pt.name]}),(0,u.jsx)("div",{className:"cert-rank",children:L.officer?L.officer+" \xB7 "+L.full:"Activated Member"}),(0,u.jsx)("div",{className:"cert-hr"}),(0,u.jsx)("p",{className:"cert-cite",children:L.cite}),(0,u.jsx)("div",{className:"cert-evidence",children:(()=>{let h={};L.reqs.forEach(z=>{h[z.type]=(h[z.type]||0)+1});let R=[];return h.document&&R.push(h.document+" agreed"),h.attendance&&R.push(h.attendance+" attended"),h.demonstration&&R.push("1 demonstration witnessed"),h.derived&&R.push("1 trainee certified"),R.join(" \xB7 ")})()}),(0,u.jsx)("div",{className:"cert-sigs",children:["Academy Commandant","Chief Operating Officer"].map(h=>(0,u.jsxs)("div",{children:[(0,u.jsx)("span",{}),(0,u.jsx)("em",{children:h})]},h))}),(0,u.jsxs)("div",{className:"cert-qr",children:[(0,u.jsx)(u1,{seed:L.ref}),(0,u.jsx)("em",{children:"Scan to verify"})]}),(0,u.jsxs)("div",{className:"cert-record",children:[(0,u.jsxs)("div",{children:[(0,u.jsx)("em",{children:"Dated"}),(0,u.jsx)("b",{children:"28 July 2026"})]}),(0,u.jsxs)("div",{children:[(0,u.jsx)("em",{children:"Card"}),(0,u.jsx)("b",{children:Pt.card.slice(-9)})]}),(0,u.jsxs)("div",{children:[(0,u.jsx)("em",{children:"Reference"}),(0,u.jsx)("b",{children:L.ref})]})]}),(0,u.jsx)("p",{className:"cert-fine",children:"An internal distinction of the Gentrep Academy."})]})}),(0,u.jsxs)("div",{className:"no-print",children:[(0,u.jsx)("button",{className:"tap btn navy wide",onClick:()=>{E("Opening the print dialog. Choose Save as PDF."),window.print()},children:"Download as PDF"}),(0,u.jsxs)("p",{className:"fine center",children:["In the print window choose ",(0,u.jsx)("b",{children:"Save as PDF"})," as the destination."]}),(0,u.jsx)("button",{className:"tap btn tg wide",onClick:async()=>{let h=(L.abbr?L.abbr+" ":"")+Pt.name+" \u2014 "+(L.officer||"Activated Member")+", Gentrep Academy.",R="https://ggverse.ph/v/"+L.ref;try{if(navigator.share){await navigator.share({title:"Gentrep Academy",text:h,url:R});return}}catch(z){if(z?.name==="AbortError")return}try{await navigator.clipboard.writeText(h+" "+R),$("Copied \u2014 paste it anywhere")}catch{$(R)}},children:"Share"}),(0,u.jsx)("button",{className:"tap btn outline wide",onClick:()=>C(!1),children:"Close"})]})]}),W&&(0,u.jsxs)(ya,{label:"About Gentrep Academy",onClose:()=>f(!1),children:[(0,u.jsxs)("div",{className:"sheet-head",children:[(0,u.jsxs)("div",{children:[(0,u.jsx)("h2",{className:"ant h1",children:"About Gentrep Academy"}),(0,u.jsx)("p",{className:"fine",children:"Read this once. About five minutes."})]}),(0,u.jsx)("button",{className:"tap pill",onClick:()=>f(!1),"aria-label":"Close",children:"Close"})]}),(0,u.jsx)("p",{className:"lead",children:"The Academy is where you learn this business, one level at a time. Every level is a short course: sessions you attend in person, and a scan at the door that records you were there. You never tick your own boxes \u2014 that is what makes them worth something."}),(0,u.jsx)("h3",{className:"sec mt",children:"The five levels"}),Tt.map(h=>(0,u.jsxs)("div",{className:"about-lvl",children:[(0,u.jsx)(Ln,{...Nn[h.k],size:h.k==="CC"?22:h.k==="BASE"?24:14,mark:!1}),(0,u.jsxs)("div",{children:[(0,u.jsx)("b",{children:h.full}),(0,u.jsx)("em",{children:h.phase})]})]},h.k)),(0,u.jsx)("h3",{className:"sec mt",children:"How a course is proven"}),(0,u.jsx)("div",{className:"about-table",children:[["Watch and agree","You agree in the app; the record is kept"],["Attend","The scan at the door"],["Show it","An upline watches and signs it off"],["Earned by your trainee","Their certificate, not your word"]].map(([h,R])=>(0,u.jsxs)("div",{children:[(0,u.jsx)("b",{children:h}),(0,u.jsx)("span",{children:R})]},h))}),(0,u.jsx)("h3",{className:"sec mt",children:"If something changes"}),(0,u.jsx)("div",{className:"about-table",children:[["Cannot make it?","Open the date and cancel. The seat goes back to someone else."],["Want a different date?","Tap Switch. No need to cancel first."],["Session full?","Join the waitlist and you'll be told when a seat opens."],["Missed one?","Pick another date. Nothing else you've done is lost."],["No dates posted?","That one is waiting on us, not on you."],["Is there a deadline?","No. Most finish a level in about three weeks."]].map(([h,R])=>(0,u.jsxs)("div",{children:[(0,u.jsx)("b",{children:h}),(0,u.jsx)("span",{children:R})]},h))}),(0,u.jsxs)("div",{className:"closing",children:["The app only keeps the record. What you actually learn happens in the room \u2014 from the people, the stories and the questions you ask there. ",(0,u.jsx)("b",{children:"See you Saturday."})]}),(0,u.jsx)("button",{className:"tap btn navy wide",onClick:()=>f(!1),children:"Got it"})]}),c&&(0,u.jsx)("div",{className:"fade toast",children:c})]})}var ka=({cx:e,cy:t,s:n})=>(0,u.jsxs)("g",{fill:Gl,stroke:Gl,strokeWidth:n*.15,strokeLinecap:"round",strokeLinejoin:"round",children:[(0,u.jsx)("line",{x1:e-n*.42,y1:t+n*.3,x2:e+n*.12,y2:t-n*.46}),(0,u.jsx)("line",{x1:e-n*.42,y1:t+n*.3,x2:e+n*.44,y2:t+n*.28}),(0,u.jsx)("circle",{cx:e+n*.12,cy:t-n*.46,r:n*.19}),(0,u.jsx)("circle",{cx:e-n*.42,cy:t+n*.3,r:n*.25}),(0,u.jsx)("circle",{cx:e+n*.44,cy:t+n*.28,r:n*.33})]}),xa=e=>{let t=pd[e]||pd.silver,n="m-"+e;return{m:t,id:n,defs:(0,u.jsx)("defs",{children:(0,u.jsxs)("linearGradient",{id:n,x1:"0",y1:"0",x2:"0.35",y2:"1",children:[(0,u.jsx)("stop",{offset:"0%",stopColor:t.hi}),(0,u.jsx)("stop",{offset:"42%",stopColor:t.mid}),(0,u.jsx)("stop",{offset:"72%",stopColor:t.lo}),(0,u.jsx)("stop",{offset:"100%",stopColor:t.mid})]})})}},i1=({n:e=1,size:t=40,metal:n="silver",mark:r=!0})=>{let{m:l,id:o,defs:i}=xa(n),a=21,s=9,d=100,g=e*a+(e-1)*s;return(0,u.jsxs)("svg",{width:t*1.7,height:t*1.7*(g/d),viewBox:`0 0 ${d} ${g}`,"aria-hidden":"true",style:{flexShrink:0},children:[i,Array.from({length:e}).map((v,y)=>(0,u.jsxs)("g",{children:[(0,u.jsx)("rect",{x:"1.5",y:y*(a+s)+1.2,width:d-3,height:a-2.4,rx:4,fill:`url(#${o})`,stroke:l.lo,strokeWidth:"2.2"}),(0,u.jsx)("line",{x1:"7",y1:y*(a+s)+a*.34,x2:d-7,y2:y*(a+s)+a*.34,stroke:l.hi,strokeWidth:"1.2",opacity:".55"})]},y)),r&&(0,u.jsx)(ka,{cx:d/2,cy:g/2,s:g*.42})]})},a1=({size:e=46,metal:t="gold",mark:n=!0})=>{let{m:r,id:l,defs:o}=xa(t);return(0,u.jsxs)("svg",{width:e,height:e,viewBox:"0 0 100 100","aria-hidden":"true",style:{flexShrink:0},children:[o,(0,u.jsx)("path",{d:"M50 4 L96 50 L50 96 L4 50 Z",fill:`url(#${l})`,stroke:r.lo,strokeWidth:"2.6",strokeLinejoin:"round"}),(0,u.jsx)("path",{d:"M50 15 L85 50 L50 85 L15 50 Z",fill:"none",stroke:r.ink,strokeWidth:"1.4",opacity:".3"}),(0,u.jsx)("path",{d:"M50 4 L96 50 L50 50 Z",fill:r.hi,opacity:".28"}),n&&(0,u.jsx)(ka,{cx:50,cy:50,s:26})]})},s1=({size:e=46,metal:t="bronze"})=>{let{m:n,id:r,defs:l}=xa(t);return(0,u.jsxs)("svg",{width:e,height:e,viewBox:"0 0 100 100","aria-hidden":"true",style:{flexShrink:0},children:[l,(0,u.jsx)("circle",{cx:"50",cy:"50",r:"46",fill:`url(#${r})`,stroke:n.lo,strokeWidth:"2.4"}),(0,u.jsx)("circle",{cx:"50",cy:"50",r:"38",fill:"none",stroke:n.ink,strokeWidth:"1.5",opacity:".32"}),Array.from({length:24}).map((o,i)=>{let a=i*15*Math.PI/180;return(0,u.jsx)("line",{x1:50+Math.cos(a)*39,y1:50+Math.sin(a)*39,x2:50+Math.cos(a)*45,y2:50+Math.sin(a)*45,stroke:n.ink,strokeWidth:"1.3",opacity:".42"},i)}),(0,u.jsx)(ka,{cx:50,cy:50,s:26})]})},Ln=({kind:e,n:t=1,size:n=40,metal:r,mark:l=!0})=>e==="seal"?(0,u.jsx)(s1,{size:n,metal:r}):e==="field"?(0,u.jsx)(a1,{size:n,metal:r,mark:l}):(0,u.jsx)(i1,{n:t,size:n,metal:r,mark:l}),u1=({seed:e="GA",size:t=72})=>{let n=7;for(let s of e)n=n*31+s.charCodeAt(0)&2147483647;let r=()=>(n=n*1103515245+12345&2147483647,n/2147483647),l=21,o=100/l,i=[],a=(s,d)=>{i.push((0,u.jsx)("rect",{x:s*o,y:d*o,width:o*7,height:o*7,fill:m.navy},"f"+s+d)),i.push((0,u.jsx)("rect",{x:(s+1)*o,y:(d+1)*o,width:o*5,height:o*5,fill:"#fff"},"g"+s+d)),i.push((0,u.jsx)("rect",{x:(s+2)*o,y:(d+2)*o,width:o*3,height:o*3,fill:m.navy},"h"+s+d))};for(let s=0;s<l;s++)for(let d=0;d<l;d++)!(d<8&&s<8||d>l-9&&s<8||d<8&&s>l-9)&&r()>.52&&i.push((0,u.jsx)("rect",{x:d*o,y:s*o,width:o+.35,height:o+.35,fill:m.navy},d+"_"+s));return a(0,0),a(l-7,0),a(0,l-7),(0,u.jsx)("svg",{viewBox:"0 0 100 100",width:t,height:t,"aria-hidden":"true",children:i})},c1=()=>(0,u.jsx)("svg",{width:"19",height:"19",viewBox:"0 0 24 24",fill:"#fff","aria-hidden":"true",children:(0,u.jsx)("path",{d:"M21.9 4.3 18.9 19c-.2 1-.8 1.3-1.7.8l-4.6-3.4-2.2 2.1c-.3.3-.5.5-1 .5l.4-4.9 8.9-8c.4-.3-.1-.5-.6-.2L7.2 12.6 2.7 11.2c-1-.3-1-1 .2-1.4l18-6.9c.8-.3 1.5.2 1 1.4z"})});function ya({children:e,onClose:t,label:n}){let r=(0,G.useRef)(null),l=(0,G.useRef)(null),o=(0,G.useRef)(t);return o.current=t,(0,G.useEffect)(()=>{l.current=document.activeElement;let i=document.body.style.overflow;document.body.style.overflow="hidden";let a=setTimeout(()=>r.current?.focus({preventScroll:!0}),40),s=d=>{if(d.key==="Escape"){d.preventDefault(),o.current();return}if(d.key!=="Tab"||!r.current)return;let g=[...r.current.querySelectorAll("button:not([disabled]),input,[tabindex]:not([tabindex='-1'])")].filter(w=>w.offsetParent!==null);if(!g.length)return;let v=g[0],y=g[g.length-1];d.shiftKey&&(document.activeElement===v||document.activeElement===r.current)?(d.preventDefault(),y.focus({preventScroll:!0})):!d.shiftKey&&document.activeElement===y&&(d.preventDefault(),v.focus({preventScroll:!0}))};return document.addEventListener("keydown",s),()=>{clearTimeout(a),document.removeEventListener("keydown",s),document.body.style.overflow=i,l.current?.focus?.({preventScroll:!0})}},[]),(0,u.jsx)("div",{className:"modal",role:"dialog","aria-modal":"true","aria-label":n,onClick:t,children:(0,u.jsxs)("div",{className:"sheet up",ref:r,tabIndex:-1,onClick:i=>i.stopPropagation(),children:[(0,u.jsx)("div",{className:"grab only-mobile"}),e]})})}function d1({fire:e}){let[t,n]=(0,G.useState)([]);return(0,G.useEffect)(()=>{if(!e||window.matchMedia?.("(prefers-reduced-motion: reduce)").matches)return;let r=[m.gold,m.blue,m.navy,Gl,m.good,"#fff"];n(Array.from({length:80},(o,i)=>({id:e+"-"+i,left:50+(Math.random()-.5)*70,tx:(Math.random()-.5)*600,ty:120+Math.random()*260,rot:(Math.random()-.5)*900,c:r[Math.random()*r.length|0],w:6+Math.random()*7,h:9+Math.random()*12,d:1.5+Math.random()*.8,delay:Math.random()*.2})));let l=setTimeout(()=>n([]),2800);return()=>clearTimeout(l)},[e]),t.length?(0,u.jsx)("div",{className:"cf-wrap","aria-hidden":"true",children:t.map(r=>(0,u.jsx)("span",{className:"cf",style:{left:r.left+"%",width:r.w,height:r.h,background:r.c,"--tx":r.tx+"px","--ty":r.ty+"px","--rot":r.rot+"deg",animationDuration:r.d+"s",animationDelay:r.delay+"s"}},r.id))}):null}var f1=()=>(0,u.jsx)("style",{children:`
@import url('https://fonts.googleapis.com/css2?family=Sora:wght@600;700&family=Anton&family=Inter:wght@400;500;600;700&family=Playfair+Display:ital@1&display=swap');
*{box-sizing:border-box;-webkit-tap-highlight-color:transparent;}
html,body{margin:0;overflow-x:hidden;}
.ga{min-height:100vh;min-height:100dvh;background:${m.paper};color:${m.ink};font-family:'Inter',system-ui,sans-serif;font-size:15px;}
.ga *{max-width:100%;}
.plate-mark,.cert-mark{max-width:none !important;}
button{font-family:'Sora',system-ui,sans-serif;border:none;cursor:pointer;min-height:44px;}
button:focus-visible,[tabindex]:focus-visible{outline:3px solid ${m.blue};outline-offset:2px;}
.tap{transition:transform .08s ease;} .tap:active{transform:scale(.98);}
h1,h2,h3,p{margin:0;overflow-wrap:anywhere;}
.sr-only{position:absolute;width:1px;height:1px;overflow:hidden;clip:rect(0 0 0 0);white-space:nowrap;}
.skip{position:absolute;left:-9999px;top:8px;z-index:100;background:${m.navy};color:#fff;padding:12px 18px;border-radius:10px;font-weight:700;text-decoration:none;}
.skip:focus{left:16px;}
.grow{flex:1;min-width:0;} .mt{margin-top:18px;} .center{text-align:center;}
.noscroll::-webkit-scrollbar{display:none;} .noscroll{scrollbar-width:none;}

.shell{display:block;}
.side{display:none;}
.col{max-width:440px;margin:0 auto;padding:0 max(16px,env(safe-area-inset-left)) 120px;}
.brand{display:flex;align-items:flex-end;gap:8px;}
.serif{font-family:'Playfair Display',Georgia,serif;font-style:italic;font-size:19px;line-height:.95;color:${m.navy};}
.serif.big{font-size:23px;}
.mast{display:flex;align-items:flex-end;justify-content:space-between;gap:12px;padding:22px 2px 4px;}
.sub{font-size:13.5px;color:${m.mute};padding:0 2px 8px;}
.pill{background:${m.card};border:1.5px solid ${m.line};border-radius:999px;padding:0 16px;min-height:44px;font-size:13.5px;font-weight:700;color:${m.navy};}
.pill.sm{font-size:13px;padding:0 14px;}

/* ladder */
.ladder{display:flex;gap:8px;overflow-x:auto;padding:8px 0 2px;}
.rung{flex-shrink:0;display:flex;align-items:center;gap:8px;padding:10px 15px;border-radius:12px;
      background:${m.card};border:1.5px solid ${m.line};color:${m.ink};}
.rung.on{background:${m.navy};border-color:${m.navy};color:#fff;}
.rung .ant{font-family:'Anton',sans-serif;font-size:15px;letter-spacing:.06em;}
.lock{font-family:'Inter',sans-serif;font-size:12px;font-weight:600;color:${m.mute};}
.rung.on .lock{color:rgba(255,255,255,.7);}

/* plate */
.plate{background:${gd};background-color:${m.brandD};border-radius:18px;padding:20px 18px;color:#fff;margin-top:14px;
       position:relative;overflow:hidden;isolation:isolate;box-shadow:0 18px 40px -22px rgba(14,34,73,.7);}
.plate.done{background:linear-gradient(160deg,#1a7a49,#0f5a35);}
.hatch{background-image:repeating-linear-gradient(115deg,rgba(255,255,255,.075) 0 2px,transparent 2px 13px);}
.plate-mark{position:absolute;top:50%;left:76%;transform:translateY(-50%);opacity:.16;z-index:-1;}
.rule-row{display:flex;align-items:center;gap:9px;}
.rule-row i{height:2px;width:22px;background:${m.gold};display:block;}
.rule-row span{font-size:12.5px;letter-spacing:.14em;text-transform:uppercase;opacity:.92;}
.plate-title{font-family:'Anton',sans-serif;font-size:30px;letter-spacing:.03em;margin-top:7px;line-height:1.02;text-transform:uppercase;}
.plate-sub{font-size:14px;color:rgba(255,255,255,.8);margin-top:5px;}
.plate-foot{display:flex;align-items:flex-end;justify-content:space-between;gap:12px;margin-top:12px;}
.plate-foot b{font-size:15px;}
.pips{display:flex;gap:4px;}
.pip{width:9px;height:9px;border-radius:2px;transform:rotate(45deg);background:rgba(255,255,255,.28);}
.pip.done{background:${m.gold};} .pip.booked{background:rgba(245,183,22,.5);} .pip.missed{background:${m.clay};}
.bar{height:8px;background:rgba(255,255,255,.25);border-radius:99px;margin-top:10px;overflow:hidden;}
.bar i{display:block;height:100%;background:${m.gold};transition:width .45s cubic-bezier(.4,0,.2,1);}
.plate-note{font-size:13px;opacity:.92;margin-top:9px;}

/* chat */
.chat{width:100%;margin-top:12px;background:${m.card};border:1.5px solid ${m.line};border-radius:14px;
      padding:13px 14px;display:flex;align-items:center;gap:12px;text-align:left;}
.tg{width:42px;height:42px;border-radius:12px;background:${m.tg};display:grid;place-items:center;flex-shrink:0;}
.chat .left b{display:block;font-family:'Sora',sans-serif;font-size:15.5px;font-weight:600;color:${m.navy};}
.chat .left em{display:block;font-size:13.5px;color:${m.mute};font-style:normal;margin-top:2px;}

/* section titles */
.bar-title{display:flex;align-items:center;gap:10px;margin:24px 0 14px;}
.bar-title:after{content:"";flex:1;height:1px;background:${m.line};}
.sec{font-family:'Anton',sans-serif;font-size:15px;letter-spacing:.11em;text-transform:uppercase;color:${m.navy};}
.sec:focus{outline:none;}

/* requirements */
.reqs{list-style:none;margin:0;padding:0;}
.req{display:flex;gap:12px;align-items:stretch;}
.spine{width:30px;position:relative;flex-shrink:0;}
.rail{position:absolute;left:14px;width:2px;}
.node{position:absolute;left:3px;top:18px;width:24px;height:24px;border-radius:50%;background:#fff;
      border:2.5px solid #c3cedd;display:grid;place-items:center;color:${m.navy};font-size:13px;font-weight:800;
      font-family:'Sora',sans-serif;z-index:1;}
.node.done{background:${m.gold};border-color:${m.gold};}
.node.booked{border-color:${m.gold};}
.node.missed{border-color:${m.clay};color:${m.clay};}
.req-card{flex:1;min-width:0;background:${m.card};border:1.5px solid ${m.line};border-radius:14px;margin-bottom:10px;overflow:hidden;}
.req-card.active{border-color:${m.blue};box-shadow:0 10px 26px -18px rgba(37,105,184,.9);}
.req-card.missed{border-color:${m.clay};}
.req-head{padding:14px 15px 13px;}
.req-type{font-size:12px;font-weight:700;letter-spacing:.07em;text-transform:uppercase;}
.req-head h3{font-family:'Sora',sans-serif;font-size:16.5px;font-weight:600;color:${m.navy};margin-top:4px;line-height:1.3;}
.req-head p{font-size:14px;margin-top:5px;line-height:1.5;}
.req-act{padding:0 15px 15px;}
.btn.flat{margin-top:0;}

/* dates */
.dates{border-top:1px solid ${m.line};background:${m.paper};padding:6px 12px 12px;}
.fine.pad{padding:14px 4px;}
.ev{background:${m.card};border:1.5px solid ${m.line};border-radius:12px;padding:12px;margin-top:8px;
    display:flex;gap:12px;align-items:center;}
.ev.mine{border-color:${m.gold};}
.datebox{width:54px;flex-shrink:0;text-align:center;padding:6px 0;border-radius:10px;background:${m.paper};border:1px solid ${m.line};}
.datebox em{display:block;font-size:11.5px;color:${m.mute};text-transform:uppercase;font-style:normal;}
.datebox b{display:block;font-family:'Anton',sans-serif;font-size:20px;font-weight:400;color:${m.navy};line-height:1.05;}
.ev-place{font-family:'Sora',sans-serif;font-size:15px;font-weight:600;color:${m.navy};}
.ev-meta{font-size:13.5px;color:${m.mute};margin-top:3px;display:flex;align-items:center;gap:5px;flex-wrap:wrap;}
.ev-seats{font-size:13.5px;margin-top:3px;}
.confirm{display:flex;flex-direction:column;gap:6px;flex-shrink:0;}

/* buttons */
.btn{border-radius:12px;font-size:15px;font-weight:700;padding:0 18px;min-height:48px;}
.btn.wide{width:100%;margin-top:12px;}
.btn.sm{min-height:44px;font-size:13.5px;padding:0 14px;flex-shrink:0;}
.btn.primary{background:${m.blue};color:#fff;}
.btn.navy{background:${m.navy};color:#fff;}
.btn.tg{background:${m.tg};color:#fff;}
.btn.outline{background:#fff;border:1.5px solid ${m.line};color:${m.navy};}
.btn.danger{background:#fff;border:1.5px solid ${m.clay};color:${m.clay};}
.btn.booked{background:${m.warnBg};border:1.5px solid ${m.gold};color:${m.warn};}
.btn:disabled{background:${m.line};color:${m.mute};cursor:not-allowed;}

/* outcome */
.outcome{display:flex;gap:12px;align-items:center;background:${m.oliveLt};border:1.5px solid #d7dccf;
         border-radius:14px;padding:16px 15px;}
.outcome.done{background:${m.goodBg};border-color:${m.good};}
.outcome p{font-size:14.5px;color:${m.olive};line-height:1.55;font-weight:500;}
.outcome.done p{color:${m.good};}

/* sticky next */
.foot{position:fixed;left:0;right:0;bottom:0;z-index:40;background:${m.card};border-top:1px solid ${m.line};
      box-shadow:0 -8px 26px rgba(15,36,68,.12);padding:12px 16px calc(12px + env(safe-area-inset-bottom));}
.foot-in{max-width:440px;margin:0 auto;display:flex;gap:12px;align-items:center;}
.foot-title{font-family:'Sora',sans-serif;font-size:15px;font-weight:600;color:${m.navy};
            white-space:nowrap;overflow:hidden;text-overflow:ellipsis;display:block;}
.eyebrow-dark{font-family:'Inter',sans-serif;font-size:12px;font-weight:700;letter-spacing:.07em;text-transform:uppercase;color:${m.mute};}

/* sheets */
.modal{position:fixed;inset:0;z-index:60;background:rgba(14,34,73,.55);display:flex;align-items:flex-end;justify-content:center;}
.sheet{width:100%;max-width:440px;max-height:90vh;max-height:90dvh;overflow-y:auto;background:${m.card};
       border-radius:20px 20px 0 0;padding:14px 16px calc(26px + env(safe-area-inset-bottom));outline:none;}
.grab{width:40px;height:4px;border-radius:2px;background:${m.line};margin:0 auto 14px;}
.sheet-head{display:flex;justify-content:space-between;align-items:flex-start;gap:12px;margin-bottom:12px;}
.h1{font-family:'Anton',sans-serif;font-size:24px;color:${m.navy};text-transform:uppercase;letter-spacing:.03em;line-height:1.1;}
.h2{font-family:'Sora',sans-serif;font-size:19px;font-weight:700;color:${m.navy};}
.fine{font-size:13px;color:${m.mute};line-height:1.55;margin-top:6px;}
.lead{font-size:15px;color:${m.ink};line-height:1.7;margin-top:12px;}
.langs{display:flex;gap:6px;margin-top:14px;padding:4px;background:${m.paper};border:1px solid ${m.line};border-radius:12px;}
.lang{flex:1;min-height:44px;border-radius:9px;background:transparent;color:${m.mute};font-size:14px;font-weight:700;}
.lang.on{background:${m.navy};color:#fff;}
.video{aspect-ratio:16/9;border-radius:14px;margin-top:12px;display:grid;place-items:center;cursor:pointer;text-align:center;}
.play{width:52px;height:52px;border-radius:50%;margin:0 auto;display:grid;place-items:center;color:#fff;font-size:18px;}
.video em{display:block;font-size:14px;margin-top:10px;font-weight:600;font-style:normal;}
.doc{max-height:200px;overflow-y:auto;padding:15px;border-radius:12px;background:${m.paper};border:1px solid ${m.line};
     font-size:14px;color:${m.ink};line-height:1.75;}

/* certificate */
.cert{background:linear-gradient(160deg,#FCFAF4,#F3EFE4);border-radius:18px;padding:26px 20px 22px;
      position:relative;overflow:hidden;isolation:isolate;border:1px solid #E3DCC9;outline:6px solid ${m.navy};outline-offset:-13px;text-align:center;color:${m.navy};}
.cert-mark{position:absolute;top:50%;left:50%;transform:translate(-50%,-50%);opacity:.05;z-index:-1;}
.cert-brand{display:flex;align-items:flex-end;justify-content:center;gap:7px;}
.cert-eyebrow{font-size:11px;letter-spacing:.34em;text-transform:uppercase;color:${m.goldD};margin-top:15px;font-weight:700;padding-left:.34em;}
.cert-ins{display:flex;justify-content:center;align-items:center;min-height:60px;margin:16px 0 2px;}
.cert-name{font-family:'Playfair Display',Georgia,serif;font-style:italic;font-size:28px;margin-top:16px;line-height:1.2;}
.cert-rank{font-size:13px;color:${m.mute};margin-top:7px;}
.cert-hr{height:1px;background:rgba(14,34,73,.2);margin:18px 22px;}
.cert-cite{font-size:13.5px;color:${m.ink};line-height:1.72;margin:0 10px;}
.cert-evidence{font-size:11px;letter-spacing:.06em;text-transform:uppercase;color:${m.mute};margin-top:16px;}
.cert-sigs{display:flex;gap:18px;justify-content:center;margin-top:24px;}
.cert-sigs div{flex:1;max-width:150px;}
.cert-sigs span{display:block;height:1px;background:rgba(14,34,73,.2);}
.cert-sigs em{display:block;font-size:10px;letter-spacing:.1em;text-transform:uppercase;color:${m.mute};margin-top:6px;font-style:normal;}
.cert-qr{display:flex;flex-direction:column;align-items:center;margin-top:22px;}
.cert-qr svg{background:#fff;padding:6px;border-radius:8px;border:1px solid rgba(14,34,73,.2);}
.cert-qr em{font-size:9.5px;letter-spacing:.13em;text-transform:uppercase;color:${m.mute};margin-top:7px;font-style:normal;}
.cert-record{display:flex;justify-content:space-between;gap:12px;margin-top:16px;padding-top:13px;border-top:1px solid rgba(14,34,73,.2);}
.cert-record em{display:block;font-size:10px;letter-spacing:.14em;text-transform:uppercase;color:${m.mute};font-style:normal;}
.cert-record b{display:block;font-family:'Sora',sans-serif;font-size:12.5px;font-weight:600;margin-top:2px;}
.cert-fine{font-size:10px;color:${m.mute};line-height:1.5;margin:13px 8px 0;opacity:.85;}

/* about */
.about-lvl{display:flex;gap:13px;align-items:flex-start;padding-bottom:14px;}
.about-lvl b{display:block;font-family:'Sora',sans-serif;font-size:15.5px;font-weight:700;color:${m.navy};}
.about-lvl em{display:block;font-size:13.5px;color:${m.mute};font-style:normal;margin-top:2px;}
.about-table{border:1px solid ${m.line};border-radius:14px;overflow:hidden;}
.about-table div{padding:13px 14px;border-top:1px solid ${m.line};}
.about-table div:first-child{border-top:none;}
.about-table div:nth-child(even){background:${m.paper};}
.about-table b{display:block;font-family:'Sora',sans-serif;font-size:14.5px;font-weight:600;color:${m.navy};}
.about-table span{display:block;font-size:14px;color:${m.ink};margin-top:3px;line-height:1.6;}
.closing{background:${m.oliveLt};border:1.5px solid #d7dccf;border-radius:14px;padding:15px;
         font-size:14.5px;color:${m.olive};line-height:1.7;margin-top:20px;}

/* demo */
.demo{margin-top:26px;padding:14px;background:${m.card};border:1.5px dashed ${m.sky};border-radius:14px;}
.demo-label{font-size:11.5px;font-weight:700;letter-spacing:.08em;text-transform:uppercase;color:${m.mute};}
.demo-note{font-size:13px;color:${m.mute};line-height:1.55;margin-top:7px;}
.demo-row{display:flex;gap:7px;flex-wrap:wrap;margin-top:10px;}
.demo-btn{flex:1 1 30%;min-height:44px;border-radius:10px;font-size:12.5px;font-weight:700;
          background:#fff;border:1.5px solid ${m.line};color:${m.navy};padding:0 10px;}

/* toast + confetti */
.toast{position:fixed;left:16px;right:16px;bottom:96px;z-index:70;margin:0 auto;max-width:400px;text-align:center;
       background:${m.navy};color:#fff;padding:12px 18px;border-radius:12px;font-size:14px;
       box-shadow:0 12px 30px -10px rgba(14,34,73,.6);}
.cf-wrap{position:fixed;inset:0;z-index:90;pointer-events:none;overflow:hidden;}
.cf{position:absolute;top:26%;border-radius:2px;animation-name:cf;animation-timing-function:cubic-bezier(.15,.6,.4,1);animation-fill-mode:forwards;}
@keyframes cf{0%{transform:translate(0,0) rotate(0);opacity:1}100%{transform:translate(var(--tx),var(--ty)) rotate(var(--rot));opacity:0}}
@keyframes fade{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:none}} .fade{animation:fade .2s ease;}
@keyframes up{from{transform:translateY(20px);opacity:0}to{transform:none;opacity:1}} .up{animation:up .24s ease;}

/* desktop */
@media(min-width:900px){
  .shell{display:flex;max-width:1240px;margin:0 auto;min-height:100vh;align-items:stretch;}
  .side{display:flex;flex-direction:column;width:280px;flex-shrink:0;gap:10px;padding:28px 20px;
        background:${m.card};border-right:1px solid ${m.line};position:sticky;top:0;height:100vh;overflow-y:auto;}
  .col{flex:1;max-width:100%;margin:0;padding:30px 34px 60px;}
  .only-mobile{display:none !important;}
  .foot{display:none;}
  .modal{align-items:center;padding:24px;}
  .sheet{max-width:560px;border-radius:20px;max-height:88vh;}
  .who{display:flex;align-items:center;gap:11px;padding:12px 0 16px;border-bottom:1px solid ${m.line};}
  .avatar{width:40px;height:40px;border-radius:50%;background:${m.navy};color:#fff;display:grid;place-items:center;
          font-family:'Sora',sans-serif;font-weight:700;font-size:14px;flex-shrink:0;}
  .who b{display:block;font-family:'Sora',sans-serif;font-size:15px;color:${m.navy};}
  .who em{display:block;font-size:13px;color:${m.mute};font-style:normal;}
  .side-nav{display:flex;flex-direction:column;gap:6px;padding-top:4px;}
  .side-rank{display:flex;align-items:center;gap:11px;width:100%;text-align:left;padding:11px 13px;border-radius:12px;
             background:transparent;color:${m.ink};}
  .side-rank.on{background:${m.navy};color:#fff;}
  .side-rank b{display:block;font-family:'Sora',sans-serif;font-size:14.5px;font-weight:700;}
  .side-rank em{display:block;font-size:12.5px;font-style:normal;opacity:.75;}
  .tickmini{color:${m.good};font-weight:800;}
  .side-btn{margin-top:6px;width:100%;text-align:left;padding:11px 13px;border-radius:12px;background:${m.paper};
            border:1.5px solid ${m.line};color:${m.navy};font-size:14px;font-weight:700;}
  .side-next{margin-top:auto;padding-top:18px;border-top:1px solid ${m.line};}
  .side-next b{display:block;font-family:'Sora',sans-serif;font-size:15px;color:${m.navy};margin:5px 0 0;line-height:1.35;}
}
@media(min-width:1180px){ .col{padding:34px 48px 70px;} }

/* small */
@media(max-width:400px){.ga{font-size:14.5px;}.col{padding-left:13px;padding-right:13px;}}
@media(max-width:360px){.col{padding-left:11px;padding-right:11px;}.spine{width:24px;}
  .ev{flex-wrap:wrap;}.ev-act{width:100%;}.datebox{width:46px;}}
@media(max-width:320px){.col{padding-left:9px;padding-right:9px;}.ga{font-size:14px;}}
@media(prefers-reduced-motion:reduce){.fade,.up,.cf{animation:none;}}

/* print */
@media print{
  @page{size:A4 portrait;margin:14mm;}
  .shell,.foot,.no-print,.cf-wrap,.toast{display:none !important;}
  .modal{position:static !important;background:#fff !important;padding:0 !important;display:block !important;}
  .sheet{max-width:none !important;max-height:none !important;overflow:visible !important;border-radius:0 !important;box-shadow:none !important;padding:0 !important;}
  .cert{outline-offset:-10px !important;border-radius:0 !important;-webkit-print-color-adjust:exact;print-color-adjust:exact;}
  body{background:#fff !important;}
}
  `});(0,vd.createRoot)(document.getElementById("root")).render(yd.default.createElement(va));})();
/*! Bundled license information:

react/cjs/react.production.min.js:
  (**
   * @license React
   * react.production.min.js
   *
   * Copyright (c) Facebook, Inc. and its affiliates.
   *
   * This source code is licensed under the MIT license found in the
   * LICENSE file in the root directory of this source tree.
   *)

scheduler/cjs/scheduler.production.min.js:
  (**
   * @license React
   * scheduler.production.min.js
   *
   * Copyright (c) Facebook, Inc. and its affiliates.
   *
   * This source code is licensed under the MIT license found in the
   * LICENSE file in the root directory of this source tree.
   *)

react-dom/cjs/react-dom.production.min.js:
  (**
   * @license React
   * react-dom.production.min.js
   *
   * Copyright (c) Facebook, Inc. and its affiliates.
   *
   * This source code is licensed under the MIT license found in the
   * LICENSE file in the root directory of this source tree.
   *)

react/cjs/react-jsx-runtime.production.min.js:
  (**
   * @license React
   * react-jsx-runtime.production.min.js
   *
   * Copyright (c) Facebook, Inc. and its affiliates.
   *
   * This source code is licensed under the MIT license found in the
   * LICENSE file in the root directory of this source tree.
   *)
*/
</script>
</body>
</html>
````


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



---

<!-- FILE: Inbox/gentrep-academy-dashboard/stitch-export.html -->
# Inbox/gentrep-academy-dashboard/stitch-export.html

````html
<!DOCTYPE html>

<html class="light" lang="en"><head>
<meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>Gentrep Academy Dashboard</title>
<script src="https://cdn.tailwindcss.com?plugins=forms,container-queries"></script>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&amp;family=Newsreader:wght@400;500;600;700;800&amp;family=Public+Sans:wght@500;600;700&amp;display=swap" rel="stylesheet"/>
<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1&amp;display=swap" rel="stylesheet"/>
<script id="tailwind-config">
        tailwind.config = {
          darkMode: "class",
          theme: {
            extend: {
              "colors": {
                      "on-secondary-container": "#7a5c2e",
                      "on-primary-container": "#878eff",
                      "on-tertiary-fixed": "#400100",
                      "on-error-container": "#93000a",
                      "secondary-fixed-dim": "#e8c08a",
                      "surface-container-low": "#f6f3ec",
                      "surface-dim": "#dcdad3",
                      "on-tertiary": "#ffffff",
                      "outline": "#767686",
                      "on-secondary-fixed-variant": "#5d4217",
                      "on-background": "#1c1c18",
                      "inverse-surface": "#31312c",
                      "on-tertiary-fixed-variant": "#891d11",
                      "on-surface": "#1c1c18",
                      "on-secondary-fixed": "#291800",
                      "on-secondary": "#ffffff",
                      "on-error": "#ffffff",
                      "error-container": "#ffdad6",
                      "surface-container-lowest": "#ffffff",
                      "inverse-on-surface": "#f3f0e9",
                      "background": "#fcf9f2",
                      "primary": "#000070",
                      "surface-tint": "#444dd4",
                      "secondary-fixed": "#ffddb1",
                      "surface-bright": "#fcf9f2",
                      "primary-fixed-dim": "#bfc2ff",
                      "on-primary": "#ffffff",
                      "surface-container-high": "#ebe8e1",
                      "secondary": "#77592c",
                      "on-tertiary-container": "#f86e59",
                      "inverse-primary": "#bfc2ff",
                      "error": "#ba1a1a",
                      "primary-container": "#0608a9",
                      "on-primary-fixed": "#00006e",
                      "outline-variant": "#c6c5d7",
                      "on-surface-variant": "#454654",
                      "primary-fixed": "#e0e0ff",
                      "secondary-container": "#ffd69f",
                      "tertiary-fixed-dim": "#ffb4a7",
                      "surface-container-highest": "#e5e2db",
                      "surface-variant": "#e5e2db",
                      "tertiary-container": "#690300",
                      "tertiary": "#420100",
                      "tertiary-fixed": "#ffdad4",
                      "surface": "#fcf9f2",
                      "surface-container": "#f1eee7",
                      "on-primary-fixed-variant": "#2930bc"
              },
              "borderRadius": {
                      "DEFAULT": "0.25rem",
                      "lg": "0.5rem",
                      "xl": "0.75rem",
                      "full": "9999px",
                      "card": "14px"
              },
              "spacing": {},
              "fontFamily": {
                      "headline": [
                              "Newsreader"
                      ],
                      "display": [
                              "Newsreader"
                      ],
                      "body": [
                              "Inter"
                      ],
                      "label": [
                              "Public Sans"
                      ]
              },
              "fontSize": {}
      },
          },
        }
      </script>
<style>
        body {
            background-color: #F4F1EA;
            color: #0F0F18;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)' opacity='0.05'/%3E%3C/svg%3E");
        }
        .surface-card {
            background-color: #FCFAF5;
            border: 1px solid #D8D2C2;
            border-radius: 14px;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05), 0 2px 4px -1px rgba(0, 0, 0, 0.03);
        }
      </style>
</head>
<body class="flex min-h-screen">
<!-- SideNavBar -->
<nav class="h-screen w-64 fixed left-0 top-0 bg-surface-container-low dark:bg-surface-container border-r border-outline-variant flex flex-col h-full py-6 z-50">
<div class="px-6 mb-8 flex items-center gap-3">
<div class="w-8 h-8 rounded-full bg-primary-container flex items-center justify-center text-on-primary font-headline font-bold">G</div>
<div>
<h1 class="font-headline text-lg font-black text-primary">Gentrep Academy</h1>
<p class="font-body text-xs text-on-surface-variant uppercase tracking-wider">Member Portal</p>
</div>
</div>
<ul class="flex-1 px-4 space-y-1">
<li>
<a class="flex items-center gap-3 text-primary bg-primary-container/10 border-r-4 border-primary px-4 py-3 rounded-l-lg font-body text-sm font-medium scale-98 active:scale-95 transition-transform" href="#">
<span class="material-symbols-outlined text-lg" style="font-variation-settings: 'FILL' 1;">dashboard</span>
                    Dashboard
                </a>
</li>
<li>
<a class="flex items-center gap-3 text-on-surface-variant hover:text-on-surface px-4 py-3 rounded-lg font-body text-sm font-medium hover:bg-surface-container-high transition-all scale-98 active:scale-95 transition-transform" href="#">
<span class="material-symbols-outlined text-lg">menu_book</span>
                    Curriculum
                </a>
</li>
<li>
<a class="flex items-center gap-3 text-on-surface-variant hover:text-on-surface px-4 py-3 rounded-lg font-body text-sm font-medium hover:bg-surface-container-high transition-all scale-98 active:scale-95 transition-transform" href="#">
<span class="material-symbols-outlined text-lg">event_available</span>
                    Training
                </a>
</li>
<li>
<a class="flex items-center gap-3 text-on-surface-variant hover:text-on-surface px-4 py-3 rounded-lg font-body text-sm font-medium hover:bg-surface-container-high transition-all scale-98 active:scale-95 transition-transform" href="#">
<span class="material-symbols-outlined text-lg">folder_shared</span>
                    Resources
                </a>
</li>
<li>
<a class="flex items-center gap-3 text-on-surface-variant hover:text-on-surface px-4 py-3 rounded-lg font-body text-sm font-medium hover:bg-surface-container-high transition-all scale-98 active:scale-95 transition-transform" href="#">
<span class="material-symbols-outlined text-lg">military_tech</span>
                    Academy Rank
                </a>
</li>
</ul>
<div class="px-4 mt-auto space-y-1">
<a class="flex items-center gap-3 text-on-surface-variant hover:text-on-surface px-4 py-3 rounded-lg font-body text-sm font-medium hover:bg-surface-container-high transition-all" href="#">
<span class="material-symbols-outlined text-lg">settings</span>
                Settings
            </a>
<a class="flex items-center gap-3 text-on-surface-variant hover:text-on-surface px-4 py-3 rounded-lg font-body text-sm font-medium hover:bg-surface-container-high transition-all" href="#">
<span class="material-symbols-outlined text-lg">help_outline</span>
                Support
            </a>
<div class="mt-4 pt-4 border-t border-outline-variant px-4 flex items-center justify-between">
<div class="flex items-center gap-2">
<div class="w-8 h-8 rounded-full bg-surface-variant overflow-hidden">
<img class="w-full h-full object-cover" data-alt="A close up, professional portrait of a business person in a well lit studio setting with a clean, modern aesthetic. The lighting should be soft and flattering, highlighting features gently." src="https://lh3.googleusercontent.com/aida-public/AB6AXuCX1OCTTaoTtErouviSsXJwqrYUegzXy__S0ziK7MeNvCyAEWLt9W1fqt3nnV5axsOyze2szn5RtV-Rc17PvsS9Rq6l812_3Jni23ZI9AXB38Er-HsYdGOZsG0UwXFpT-c_5iBw8E--n7AuTX4dPy33ZRWAfjhKavmVtY2Au0_DtW1qWBAUKII9YaFwu-RXloeD9Ify10mcCYYik817z71igV8oItIOSlAdsnvdKoPNP7eSYO31Z8MTurfMon4Q3m6EXXnCZUyFuZc"/>
</div>
<div>
<p class="font-body text-sm font-medium text-on-surface">J. Dela Cruz</p>
<p class="font-body text-xs text-on-surface-variant">View Profile</p>
</div>
</div>
</div>
</div>
</nav>
<!-- Main Content -->
<main class="ml-64 flex-1 flex flex-col">
<!-- Alert Band -->
<div class="bg-primary-container text-on-primary py-2 px-8 flex items-center justify-between text-sm font-body">
<div class="flex items-center gap-2">
<span class="material-symbols-outlined text-sm">stars</span>
<span><strong>Recognition Night Invite:</strong> You are eligible for Rank Certification. RSVP required by Friday.</span>
</div>
<a class="underline font-medium hover:text-primary-fixed-dim transition-colors" href="#">Action Required</a>
</div>
<div class="p-8 max-w-7xl mx-auto w-full space-y-10">
<!-- Header -->
<header class="space-y-2">
<p class="font-label text-xs uppercase tracking-widest text-secondary font-bold">ACADEMY</p>
<h2 class="font-headline text-4xl font-semibold text-on-surface tracking-tight">Your training path</h2>
<p class="font-body text-on-surface-variant max-w-2xl text-lg">Continue your progression through the Gentrep curriculum. Next major milestone: Certification.</p>
</header>
<!-- Summary Cards -->
<section class="grid grid-cols-1 md:grid-cols-3 gap-6">
<!-- Status -->
<div class="surface-card p-6 flex flex-col justify-between">
<div class="flex items-start justify-between mb-4">
<div class="w-10 h-10 rounded-full bg-surface-variant flex items-center justify-center text-primary">
<span class="material-symbols-outlined">check_circle</span>
</div>
<span class="font-label text-xs uppercase tracking-wider text-on-surface-variant bg-surface-container-highest px-2 py-1 rounded">Status</span>
</div>
<div>
<p class="font-headline text-2xl font-semibold text-on-surface">Activated Member</p>
<p class="font-body text-sm text-on-surface-variant mt-1">In good standing</p>
</div>
</div>
<!-- Rank -->
<div class="surface-card p-6 flex flex-col justify-between bg-[#F4F1EA]">
<div class="flex items-start justify-between mb-4">
<div class="w-10 h-10 rounded-full bg-secondary/10 flex items-center justify-center text-secondary">
<span class="material-symbols-outlined" style="font-variation-settings: 'FILL' 1;">military_tech</span>
</div>
<span class="font-label text-xs uppercase tracking-wider text-secondary font-bold px-2 py-1 rounded">Current Rank</span>
</div>
<div>
<p class="font-headline text-2xl font-semibold text-on-surface">Team Leader</p>
<p class="font-body text-sm text-on-surface-variant mt-1">Tier 2</p>
</div>
</div>
<!-- Certificate -->
<div class="surface-card p-6 flex flex-col justify-between">
<div class="flex items-start justify-between mb-4">
<div class="w-10 h-10 rounded-full bg-surface-variant flex items-center justify-center text-on-surface-variant">
<span class="material-symbols-outlined">badge</span>
</div>
<span class="font-label text-xs uppercase tracking-wider text-on-surface-variant bg-surface-container-highest px-2 py-1 rounded">ID</span>
</div>
<div>
<p class="font-headline text-2xl font-semibold text-on-surface font-mono tracking-tighter">GA-TL-0847</p>
<p class="font-body text-sm text-on-surface-variant mt-1">Issued Jun 2024</p>
</div>
</div>
</section>
<div class="grid grid-cols-1 lg:grid-cols-3 gap-10">
<!-- Primary Section: Upcoming Sessions -->
<section class="lg:col-span-2 space-y-6">
<div class="flex items-center justify-between border-b border-outline-variant pb-2">
<h3 class="font-headline text-2xl font-semibold text-on-surface">Upcoming Sessions</h3>
<a class="font-body text-sm font-medium text-primary hover:underline" href="#">View Calendar</a>
</div>
<div class="space-y-4">
<!-- Session 1 -->
<div class="surface-card p-5 flex flex-col sm:flex-row gap-5 items-start sm:items-center group hover:bg-surface-container-lowest transition-colors cursor-pointer">
<div class="bg-surface-variant p-3 rounded-lg text-center min-w-[70px]">
<span class="block font-label text-xs uppercase font-bold text-on-surface-variant">Aug</span>
<span class="block font-headline text-xl font-bold text-on-surface">10</span>
</div>
<div class="flex-1">
<div class="flex items-center gap-2 mb-1">
<span class="font-label text-[10px] uppercase tracking-widest text-primary font-bold bg-primary-container/10 px-2 py-0.5 rounded">Core</span>
<h4 class="font-body text-base font-semibold text-on-surface">Business Orientation</h4>
</div>
<div class="flex items-center gap-4 text-sm text-on-surface-variant font-body">
<span class="flex items-center gap-1"><span class="material-symbols-outlined text-[16px]">location_on</span> Lagao Hall</span>
<span class="flex items-center gap-1"><span class="material-symbols-outlined text-[16px]">schedule</span> 9:00 AM</span>
</div>
</div>
<div class="mt-4 sm:mt-0">
<button class="px-5 py-2 bg-primary-container text-on-primary rounded-lg font-body text-sm font-medium hover:bg-primary transition-colors">Attend</button>
</div>
</div>
<!-- Session 2 -->
<div class="surface-card p-5 flex flex-col sm:flex-row gap-5 items-start sm:items-center group hover:bg-surface-container-lowest transition-colors cursor-pointer border-l-4 border-l-secondary">
<div class="bg-surface-variant p-3 rounded-lg text-center min-w-[70px]">
<span class="block font-label text-xs uppercase font-bold text-on-surface-variant">Aug</span>
<span class="block font-headline text-xl font-bold text-on-surface">17</span>
</div>
<div class="flex-1">
<div class="flex items-center gap-2 mb-1">
<span class="font-label text-[10px] uppercase tracking-widest text-secondary font-bold bg-secondary/10 px-2 py-0.5 rounded">Special</span>
<h4 class="font-body text-base font-semibold text-on-surface">Ginhawa Talk</h4>
</div>
<div class="flex items-center gap-4 text-sm text-on-surface-variant font-body">
<span class="flex items-center gap-1"><span class="material-symbols-outlined text-[16px]">location_on</span> Koronadal</span>
<span class="flex items-center gap-1"><span class="material-symbols-outlined text-[16px]">schedule</span> 2:00 PM</span>
</div>
</div>
<div class="mt-4 sm:mt-0">
<button class="px-5 py-2 border border-outline text-on-surface rounded-lg font-body text-sm font-medium hover:bg-surface-variant transition-colors">Waitlist</button>
</div>
</div>
<!-- Session 3 -->
<div class="surface-card p-5 flex flex-col sm:flex-row gap-5 items-start sm:items-center opacity-70">
<div class="bg-surface-variant p-3 rounded-lg text-center min-w-[70px]">
<span class="block font-label text-xs uppercase font-bold text-on-surface-variant">Aug</span>
<span class="block font-headline text-xl font-bold text-on-surface">24</span>
</div>
<div class="flex-1">
<div class="flex items-center gap-2 mb-1">
<span class="font-label text-[10px] uppercase tracking-widest text-on-surface-variant font-bold bg-surface-variant px-2 py-0.5 rounded">Advanced</span>
<h4 class="font-body text-base font-semibold text-on-surface flex items-center gap-2">Testimonial Session <span class="material-symbols-outlined text-sm">lock</span></h4>
</div>
<div class="flex items-center gap-4 text-sm text-on-surface-variant font-body">
<span class="flex items-center gap-1"><span class="material-symbols-outlined text-[16px]">location_on</span> TBD</span>
<span class="flex items-center gap-1"><span class="material-symbols-outlined text-[16px]">schedule</span> TBD</span>
</div>
</div>
<div class="mt-4 sm:mt-0">
<span class="font-body text-xs text-on-surface-variant uppercase tracking-wider font-semibold">Locked</span>
</div>
</div>
</div>
</section>
<!-- Secondary Section: Learning Modules -->
<aside class="space-y-6">
<div class="flex items-center justify-between border-b border-outline-variant pb-2">
<h3 class="font-headline text-2xl font-semibold text-on-surface">Modules</h3>
</div>
<div class="surface-card overflow-hidden">
<ul class="divide-y divide-outline-variant">
<!-- Module 1 -->
<li class="p-4 hover:bg-surface-container-lowest transition-colors flex items-center gap-4 cursor-pointer">
<div class="w-8 h-8 rounded-full bg-secondary/20 flex items-center justify-center text-secondary">
<span class="material-symbols-outlined text-sm" style="font-variation-settings: 'FILL' 1;">check</span>
</div>
<div class="flex-1">
<h4 class="font-body text-sm font-medium text-on-surface">The Product Story</h4>
<div class="w-full bg-surface-variant h-1 mt-2 rounded-full overflow-hidden">
<div class="bg-secondary h-full w-full"></div>
</div>
</div>
</li>
<!-- Module 2 -->
<li class="p-4 hover:bg-surface-container-lowest transition-colors flex items-center gap-4 cursor-pointer bg-primary-container/5 border-l-2 border-primary">
<div class="w-8 h-8 rounded-full bg-primary-container flex items-center justify-center text-on-primary shadow-sm">
<span class="material-symbols-outlined text-sm">play_arrow</span>
</div>
<div class="flex-1">
<h4 class="font-body text-sm font-semibold text-primary">Your First Twenty Names</h4>
<div class="w-full bg-surface-variant h-1 mt-2 rounded-full overflow-hidden">
<div class="bg-primary h-full w-1/3"></div>
</div>
</div>
</li>
<!-- Module 3 -->
<li class="p-4 hover:bg-surface-container-lowest transition-colors flex items-center gap-4 cursor-pointer">
<div class="w-8 h-8 rounded-full bg-surface-variant flex items-center justify-center text-on-surface-variant">
<span class="material-symbols-outlined text-sm">play_arrow</span>
</div>
<div class="flex-1">
<h4 class="font-body text-sm font-medium text-on-surface">The Invite Conversation</h4>
<div class="w-full bg-surface-variant h-1 mt-2 rounded-full overflow-hidden">
<div class="bg-primary h-full w-0"></div>
</div>
</div>
</li>
<!-- Module 4 -->
<li class="p-4 opacity-50 flex items-center gap-4">
<div class="w-8 h-8 rounded-full bg-surface-variant flex items-center justify-center text-on-surface-variant">
<span class="material-symbols-outlined text-sm">lock</span>
</div>
<div class="flex-1">
<h4 class="font-body text-sm font-medium text-on-surface">Following Up</h4>
</div>
</li>
<!-- Module 5 -->
<li class="p-4 opacity-50 flex items-center gap-4">
<div class="w-8 h-8 rounded-full bg-surface-variant flex items-center justify-center text-on-surface-variant">
<span class="material-symbols-outlined text-sm">lock</span>
</div>
<div class="flex-1">
<h4 class="font-body text-sm font-medium text-on-surface">Leaders Training</h4>
</div>
</li>
</ul>
</div>
</aside>
</div>
</div>
</main>
</body></html>
````


---

<!-- FILE: Showcase/index.html -->
# Showcase/index.html

````html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>GutGuard Design System — Visual Showcase</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,400;0,9..144,500;0,9..144,600;1,9..144,400&family=Inter+Tight:wght@400;500;600;700;800;900&display=swap" rel="stylesheet" />
  <style>
    :root {
      --bone: #F4F1EA;
      --bone-soft: #EBE7DE;
      --bone-deep: #DDD7C8;
      --paper: #FCFAF5;
      --blue: #0608A9;
      --blue-press: #04067A;
      --gold: #B08D5B;
      --gold-soft: #C9AC7E;
      --ink: #0F0F18;
      --ink-2: #3A3A48;
      --ink-3: #6B6B7A;
      --ink-4: #A0A0AE;
      --rule: #D8D2C2;
      --rule-soft: #E5E0D2;
      --error: #B0202E;
      --error-text: #8F1824;
      --serif: "Fraunces", "Times New Roman", serif;
      --sans: "Inter Tight", system-ui, sans-serif;
      --r-sm: 10px;
      --r-md: 14px;
      --r-lg: 24px;
      --r-pill: 999px;
      --shadow-card: 0 14px 36px rgba(15, 15, 24, 0.07);
      --shadow-modal: 0 24px 80px rgba(15, 15, 24, 0.28);
      --ease: cubic-bezier(0.22, 1, 0.36, 1);
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      color: var(--ink);
      background-color: var(--bone);
      background-image: radial-gradient(circle at 1px 1px, rgba(15, 15, 24, 0.025) 1px, transparent 0);
      background-size: 3px 3px;
      font-family: var(--sans);
      font-size: 16px;
      line-height: 1.5;
      -webkit-font-smoothing: antialiased;
    }
    button, input, select, textarea { font: inherit; }
    button { cursor: pointer; border: none; background: none; color: inherit; }
    a { color: var(--blue); }
    :focus-visible { outline: 3px solid var(--gold); outline-offset: 3px; }

    /* —— layout —— */
    .frame {
      display: grid;
      grid-template-columns: 240px 1fr;
      min-height: 100vh;
    }
    .nav {
      position: sticky;
      top: 0;
      height: 100vh;
      overflow: auto;
      padding: 28px 20px 40px;
      border-right: 1px solid var(--rule);
      background: rgba(252, 250, 245, 0.92);
      backdrop-filter: blur(10px);
    }
    .nav-brand {
      display: flex;
      align-items: baseline;
      gap: 8px;
      margin-bottom: 8px;
    }
    .nav-brand strong {
      font-size: 18px;
      font-weight: 800;
      letter-spacing: -0.02em;
    }
    .nav-brand em {
      font-family: var(--serif);
      font-style: italic;
      font-size: 18px;
      color: var(--blue);
      font-weight: 400;
    }
    .nav-sub {
      font-size: 12px;
      color: var(--ink-3);
      margin-bottom: 24px;
      line-height: 1.4;
    }
    .nav a {
      display: block;
      padding: 9px 12px;
      border-radius: var(--r-sm);
      color: var(--ink-2);
      text-decoration: none;
      font-size: 13.5px;
      font-weight: 600;
    }
    .nav a:hover { color: var(--blue); background: rgba(6, 8, 169, 0.06); }
    .nav .group {
      margin-top: 18px;
      margin-bottom: 6px;
      padding: 0 12px;
      font-size: 10px;
      font-weight: 900;
      letter-spacing: 0.16em;
      text-transform: uppercase;
      color: var(--ink-3);
    }
    .main { padding: 40px 48px 96px; max-width: 1080px; }
    .hero { margin-bottom: 48px; padding-bottom: 32px; border-bottom: 1px solid var(--ink); }
    .eyebrow {
      font-size: 10px;
      font-weight: 900;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--blue);
      margin-bottom: 12px;
    }
    .hero h1 {
      font-family: var(--serif);
      font-size: clamp(40px, 6vw, 64px);
      font-weight: 400;
      letter-spacing: -0.025em;
      line-height: 0.95;
      margin-bottom: 14px;
    }
    .hero h1 em { color: var(--blue); font-style: italic; }
    .hero p { max-width: 46ch; color: var(--ink-2); font-size: 17px; line-height: 1.45; }

    .section { margin-top: 56px; scroll-margin-top: 24px; }
    .section-head {
      display: flex;
      align-items: baseline;
      justify-content: space-between;
      gap: 16px;
      margin-bottom: 18px;
      padding-bottom: 12px;
      border-bottom: 1px solid var(--rule);
    }
    .section-head h2 {
      font-family: var(--serif);
      font-size: 28px;
      font-weight: 400;
      line-height: 1;
    }
    .section-head span {
      font-size: 11px;
      font-weight: 700;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--ink-3);
    }
    .note {
      font-size: 13px;
      color: var(--ink-3);
      margin-bottom: 16px;
      max-width: 60ch;
    }

    .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
    .grid-3 { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; }
    .stack { display: flex; flex-direction: column; gap: 14px; }
    .row { display: flex; flex-wrap: wrap; gap: 12px; align-items: center; }
    .demo {
      background: var(--paper);
      border: 1px solid var(--rule);
      border-radius: var(--r-md);
      padding: 20px;
    }
    .demo--flush { padding: 0; overflow: hidden; }
    .demo-label {
      font-size: 10px;
      font-weight: 800;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--ink-3);
      margin-bottom: 12px;
    }
    .swatch-row { display: grid; grid-template-columns: repeat(auto-fill, minmax(120px, 1fr)); gap: 10px; }
    .swatch {
      border: 1px solid var(--rule);
      border-radius: var(--r-sm);
      overflow: hidden;
      background: var(--paper);
    }
    .swatch i { display: block; height: 64px; }
    .swatch b, .swatch small { display: block; padding: 8px 10px 0; font-size: 12px; }
    .swatch small { padding-bottom: 10px; color: var(--ink-3); font-family: ui-monospace, monospace; font-size: 11px; }

    /* —— components —— */
    .btn {
      min-height: 48px;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 12px;
      padding: 12px 18px;
      border-radius: var(--r-sm);
      font-weight: 800;
      transition: background .2s ease, color .2s ease, border-color .2s ease, transform .1s ease;
    }
    .btn:active:not(:disabled) { transform: scale(0.99); }
    .btn:disabled { background: var(--bone-soft) !important; color: var(--ink-4) !important; cursor: not-allowed; border-color: transparent !important; }
    .btn:focus-visible { outline: 3px solid var(--gold); outline-offset: 3px; }

    .btn-editorial {
      width: 100%;
      min-height: 62px;
      justify-content: space-between;
      border-radius: 0;
      background: var(--ink);
      color: var(--bone);
      padding: 18px 24px;
      position: relative;
      overflow: hidden;
    }
    .btn-editorial:hover:not(:disabled) { background: var(--blue); }
    .btn-editorial .main-label { font-size: 16px; font-weight: 600; }
    .btn-editorial .sub-label {
      display: block;
      font-family: var(--serif);
      font-style: italic;
      font-size: 12px;
      font-weight: 400;
      opacity: 0.7;
      margin-top: 2px;
    }
    .btn-editorial .arrow {
      width: 28px; height: 28px; border-radius: 50%;
      border: 1px solid currentColor;
      display: grid; place-items: center; flex-shrink: 0;
    }

    .btn-commerce {
      min-height: 62px;
      border-radius: var(--r-md);
      background: var(--blue);
      color: var(--bone);
      padding: 16px 20px;
      font-weight: 900;
      flex-direction: column;
      align-items: flex-start;
      gap: 2px;
    }
    .btn-commerce small {
      font-size: 13px;
      font-weight: 700;
      color: rgba(244, 241, 234, 0.76);
    }
    .btn-commerce:hover:not(:disabled) { background: var(--blue-press); }

    .btn-partner {
      min-height: 48px;
      border-radius: 10px;
      background: var(--blue);
      color: var(--bone);
      font-weight: 700;
      padding: 0 20px;
    }
    .btn-partner:hover:not(:disabled) { background: var(--blue-press); }

    .btn-secondary {
      border: 1px solid var(--rule);
      background: rgba(252, 250, 245, 0.72);
      color: var(--ink);
      font-size: 11px;
      font-weight: 900;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      border-radius: var(--r-sm);
    }
    .btn-secondary.square { border-radius: 0; }
    .btn-secondary:hover:not(:disabled) { border-color: var(--blue); color: var(--blue); }

    .btn-text {
      color: var(--blue);
      font-size: 13px;
      font-weight: 700;
      text-decoration: underline;
      text-underline-offset: 3px;
      min-height: 44px;
      padding: 10px 4px;
    }
    .btn-icon {
      width: 44px; height: 44px;
      border: 1px solid var(--rule);
      background: var(--paper);
      border-radius: var(--r-sm);
      display: grid; place-items: center;
      color: var(--ink);
      flex-shrink: 0;
    }
    .btn-icon:hover:not(:disabled) { border-color: var(--blue); color: var(--blue); }
    .btn-icon:disabled { color: var(--ink-4); cursor: not-allowed; }
    .btn-icon.dense { width: 36px; height: 36px; }
    .btn-icon.ghost { border-color: transparent; background: transparent; }
    .btn-icon.square { border-radius: 0; }
    .btn-icon svg,
    .icon {
      width: 20px;
      height: 20px;
      stroke: currentColor;
      fill: none;
      stroke-width: 2;
      stroke-linecap: round;
      stroke-linejoin: round;
    }

    .field { display: grid; gap: 7px; }
    .field-label {
      color: var(--ink-3);
      font-size: 10px;
      font-weight: 900;
      letter-spacing: 0.14em;
      text-transform: uppercase;
    }
    .field-label.editorial {
      font-family: var(--serif);
      font-style: italic;
      font-size: 14px;
      font-weight: 400;
      letter-spacing: 0;
      text-transform: none;
    }
    .field-control {
      width: 100%;
      min-height: 48px;
      border: 1px solid var(--rule);
      border-radius: var(--r-sm);
      background: var(--bone);
      padding: 12px 14px;
      color: var(--ink);
      outline: none;
    }
    .field-control:focus {
      border-color: var(--blue);
      box-shadow: 0 0 0 3px rgba(6, 8, 169, 0.14);
      outline: none;
    }
    .field-control.error { border-color: var(--error); box-shadow: none; }
    .field-error { color: var(--error); font-size: 12px; font-weight: 800; }
    .field-ruled {
      border: none;
      border-radius: 0;
      background: transparent;
      border-bottom: 1px solid var(--rule);
      padding: 14px 0;
      min-height: auto;
    }
    .field-ruled:focus {
      box-shadow: none;
      border-bottom-color: var(--blue);
    }
    .field.ruled:focus-within .field-label { color: var(--blue); }

    .segment {
      display: inline-grid;
      grid-auto-flow: column;
      gap: 4px;
      padding: 4px;
      border: 1px solid var(--rule);
      border-radius: var(--r-md);
      background: var(--bone-soft);
    }
    .segment button {
      min-height: 44px;
      padding: 0 16px;
      border-radius: var(--r-sm);
      font-size: 12px;
      font-weight: 800;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--ink-3);
    }
    .segment button.on {
      background: var(--paper);
      color: var(--ink);
      box-shadow: 0 2px 7px rgba(15, 15, 24, 0.09);
    }
    .segment.blue button.on {
      background: var(--blue);
      color: var(--bone);
      box-shadow: none;
    }

    .tabs {
      display: flex;
      gap: 8px;
      border-bottom: 1px solid var(--rule);
    }
    .tabs button {
      min-height: 42px;
      padding: 12px 18px;
      font-size: 11px;
      font-weight: 800;
      letter-spacing: 0.16em;
      text-transform: uppercase;
      color: var(--ink-3);
      border-bottom: 2px solid transparent;
    }
    .tabs button:hover,
    .tabs button.on {
      background: var(--blue);
      color: var(--bone);
      border-bottom-color: var(--blue);
    }

    .topbar {
      display: grid;
      grid-template-columns: 1fr auto 1fr;
      align-items: center;
      gap: 20px;
      padding: 12px 24px;
      background: rgba(244, 241, 234, 0.96);
      border-bottom: 1px solid rgba(15, 15, 24, 0.08);
      box-shadow: 0 5px 14px rgba(15, 15, 24, 0.04);
      position: relative;
    }
    .topbar::before {
      content: "";
      position: absolute;
      inset: 0 0 auto;
      height: 2px;
      background: linear-gradient(90deg, #B5431F, var(--gold), #1E6FB8);
    }
    .topbar .brand { font-weight: 800; font-size: 15px; }
    .topbar .brand em { font-family: var(--serif); font-style: italic; color: var(--blue); font-weight: 400; }
    .topbar nav { display: flex; gap: 20px; justify-content: center; }
    .topbar nav a {
      color: var(--ink-2);
      text-decoration: none;
      font-size: 14px;
      font-weight: 600;
      min-height: 44px;
      display: inline-flex;
      align-items: center;
      position: relative;
    }
    .topbar nav a:hover,
    .topbar nav a[aria-current="page"] { color: var(--blue); }
    .topbar nav a[aria-current="page"]::after {
      content: "";
      position: absolute;
      left: 0; right: 0; bottom: 8px;
      height: 2px;
      background: var(--blue);
      border-radius: 2px;
    }
    .topbar .actions { display: flex; gap: 10px; justify-content: flex-end; align-items: center; }

    .shell-demo {
      display: grid;
      grid-template-columns: 220px 1fr;
      border: 1px solid var(--rule);
      border-radius: var(--r-md);
      overflow: hidden;
      min-height: 280px;
      background: var(--bone);
    }
    .side {
      background: var(--paper);
      border-right: 1px solid var(--rule);
      padding: 18px 14px;
      display: flex;
      flex-direction: column;
      gap: 6px;
    }
    .side .side-brand {
      display: flex;
      align-items: baseline;
      gap: 6px;
      padding: 0 10px 14px;
      font-weight: 800;
    }
    .side .side-brand em { font-family: var(--serif); font-style: italic; color: var(--blue); font-weight: 400; }
    .side button {
      display: flex;
      align-items: center;
      gap: 8px;
      width: 100%;
      min-height: 44px;
      padding: 0 12px;
      border-radius: var(--r-sm);
      text-align: left;
      font-size: 14px;
      font-weight: 600;
      color: var(--ink);
    }
    .side button.on {
      background: rgba(6, 8, 169, 0.07);
      color: var(--blue);
      font-weight: 700;
    }
    .side .btn-partner,
    .side .btn-partner:hover:not(:disabled) {
      justify-content: center;
      color: var(--bone);
      font-weight: 700;
    }
    .side .side-foot {
      margin-top: auto;
      border: 1px solid var(--rule);
      border-radius: var(--r-md);
      padding: 12px;
      background: var(--bone);
    }
    .side .side-foot b { display: block; font-size: 13px; margin-bottom: 8px; }
    .shell-main { padding: 18px; position: relative; }
    .bottom-bar {
      position: absolute;
      left: 0; right: 0; bottom: 0;
      background: var(--paper);
      border-top: 1px solid var(--rule);
      padding: 12px 16px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      box-shadow: 0 -6px 24px rgba(15, 15, 24, 0.08);
    }
    .bottom-bar .eye {
      font-size: 10px;
      font-weight: 800;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--ink-3);
    }
    .bottom-bar .title { font-size: 15px; font-weight: 700; }

    .masthead {
      display: flex;
      align-items: flex-end;
      justify-content: space-between;
      gap: 16px;
      padding: 8px 0 4px;
    }
    .mast-logos { display: flex; align-items: center; gap: 10px; }
    .mast-mark {
      width: 36px; height: 40px;
      background: var(--ink);
      color: var(--bone);
      display: grid; place-items: center;
      font-size: 11px; font-weight: 900;
    }
    .mast-mark.alt { background: var(--blue); }
    .mast-x { color: var(--ink-3); font-weight: 700; }
    .mast-text .name { font-size: 14px; font-weight: 800; }
    .mast-text .ed { font-size: 11px; color: var(--ink-3); }

    .card {
      background: var(--paper);
      border: 1px solid var(--rule);
      border-radius: var(--r-md);
      padding: 18px;
      box-shadow: var(--shadow-card);
    }
    .card.editorial {
      border-radius: 0;
      background: var(--bone);
      box-shadow: none;
    }
    .card.auth { border-top: 3px solid var(--blue); }
    .card h3 { font-family: var(--serif); font-size: 22px; font-weight: 400; line-height: 1.05; margin: 6px 0 8px; }
    .card p { color: var(--ink-3); font-size: 14px; }

    .badge {
      display: inline-flex;
      align-items: center;
      min-height: 24px;
      padding: 4px 10px;
      border: 1px solid var(--rule);
      border-radius: var(--r-pill);
      font-size: 10px;
      font-weight: 900;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--ink-3);
    }
    .badge.paid {
      border-color: rgba(6, 8, 169, 0.32);
      color: var(--blue);
    }

    .alert {
      border: 1px solid var(--rule);
      background: rgba(235, 231, 222, 0.66);
      padding: 13px 15px;
      border-radius: var(--r-md);
      color: var(--blue);
      font-weight: 700;
      font-size: 14px;
    }
    .alert.error {
      border-color: rgba(176, 32, 46, 0.32);
      background: rgba(176, 32, 46, 0.07);
      color: var(--error-text);
    }
    .alert.error .t {
      display: block;
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 0.16em;
      text-transform: uppercase;
      color: var(--error);
      margin-bottom: 4px;
    }

    .toast {
      background: var(--ink);
      color: var(--bone);
      border: 1px solid rgba(6, 8, 169, 0.35);
      padding: 16px;
      box-shadow: 0 20px 48px rgba(15, 15, 24, 0.28);
      max-width: 340px;
    }
    .toast .t {
      font-size: 12px;
      font-weight: 800;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: #EAFF18;
      margin-bottom: 6px;
    }
    .toast .t.err { color: #FFB8C2; }
    .toast p { font-size: 14px; font-weight: 700; line-height: 1.35; }

    .modal-demo {
      background: rgba(15, 15, 24, 0.58);
      border-radius: var(--r-md);
      padding: 28px 20px;
      display: grid;
      place-items: center;
      min-height: 260px;
    }
    .modal {
      width: min(100%, 380px);
      background: var(--paper);
      border: 1px solid var(--rule);
      border-radius: var(--r-lg);
      padding: 20px;
      box-shadow: var(--shadow-modal);
    }
    .modal.square { border-radius: 0; }
    .modal h3 { font-family: var(--serif); font-size: 28px; font-weight: 400; line-height: 1; margin-bottom: 10px; }
    .modal p { color: var(--ink-2); font-size: 14px; margin-bottom: 16px; }
    .modal .actions { display: flex; gap: 10px; justify-content: flex-end; }

    .dialog {
      display: flex;
      flex-direction: column;
      width: min(100%, 440px);
      background: var(--paper);
      border: 1px solid var(--rule);
      border-radius: var(--r-lg);
      box-shadow: var(--shadow-modal);
      overflow: hidden;
    }
    .dialog.square { border-radius: 0; }
    .dialog-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      padding: 16px 18px;
      border-bottom: 1px solid var(--rule);
    }
    .dialog-header h3 {
      margin: 0;
      font-family: var(--serif);
      font-size: 26px;
      font-weight: 400;
      line-height: 1.1;
      letter-spacing: -0.02em;
    }
    .dialog-body {
      padding: 18px;
      color: var(--ink-2);
      font-size: 14px;
      line-height: 1.5;
    }
    .dialog-footer {
      display: flex;
      justify-content: flex-end;
      gap: 10px;
      padding: 14px 18px;
      border-top: 1px solid var(--rule);
    }

    .switch {
      position: relative;
      width: 44px;
      height: 26px;
      border: 0;
      border-radius: var(--r-pill);
      background: var(--bone-deep);
      cursor: pointer;
      flex-shrink: 0;
      transition: background 0.18s var(--ease);
    }
    .switch::after {
      content: "";
      position: absolute;
      top: 3px;
      left: 3px;
      width: 20px;
      height: 20px;
      border-radius: 50%;
      background: var(--paper);
      box-shadow: 0 1px 3px rgba(15, 15, 24, 0.18);
      transition: transform 0.18s var(--ease);
    }
    .switch[aria-checked="true"] { background: var(--blue); }
    .switch[aria-checked="true"]::after { transform: translateX(18px); }
    .switch-row {
      display: inline-flex;
      align-items: center;
      gap: 12px;
      font-size: 14px;
      font-weight: 600;
    }

    .drawer-demo {
      display: grid;
      grid-template-columns: 1fr 280px;
      min-height: 240px;
      border: 1px solid var(--rule);
      border-radius: var(--r-md);
      overflow: hidden;
    }
    .drawer-scrim { background: rgba(15, 15, 24, 0.35); }
    .drawer {
      background: var(--paper);
      border-left: 1px solid var(--rule);
      padding: 18px;
      box-shadow: -22px 0 70px rgba(15, 15, 24, 0.22);
    }
    .drawer h3 { font-family: var(--serif); font-size: 24px; font-weight: 400; margin-bottom: 8px; }

    .table-wrap { overflow: auto; border: 1px solid var(--rule); border-radius: var(--r-md); background: var(--paper); }
    table { width: 100%; border-collapse: collapse; }
    th {
      text-align: left;
      font-size: 10px;
      font-weight: 900;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--ink-3);
      padding: 12px 14px;
      border-bottom: 1px solid var(--rule);
      background: var(--bone);
    }
    td {
      padding: 14px;
      border-bottom: 1px solid var(--rule-soft);
      font-size: 14px;
      vertical-align: middle;
    }
    tr:last-child td { border-bottom: none; }

    .deflist { border-top: 1px solid var(--rule); }
    .deflist div {
      display: grid;
      grid-template-columns: 140px 1fr;
      gap: 12px;
      padding: 12px 0;
      border-bottom: 1px solid var(--rule);
    }
    .deflist dt {
      font-family: var(--serif);
      font-style: italic;
      color: var(--ink-3);
      font-size: 14px;
    }
    .deflist dd { font-weight: 600; }

    .qr {
      width: 140px;
      background: #fff;
      border: 1px solid var(--rule);
      border-radius: var(--r-md);
      padding: 10px;
    }
    .qr-grid {
      display: grid;
      grid-template-columns: repeat(7, 1fr);
      gap: 3px;
      aspect-ratio: 1;
    }
    .qr-grid i { background: var(--ink); aspect-ratio: 1; }
    .qr-grid i.off { background: transparent; }

    .rail {
      display: flex;
      align-items: center;
      gap: 0;
      padding: 8px 0;
    }
    .rail .dot {
      width: 12px; height: 12px;
      border-radius: 50%;
      border: 2px solid var(--rule);
      background: var(--paper);
      z-index: 1;
    }
    .rail .dot.done { background: var(--blue); border-color: var(--blue); }
    .rail .dot.active { border-color: var(--blue); box-shadow: 0 0 0 3px rgba(6, 8, 169, 0.16); }
    .rail .seg {
      flex: 1;
      height: 3px;
      background: var(--rule-soft);
    }
    .rail .seg.done { background: var(--blue); }

    .section-label {
      display: flex;
      align-items: center;
      gap: 10px;
      margin-bottom: 8px;
    }
    .section-label i {
      width: 24px; height: 1px; background: var(--ink); display: block;
    }
    .section-label .num {
      font-family: var(--serif);
      font-style: italic;
      color: var(--blue);
      font-size: 14px;
    }
    .section-label .lab {
      font-size: 10px;
      font-weight: 800;
      letter-spacing: 0.16em;
      text-transform: uppercase;
      color: var(--ink-3);
    }

    .task {
      display: flex;
      align-items: center;
      gap: 14px;
      padding: 14px 0;
      border-bottom: 1px solid var(--rule);
    }
    .task .num {
      width: 28px; height: 28px;
      border-radius: 50%;
      border: 1px solid var(--rule);
      display: grid; place-items: center;
      font-size: 12px; font-weight: 700;
      color: var(--ink-3);
    }
    .task.done .num {
      background: var(--blue);
      border-color: var(--blue);
      color: var(--bone);
    }
    .task .meta { color: var(--ink-3); font-size: 13px; }
    .task .chev {
      margin-left: auto;
      color: var(--ink-3);
      display: inline-grid;
      place-items: center;
    }
    .task .chev svg { width: 18px; height: 18px; }

    .empty {
      border: 1px dashed var(--rule);
      background: var(--bone);
      padding: 22px;
      text-align: center;
    }
    .empty b { display: block; margin-bottom: 4px; }
    .empty span { color: var(--ink-3); font-size: 13px; }

    /* —— File attachment (custom UI; native input hidden) —— */
    .file-attach { position: relative; }
    .file-attach__input {
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
    .upload {
      display: block;
      border: 1.5px dashed var(--rule);
      border-radius: var(--r-md);
      background: var(--bone);
      padding: 22px 18px;
      text-align: center;
      cursor: pointer;
      transition: border-color .15s ease, background .15s ease, color .15s ease;
    }
    .upload:hover,
    .upload.drag,
    .file-attach:focus-within .upload:not(.has-error) {
      border-color: var(--blue);
      background: rgba(6, 8, 169, 0.04);
    }
    .upload.has-error {
      border-color: var(--error);
      background: rgba(176, 32, 46, 0.05);
    }
    .upload .up-ico {
      display: inline-grid;
      place-items: center;
      width: 44px;
      height: 44px;
      margin: 0 auto 10px;
      border-radius: var(--r-sm);
      border: 1px solid var(--rule);
      background: var(--paper);
      color: var(--ink-3);
    }
    .upload:hover .up-ico,
    .upload.drag .up-ico { color: var(--blue); border-color: var(--blue); }
    .upload .up-ico svg { width: 22px; height: 22px; }
    .upload b { display: block; margin-bottom: 4px; font-size: 15px; }
    .upload .hint { display: block; color: var(--ink-3); font-size: 13px; margin-bottom: 14px; }
    .upload.has-error .hint { color: var(--error-text); }
    .upload .btn { pointer-events: none; }
    .file-row {
      display: flex;
      align-items: center;
      gap: 12px;
      padding: 12px 14px;
      border: 1px solid var(--rule);
      border-radius: var(--r-sm);
      background: var(--paper);
      text-align: left;
    }
    .file-row.has-error { border-color: var(--error); }
    .file-row .ico {
      width: 36px; height: 36px;
      border-radius: 8px;
      background: rgba(6, 8, 169, 0.08);
      color: var(--blue);
      display: grid; place-items: center;
      font-size: 11px; font-weight: 800;
      letter-spacing: 0.04em;
      flex-shrink: 0;
    }
    .file-row .ico svg { width: 18px; height: 18px; }
    .file-row .name { font-weight: 700; font-size: 14px; }
    .file-row .meta { font-size: 12px; color: var(--ink-3); }
    .file-row.has-error .meta { color: var(--error-text); }
    .file-row .rm { margin-left: auto; }
    .file-progress {
      margin-top: 10px;
      height: 6px;
      border-radius: var(--r-pill);
      background: var(--bone-soft);
      overflow: hidden;
    }
    .file-progress > i {
      display: block;
      height: 100%;
      width: 62%;
      background: var(--blue);
      border-radius: inherit;
    }
    .file-compact {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      flex-wrap: wrap;
    }
    .file-compact .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
    }

    .avatar {
      width: 40px; height: 40px;
      border-radius: 50%;
      background: var(--bone-soft);
      color: var(--blue);
      display: grid; place-items: center;
      font-weight: 800;
      font-size: 13px;
      border: 1px solid var(--rule);
      overflow: hidden;
      flex-shrink: 0;
    }
    .avatar.lg { width: 56px; height: 56px; font-size: 18px; }
    .avatar.sm { width: 32px; height: 32px; font-size: 11px; }
    .avatar.blue { background: rgba(6, 8, 169, 0.1); border-color: transparent; }
    .avatar-row { display: flex; align-items: center; gap: 12px; }
    .avatar-row b { display: block; font-size: 14px; }
    .avatar-row span { font-size: 13px; color: var(--ink-3); }

    .search {
      position: relative;
      display: flex;
      align-items: center;
    }
    .search .ico {
      position: absolute;
      left: 14px;
      color: var(--ink-3);
      font-size: 14px;
      pointer-events: none;
    }
    .search input {
      width: 100%;
      min-height: 48px;
      padding: 12px 40px 12px 40px;
      border: 1px solid var(--rule);
      border-radius: var(--r-sm);
      background: var(--bone);
      outline: none;
    }
    .search input::-webkit-search-decoration,
    .search input::-webkit-search-cancel-button,
    .search input::-webkit-search-results-button,
    .search input::-webkit-search-results-decoration {
      -webkit-appearance: none;
      appearance: none;
      display: none;
    }
    .search input:focus {
      border-color: var(--blue);
      box-shadow: 0 0 0 3px rgba(6, 8, 169, 0.14);
    }
    .search .clear {
      position: absolute;
      right: 8px;
      width: 32px; height: 32px;
      border-radius: 8px;
      color: var(--ink-3);
      display: grid;
      place-items: center;
    }
    .search .clear svg { width: 16px; height: 16px; }
    .search .clear:hover { color: var(--ink); background: var(--bone-soft); }

    .stepper {
      display: inline-grid;
      grid-template-columns: 36px 40px 36px;
      align-items: stretch;
    }
    .stepper button {
      min-height: 36px;
      background: var(--bone);
      border: 1px solid var(--rule);
      font-weight: 900;
      font-size: 16px;
    }
    .stepper button:first-child { border-radius: var(--r-sm) 0 0 var(--r-sm); }
    .stepper button:last-child { border-radius: 0 var(--r-sm) var(--r-sm) 0; }
    .stepper button:hover:not(:disabled) { color: var(--blue); border-color: var(--blue); }
    .stepper button:disabled { color: var(--ink-4); cursor: not-allowed; }
    .stepper .val {
      display: grid; place-items: center;
      border-top: 1px solid var(--rule);
      border-bottom: 1px solid var(--rule);
      font-weight: 700;
      background: var(--paper);
    }

    .pagination {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      padding: 12px 0;
    }
    .pagination .meta { font-size: 13px; color: var(--ink-3); }
    .pagination .controls { display: flex; align-items: center; gap: 8px; }
    .pagination select {
      min-height: 40px;
      border: 1px solid var(--rule);
      background: var(--bone);
      padding: 0 10px;
      font-weight: 600;
    }

    .menu-wrap { position: relative; display: inline-block; }
    .menu {
      position: absolute;
      right: 0; top: calc(100% + 6px);
      min-width: 180px;
      background: var(--paper);
      border: 1px solid var(--rule);
      border-radius: var(--r-sm);
      box-shadow: var(--shadow-card);
      padding: 6px;
      z-index: 5;
    }
    .menu button {
      display: block;
      width: 100%;
      text-align: left;
      min-height: 44px;
      padding: 0 12px;
      border-radius: 8px;
      font-size: 14px;
      font-weight: 600;
    }
    .menu button:hover, .menu button:focus-visible {
      background: rgba(6, 8, 169, 0.07);
      color: var(--blue);
      outline: none;
    }
    .menu button.danger { color: var(--error); }
    .menu button.danger:hover { background: rgba(176, 32, 46, 0.08); color: var(--error); }
    .menu hr { border: none; border-top: 1px solid var(--rule-soft); margin: 6px 0; }

    .tip-wrap { position: relative; display: inline-flex; }
    .tip {
      position: absolute;
      left: 50%; bottom: calc(100% + 10px);
      transform: translateX(-50%);
      background: var(--ink);
      color: var(--bone);
      font-size: 12px;
      font-weight: 600;
      padding: 8px 10px;
      border-radius: 8px;
      white-space: nowrap;
      box-shadow: var(--shadow-card);
      pointer-events: none;
      opacity: 0;
      transition: opacity .15s ease;
    }
    .tip-wrap:hover .tip, .tip-wrap:focus-within .tip { opacity: 1; }
    .tip::after {
      content: "";
      position: absolute;
      left: 50%; top: 100%;
      transform: translateX(-50%);
      border: 6px solid transparent;
      border-top-color: var(--ink);
    }

    .spinner {
      width: 22px; height: 22px;
      border: 2px solid var(--rule);
      border-top-color: var(--blue);
      border-radius: 50%;
      animation: spin .8s linear infinite;
      display: inline-block;
    }
    .spinner.lg { width: 36px; height: 36px; border-width: 3px; }
    .spinner.on-dark { border-color: rgba(244,241,234,.25); border-top-color: var(--bone); }
    @keyframes spin { to { transform: rotate(360deg); } }

    .skeleton {
      background: linear-gradient(90deg, var(--bone-soft), var(--bone-deep), var(--bone-soft));
      background-size: 200% 100%;
      animation: shimmer 1.4s ease-in-out infinite;
      border-radius: 8px;
    }
    .skeleton.line { height: 12px; margin-bottom: 10px; }
    .skeleton.line.short { width: 55%; }
    .skeleton.avatar { width: 40px; height: 40px; border-radius: 50%; }
    .skeleton.block { height: 88px; border-radius: var(--r-md); }
    @keyframes shimmer {
      0% { background-position: 100% 0; }
      100% { background-position: -100% 0; }
    }

    .accordion { border: 1px solid var(--rule); border-radius: var(--r-md); overflow: hidden; background: var(--paper); }
    .acc-item + .acc-item { border-top: 1px solid var(--rule); }
    .acc-head {
      width: 100%;
      min-height: 52px;
      padding: 12px 16px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      font-weight: 700;
      text-align: left;
    }
    .acc-head:hover { color: var(--blue); }
    .acc-head .chev {
      display: inline-grid;
      place-items: center;
      color: var(--ink-3);
      transition: transform .2s ease, color .2s ease;
      flex-shrink: 0;
    }
    .acc-head .chev svg { width: 20px; height: 20px; }
    .acc-item.open .acc-head .chev { transform: rotate(180deg); color: var(--blue); }
    .acc-body {
      display: none;
      padding: 0 16px 16px;
      color: var(--ink-2);
      font-size: 14px;
      line-height: 1.5;
    }
    .acc-item.open .acc-body { display: block; }

    .crumbs {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 8px;
      font-size: 13px;
      font-weight: 600;
    }
    .crumbs a { color: var(--ink-3); text-decoration: none; }
    .crumbs a:hover { color: var(--blue); }
    .crumbs .sep { color: var(--ink-4); }
    .crumbs .cur { color: var(--ink); }

    .datepicker {
      width: min(100%, 280px);
      background: var(--paper);
      border: 1px solid var(--rule);
      border-radius: var(--r-md);
      padding: 14px;
      box-shadow: var(--shadow-card);
    }
    .dp-head {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 12px;
      font-weight: 800;
    }
    .dp-grid {
      display: grid;
      grid-template-columns: repeat(7, 1fr);
      gap: 4px;
      text-align: center;
    }
    .dp-grid .dow {
      font-size: 10px;
      font-weight: 800;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      color: var(--ink-3);
      padding: 6px 0;
    }
    .dp-grid button {
      aspect-ratio: 1;
      border-radius: 8px;
      font-size: 13px;
      font-weight: 600;
      color: var(--ink);
    }
    .dp-grid button:hover { background: var(--bone-soft); }
    .dp-grid button.today { box-shadow: inset 0 0 0 1.5px var(--blue); }
    .dp-grid button.on { background: var(--blue); color: var(--bone); }
    .dp-grid button.mute { color: var(--ink-4); }

    .bell-wrap { position: relative; display: inline-flex; }
    .bell-btn {
      width: 44px; height: 44px;
      border: 1px solid var(--rule);
      border-radius: var(--r-sm);
      background: var(--paper);
      display: grid; place-items: center;
      font-size: 18px;
    }
    .bell-btn:hover { border-color: var(--blue); color: var(--blue); }
    .bell-count {
      position: absolute;
      top: -4px; right: -4px;
      min-width: 18px; height: 18px;
      padding: 0 5px;
      border-radius: var(--r-pill);
      background: var(--blue);
      color: var(--bone);
      font-size: 10px;
      font-weight: 900;
      display: grid; place-items: center;
    }
    .bell-panel {
      position: absolute;
      right: 0; top: calc(100% + 8px);
      width: 280px;
      background: var(--paper);
      border: 1px solid var(--rule);
      border-radius: var(--r-md);
      box-shadow: var(--shadow-card);
      overflow: hidden;
      z-index: 6;
    }
    .bell-panel .ph {
      padding: 12px 14px;
      border-bottom: 1px solid var(--rule);
      font-size: 11px;
      font-weight: 900;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--ink-3);
    }
    .bell-item {
      display: block;
      width: 100%;
      text-align: left;
      padding: 12px 14px;
      border-bottom: 1px solid var(--rule-soft);
    }
    .bell-item:hover { background: rgba(6, 8, 169, 0.05); }
    .bell-item.unread { background: rgba(6, 8, 169, 0.06); }
    .bell-item b { display: block; font-size: 13px; margin-bottom: 2px; }
    .bell-item span { font-size: 12px; color: var(--ink-3); }

    .chat-row {
      display: flex;
      align-items: center;
      gap: 12px;
      width: 100%;
      padding: 14px;
      border: 1px solid var(--rule);
      border-radius: var(--r-md);
      background: var(--paper);
      text-align: left;
    }
    .chat-row:hover { border-color: var(--blue); }
    .chat-tile {
      width: 42px; height: 42px;
      border-radius: 12px;
      background: #1373a2;
      color: #fff;
      display: grid; place-items: center;
      font-weight: 800;
      font-size: 12px;
      flex-shrink: 0;
    }
    .chat-row b { display: block; font-size: 15px; font-weight: 700; }
    .chat-row em { display: block; font-style: normal; font-size: 13px; color: var(--ink-3); margin-top: 2px; }
    .chat-row .go { margin-left: auto; color: var(--ink-3); font-weight: 700; }

    @media (prefers-reduced-motion: reduce) {
      .spinner, .skeleton { animation: none !important; }
    }

    .admin-hero {
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      gap: 20px;
      padding-bottom: 20px;
      border-bottom: 1px solid var(--ink);
      margin-bottom: 16px;
    }
    .admin-hero .kicker {
      font-size: 10px;
      font-weight: 700;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--ink-3);
      margin-bottom: 8px;
    }
    .admin-hero h3 {
      font-family: var(--serif);
      font-size: clamp(36px, 5vw, 52px);
      font-weight: 400;
      line-height: 0.95;
    }
    .admin-summary {
      border: 1px solid var(--rule);
      padding: 14px 16px;
      text-align: right;
      min-width: 120px;
      color: var(--ink-3);
      font-size: 12px;
    }
    .admin-summary strong {
      display: block;
      font-family: var(--serif);
      font-size: 36px;
      font-weight: 400;
      color: var(--blue);
      line-height: 1;
    }

    .type-sample { margin-bottom: 18px; }
    .type-sample .display {
      font-family: var(--serif);
      font-size: clamp(36px, 5vw, 56px);
      line-height: 0.95;
      letter-spacing: -0.025em;
    }
    .type-sample .display em { color: var(--blue); font-style: italic; }
    .type-sample .ui { font-size: 16px; color: var(--ink-2); margin-top: 8px; }
    .type-meta { font-size: 12px; color: var(--ink-3); margin-top: 4px; }

    .dialect-pills { display: flex; gap: 8px; flex-wrap: wrap; margin-top: 16px; }
    .dialect-pills span {
      border: 1px solid var(--rule);
      border-radius: var(--r-pill);
      padding: 6px 12px;
      font-size: 11px;
      font-weight: 800;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--ink-3);
    }

    @media (max-width: 900px) {
      .frame { grid-template-columns: 1fr; }
      .nav {
        position: relative;
        height: auto;
        border-right: none;
        border-bottom: 1px solid var(--rule);
      }
      .nav .links { display: flex; flex-wrap: wrap; gap: 4px; }
      .nav .group { width: 100%; }
      .main { padding: 28px 18px 80px; }
      .grid-2, .grid-3, .shell-demo, .drawer-demo { grid-template-columns: 1fr; }
      .topbar { grid-template-columns: 1fr; }
      .topbar nav, .topbar .actions { justify-content: flex-start; }
    }

    @media (prefers-reduced-motion: reduce) {
      * { transition: none !important; animation: none !important; }
    }
  </style>
</head>
<body>
  <div class="frame">
    <aside class="nav">
      <div class="nav-brand"><strong>GutGuard</strong><em>DS</em></div>
      <p class="nav-sub">Visual showcase · Doctors look · open in a browser</p>
      <div class="group">Foundations</div>
      <div class="links">
        <a href="#foundations">Color &amp; type</a>
      </div>
      <div class="group">Actions</div>
      <div class="links">
        <a href="#buttons">Buttons</a>
        <a href="#icon-button">Icon button</a>
        <a href="#fields">Form fields</a>
        <a href="#segment">Segmented</a>
        <a href="#switch">Switch</a>
        <a href="#tabs">Tabs</a>
      </div>
      <div class="group">Shell</div>
      <div class="links">
        <a href="#topbar">Top bar</a>
        <a href="#sidebar">Sidebar + bottom bar</a>
        <a href="#masthead">Masthead</a>
        <a href="#admin">Admin shell</a>
      </div>
      <div class="group">Surfaces</div>
      <div class="links">
        <a href="#cards">Cards</a>
        <a href="#feedback">Badge · Alert · Toast</a>
        <a href="#dialog">Dialog</a>
        <a href="#modal">Modal · Drawer</a>
      </div>
      <div class="group">Data</div>
      <div class="links">
        <a href="#table">Table</a>
        <a href="#deflist">Definition list</a>
        <a href="#qr">QR · Progress · Tasks</a>
        <a href="#empty">Empty state</a>
      </div>
      <div class="group">Utilities</div>
      <div class="links">
        <a href="#file">File attachment</a>
        <a href="#avatar">Avatar</a>
        <a href="#search">Search</a>
        <a href="#stepper">Quantity stepper</a>
        <a href="#pagination">Pagination</a>
        <a href="#dropdown">Dropdown menu</a>
        <a href="#tooltip">Tooltip</a>
        <a href="#spinner">Spinner · Skeleton</a>
      </div>
      <div class="group">Extended</div>
      <div class="links">
        <a href="#accordion">Accordion</a>
        <a href="#breadcrumbs">Breadcrumbs</a>
        <a href="#datepicker">Date picker</a>
        <a href="#notify">Notification bell</a>
        <a href="#chatrow">Chat link row</a>
      </div>
    </aside>

    <main class="main">
      <header class="hero">
        <div class="eyebrow">GutGuard Design System</div>
        <h1>Visual <em>component</em> showcase</h1>
        <p>Every skin below follows GutGuard Doctors: bone canvas, ultramarine actions, Fraunces + Inter Tight. Prototypes supply structure only — this is how components should look.</p>
        <div class="dialect-pills">
          <span>Editorial · square</span>
          <span>Commerce · soft radius</span>
          <span>Admin · dense square</span>
        </div>
      </header>

      <!-- Foundations -->
      <section class="section" id="foundations">
        <div class="section-head"><h2>Foundations</h2><span>Tokens</span></div>
        <p class="note">Recognition cues shared by every product.</p>
        <div class="swatch-row">
          <div class="swatch"><i style="background:#F4F1EA"></i><b>Bone</b><small>#F4F1EA</small></div>
          <div class="swatch"><i style="background:#FCFAF5;border-bottom:1px solid #D8D2C2"></i><b>Paper</b><small>#FCFAF5</small></div>
          <div class="swatch"><i style="background:#0608A9"></i><b>Blue</b><small>#0608A9</small></div>
          <div class="swatch"><i style="background:#0F0F18"></i><b>Ink</b><small>#0F0F18</small></div>
          <div class="swatch"><i style="background:#B08D5B"></i><b>Gold</b><small>#B08D5B</small></div>
          <div class="swatch"><i style="background:#D8D2C2"></i><b>Rule</b><small>#D8D2C2</small></div>
          <div class="swatch"><i style="background:#B0202E"></i><b>Error</b><small>#B0202E</small></div>
          <div class="swatch"><i style="background:#EBE7DE"></i><b>Bone soft</b><small>#EBE7DE</small></div>
        </div>
        <div class="demo" style="margin-top:16px">
          <div class="type-sample">
            <div class="display">Clinical meets <em>editorial</em></div>
            <div class="ui">Inter Tight body — 16px / 1.5 for interface reading and controls.</div>
            <div class="type-meta">Fraunces 400 display · Inter Tight UI · gold focus rings</div>
          </div>
        </div>
      </section>

      <!-- Buttons -->
      <section class="section" id="buttons">
        <div class="section-head"><h2>Buttons</h2><span>Actions</span></div>
        <div class="grid-2">
          <div class="demo">
            <div class="demo-label">Editorial primary</div>
            <button class="btn btn-editorial">
              <span><span class="main-label">Continue registration</span><span class="sub-label">Takes about two minutes</span></span>
              <span class="arrow" aria-hidden="true">→</span>
            </button>
          </div>
          <div class="demo">
            <div class="demo-label">Commerce primary</div>
            <button class="btn btn-commerce" style="width:100%">
              Place order
              <small>Ships in 2–3 business days</small>
            </button>
          </div>
          <div class="demo">
            <div class="demo-label">Partner · secondary · text · icon</div>
            <div class="row">
              <button class="btn btn-partner">Sign in</button>
              <button class="btn btn-secondary">Learn more</button>
              <button class="btn btn-text">Resend code</button>
              <button class="btn btn-icon" aria-label="Close"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M18 6 6 18"/><path d="m6 6 12 12"/></svg></button>
              <button class="btn btn-partner" disabled>Disabled</button>
            </div>
          </div>
          <div class="demo">
            <div class="demo-label">Focus: Tab onto a control — gold ring</div>
            <button class="btn btn-secondary square">Admin square</button>
          </div>
        </div>
      </section>

      <!-- Icon button -->
      <section class="section" id="icon-button">
        <div class="section-head"><h2>Icon button</h2><span>Lucide-style SVG</span></div>
        <div class="demo">
          <div class="demo-label">Close · chevrons · overflow · dense · ghost · disabled</div>
          <div class="row">
            <button class="btn btn-icon" type="button" aria-label="Close"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M18 6 6 18"/><path d="m6 6 12 12"/></svg></button>
            <button class="btn btn-icon" type="button" aria-label="Expand"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="m6 9 6 6 6-6"/></svg></button>
            <button class="btn btn-icon" type="button" aria-label="Previous"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="m15 18-6-6 6-6"/></svg></button>
            <button class="btn btn-icon" type="button" aria-label="Next"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="m9 18 6-6-6-6"/></svg></button>
            <button class="btn btn-icon" type="button" aria-label="More actions"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><circle cx="12" cy="12" r="1" fill="currentColor" stroke="none"/><circle cx="19" cy="12" r="1" fill="currentColor" stroke="none"/><circle cx="5" cy="12" r="1" fill="currentColor" stroke="none"/></svg></button>
            <button class="btn btn-icon dense" type="button" aria-label="Close dense"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M18 6 6 18"/><path d="m6 6 12 12"/></svg></button>
            <button class="btn btn-icon ghost" type="button" aria-label="Close ghost"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M18 6 6 18"/><path d="m6 6 12 12"/></svg></button>
            <button class="btn btn-icon" type="button" aria-label="Disabled" disabled><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M18 6 6 18"/><path d="m6 6 12 12"/></svg></button>
          </div>
        </div>
      </section>

      <!-- Fields -->
      <section class="section" id="fields">
        <div class="section-head"><h2>Form fields</h2><span>Inputs</span></div>
        <div class="grid-2">
          <div class="demo">
            <div class="demo-label">Commerce boxed</div>
            <div class="stack">
              <label class="field">
                <span class="field-label">Email</span>
                <input class="field-control" type="email" placeholder="you@clinic.com" value="rey@bravo.ph" />
              </label>
              <label class="field">
                <span class="field-label">Mobile</span>
                <input class="field-control error" type="text" value="09" aria-invalid="true" />
                <span class="field-error">Enter a valid PH mobile number</span>
              </label>
            </div>
          </div>
          <div class="demo">
            <div class="demo-label">Editorial ruled</div>
            <div class="stack">
              <label class="field ruled">
                <span class="field-label editorial">Full name</span>
                <input class="field-control field-ruled" type="text" value="Dr. Rey Aquino" />
              </label>
              <label class="field ruled">
                <span class="field-label editorial">Clinic</span>
                <input class="field-control field-ruled" type="text" placeholder="Clinic name" />
              </label>
            </div>
          </div>
        </div>
      </section>

      <!-- Segment + Tabs -->
      <section class="section" id="segment">
        <div class="section-head"><h2>Segmented control</h2><span>Choice</span></div>
        <div class="demo row">
          <div class="segment" role="group" aria-label="Plan">
            <button type="button" class="on">Trial</button>
            <button type="button">Protocol</button>
          </div>
          <div class="segment blue" role="group" aria-label="QR mode">
            <button type="button" class="on">Shop</button>
            <button type="button">Profile</button>
          </div>
        </div>
      </section>

      <!-- Switch -->
      <section class="section" id="switch">
        <div class="section-head"><h2>Switch</h2><span>Boolean</span></div>
        <div class="demo">
          <div class="demo-label">Off · on — blue track when checked</div>
          <div class="row">
            <div class="switch-row">
              <button type="button" class="switch" role="switch" aria-checked="false" aria-label="SMS alerts"></button>
              <span>SMS alerts</span>
            </div>
            <div class="switch-row">
              <button type="button" class="switch" role="switch" aria-checked="true" aria-label="Email digest"></button>
              <span>Email digest</span>
            </div>
          </div>
        </div>
      </section>

      <section class="section" id="tabs">
        <div class="section-head"><h2>Tabs</h2><span>Admin</span></div>
        <div class="demo demo--flush">
          <div class="tabs" role="tablist">
            <button type="button" class="on" role="tab" aria-selected="true">Wheel</button>
            <button type="button" role="tab">Doctors</button>
            <button type="button" role="tab">Orders</button>
            <button type="button" role="tab">Newsletter</button>
          </div>
          <div style="padding:18px;color:var(--ink-3);font-size:14px">Active tab: blue fill, bone label, square admin dialect.</div>
        </div>
      </section>

      <!-- Top bar -->
      <section class="section" id="topbar">
        <div class="section-head"><h2>Top bar</h2><span>Shell</span></div>
        <p class="note">Fixed site chrome for marketing / shop. Not used on admin or booth.</p>
        <div class="demo demo--flush">
          <header class="topbar">
            <div class="brand">GutGuard <em>Clinic</em></div>
            <nav aria-label="Primary">
              <a href="#" aria-current="page">System</a>
              <a href="#">Science</a>
              <a href="#">Shop</a>
            </nav>
            <div class="actions">
              <button class="btn btn-text">Log in</button>
              <button class="btn btn-partner" style="min-height:40px;font-size:13px">Get started</button>
            </div>
          </header>
        </div>
      </section>

      <!-- Sidebar + bottom -->
      <section class="section" id="sidebar">
        <div class="section-head"><h2>Sidebar + bottom bar</h2><span>Shell</span></div>
        <p class="note">Desktop sidebar + mobile bottom CTA. Same Doctors skin — structure from Lifestyle / Academy prototypes.</p>
        <div class="shell-demo">
          <aside class="side">
            <div class="side-brand">GutGuard <em>Life</em></div>
            <button type="button" class="on">My Health</button>
            <button type="button">My Team</button>
            <button type="button">My Story</button>
            <button type="button" style="margin-top:8px;color:var(--ink-3);font-size:13px">Settings</button>
            <div class="side-foot">
              <b>Supply left · 4 days</b>
              <button class="btn btn-partner" style="width:100%;min-height:42px;font-size:13px">Reorder</button>
            </div>
          </aside>
          <div class="shell-main">
            <div class="eyebrow">My Health</div>
            <h3 style="font-family:var(--serif);font-size:28px;font-weight:400;margin:6px 0 10px">Day 4 of 10</h3>
            <p style="color:var(--ink-3);font-size:14px;max-width:36ch">Main column content. Bottom bar is shown here as a preview of the mobile CTA.</p>
            <div class="bottom-bar">
              <div>
                <div class="eye">Do this next</div>
                <div class="title">Order your refill</div>
              </div>
              <button class="btn btn-partner" style="min-height:44px">Order</button>
            </div>
          </div>
        </div>
      </section>

      <!-- Masthead -->
      <section class="section" id="masthead">
        <div class="section-head"><h2>Masthead</h2><span>Booth</span></div>
        <div class="demo">
          <div class="masthead">
            <div class="mast-logos">
              <div class="mast-mark">GG</div>
              <span class="mast-x">×</span>
              <div class="mast-mark alt">TT</div>
              <div class="mast-text" style="margin-left:8px">
                <div class="name">Physicians Program</div>
                <div class="ed">Manila edition · Aug 2026</div>
              </div>
            </div>
            <button class="btn btn-secondary" style="border-radius:999px">About</button>
          </div>
          <div class="rail" style="margin-top:18px" aria-label="Progress">
            <span class="dot done"></span><span class="seg done"></span>
            <span class="dot done"></span><span class="seg done"></span>
            <span class="dot active"></span><span class="seg"></span>
            <span class="dot"></span>
          </div>
        </div>
      </section>

      <!-- Admin -->
      <section class="section" id="admin">
        <div class="section-head"><h2>Admin shell</h2><span>Ops</span></div>
        <div class="demo">
          <div class="admin-hero">
            <div>
              <div class="kicker">Admin · Wheel</div>
              <h3>Prize desk</h3>
            </div>
            <div class="admin-summary">Live spins<strong>128</strong></div>
          </div>
          <div class="tabs">
            <button type="button" class="on">Wheel</button>
            <button type="button">Doctors</button>
            <button type="button">SMS</button>
          </div>
        </div>
      </section>

      <!-- Cards -->
      <section class="section" id="cards">
        <div class="section-head"><h2>Cards</h2><span>Surfaces</span></div>
        <div class="grid-3">
          <div class="card editorial">
            <div class="eyebrow" style="color:var(--ink-3)">Editorial</div>
            <h3>Ruled panel</h3>
            <p>Square, bone, no heavy shadow — printed-form feel.</p>
          </div>
          <div class="card">
            <div class="eyebrow">Commerce</div>
            <h3>Raised paper</h3>
            <p>14px radius, soft shadow, paper on bone.</p>
          </div>
          <div class="card auth">
            <div class="eyebrow">Partner auth</div>
            <h3>Sign in</h3>
            <p>Blue top edge marks the auth moment.</p>
          </div>
        </div>
      </section>

      <!-- Feedback -->
      <section class="section" id="feedback">
        <div class="section-head"><h2>Badge · Alert · Toast</h2><span>Feedback</span></div>
        <div class="grid-2">
          <div class="demo stack">
            <div class="demo-label">Badges</div>
            <div class="row">
              <span class="badge">Pending</span>
              <span class="badge paid">Paid</span>
              <span class="badge paid">Active</span>
            </div>
            <div class="demo-label" style="margin-top:8px">Alerts</div>
            <div class="alert">Your card is ready — show it at the door.</div>
            <div class="alert error"><span class="t">Error</span>We couldn’t verify that mobile number.</div>
          </div>
          <div class="demo">
            <div class="demo-label">Toast</div>
            <div class="toast">
              <div class="t">Success</div>
              <p>Order confirmed. We’ll text tracking details shortly.</p>
            </div>
            <div class="toast" style="margin-top:12px">
              <div class="t err">Error</div>
              <p>Payment failed — try another method.</p>
            </div>
          </div>
        </div>
      </section>

      <!-- Dialog -->
      <section class="section" id="dialog">
        <div class="section-head"><h2>Dialog</h2><span>Header · body · footer</span></div>
        <p class="note">Structured chrome with SVG close. Prefer Dialog for titled confirm/detail flows. Backdrop rules stay with Modal.</p>
        <div class="grid-2">
          <div class="modal-demo">
            <div class="dialog" role="dialog" aria-modal="true" aria-labelledby="dlg-commerce-title">
              <div class="dialog-header">
                <h3 id="dlg-commerce-title">Confirm registration</h3>
                <button class="btn btn-icon ghost" type="button" aria-label="Close"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M18 6 6 18"/><path d="m6 6 12 12"/></svg></button>
              </div>
              <div class="dialog-body">
                Submit registration for <strong style="color:var(--ink)">Dr. Rey Aquino</strong>? They will receive an SMS with partner portal access.
              </div>
              <div class="dialog-footer">
                <button class="btn btn-secondary" type="button">Cancel</button>
                <button class="btn btn-partner" type="button">Confirm</button>
              </div>
            </div>
          </div>
          <div class="modal-demo">
            <div class="dialog square" role="dialog" aria-modal="true" aria-labelledby="dlg-admin-title">
              <div class="dialog-header">
                <h3 id="dlg-admin-title">Void order</h3>
                <button class="btn btn-icon ghost square" type="button" aria-label="Close"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M18 6 6 18"/><path d="m6 6 12 12"/></svg></button>
              </div>
              <div class="dialog-body">
                Void <strong style="color:var(--ink)">GG-24018</strong>? This cannot be undone from the admin table.
              </div>
              <div class="dialog-footer">
                <button class="btn btn-secondary square" type="button">Cancel</button>
                <button class="btn btn-secondary square" type="button" style="border-color:var(--error);color:var(--error-text)">Void</button>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- Modal / Drawer -->
      <section class="section" id="modal">
        <div class="section-head"><h2>Modal · Drawer</h2><span>Overlays</span></div>
        <p class="note">Simple confirm shell + drawer. For header / close / footer chrome, use <a href="#dialog">Dialog</a>.</p>
        <div class="grid-2">
          <div class="modal-demo">
            <div class="modal">
              <h3>Confirm</h3>
              <p>Submit registration for Dr. Rey Aquino?</p>
              <div class="actions">
                <button class="btn btn-secondary">Cancel</button>
                <button class="btn btn-partner">Confirm</button>
              </div>
            </div>
          </div>
          <div class="drawer-demo">
            <div class="drawer-scrim"></div>
            <aside class="drawer">
              <h3>Basket</h3>
              <p style="color:var(--ink-3);font-size:14px;margin-bottom:14px">Side drawer · paper · soft shadow.</p>
              <button class="btn btn-commerce" style="width:100%;min-height:52px;font-size:14px">Checkout</button>
            </aside>
          </div>
        </div>
      </section>

      <!-- Table -->
      <section class="section" id="table">
        <div class="section-head"><h2>Table</h2><span>Data</span></div>
        <div class="table-wrap">
          <table>
            <thead>
              <tr><th>Name</th><th>Clinic</th><th>Status</th><th></th></tr>
            </thead>
            <tbody>
              <tr>
                <td>Dr. Rey Aquino</td>
                <td>Bravo Medical</td>
                <td><span class="badge paid">Paid</span></td>
                <td><button class="btn btn-secondary" style="min-height:36px;padding:0 12px">Open</button></td>
              </tr>
              <tr>
                <td>Dr. Ana Cruz</td>
                <td>North Clinic</td>
                <td><span class="badge">Pending</span></td>
                <td><button class="btn btn-secondary" style="min-height:36px;padding:0 12px">Open</button></td>
              </tr>
            </tbody>
          </table>
        </div>
      </section>

      <!-- Def list -->
      <section class="section" id="deflist">
        <div class="section-head"><h2>Definition list</h2><span>Data</span></div>
        <div class="demo">
          <dl class="deflist">
            <div><dt>Full name</dt><dd>Dr. Rey Aquino</dd></div>
            <div><dt>Clinic</dt><dd>Bravo Medical</dd></div>
            <div><dt>Mobile</dt><dd>+63 917 000 0000</dd></div>
          </dl>
        </div>
      </section>

      <!-- QR / progress / tasks -->
      <section class="section" id="qr">
        <div class="section-head"><h2>QR · Progress · Tasks</h2><span>Utility</span></div>
        <div class="grid-3">
          <div class="demo">
            <div class="demo-label">QR block</div>
            <div class="qr" aria-hidden="true">
              <div class="qr-grid">
                <i></i><i></i><i></i><i class="off"></i><i></i><i></i><i></i>
                <i></i><i class="off"></i><i></i><i class="off"></i><i></i><i class="off"></i><i></i>
                <i></i><i></i><i></i><i class="off"></i><i></i><i></i><i></i>
                <i class="off"></i><i class="off"></i><i class="off"></i><i></i><i class="off"></i><i class="off"></i><i class="off"></i>
                <i></i><i></i><i></i><i class="off"></i><i></i><i class="off"></i><i></i>
                <i></i><i class="off"></i><i></i><i></i><i class="off"></i><i></i><i></i>
                <i></i><i></i><i></i><i class="off"></i><i></i><i></i><i></i>
              </div>
            </div>
            <div class="row" style="margin-top:12px">
              <button class="btn btn-secondary">Download</button>
            </div>
          </div>
          <div class="demo">
            <div class="demo-label">Section label</div>
            <div class="section-label">
              <i></i><span class="num">01</span><span class="lab">What it takes</span>
            </div>
            <p style="color:var(--ink-2);font-size:14px;margin-top:8px">Complete each requirement to unlock the next rank.</p>
          </div>
          <div class="demo">
            <div class="demo-label">Task items</div>
            <div class="task done">
              <span class="num">✓</span>
              <div><b>Verify TikTok</b><div class="meta">Connected</div></div>
            </div>
            <div class="task">
              <span class="num">2</span>
              <div><b>Book session</b><div class="meta">Choose a date</div></div>
              <span class="chev" aria-hidden="true"><svg class="icon" viewBox="0 0 24 24"><path d="m9 18 6-6-6-6"/></svg></span>
            </div>
          </div>
        </div>
      </section>

      <!-- Empty -->
      <section class="section" id="empty">
        <div class="section-head"><h2>Empty state</h2><span>Feedback</span></div>
        <div class="empty">
          <b>No orders yet</b>
          <span>When partners check out, they’ll show up here.</span>
        </div>
      </section>

      <!-- File attachment -->
      <section class="section" id="file">
        <div class="section-head"><h2>File attachment</h2><span>Custom · hide native input</span></div>
        <p class="note">Never show the browser’s default file control. Keep <code>&lt;input type="file"&gt;</code> visually hidden; open it from the drop zone or a secondary button.</p>
        <div class="grid-2">
          <div class="demo">
            <div class="demo-label">Drop zone (empty)</div>
            <div class="file-attach" data-file-demo="empty">
              <input class="file-attach__input" id="file-demo-empty" type="file" accept=".html,.png,.jpg,.jpeg,image/*,text/html" />
              <label class="upload" for="file-demo-empty">
                <span class="up-ico" aria-hidden="true"><svg class="icon" viewBox="0 0 24 24"><path d="M12 3v12"/><path d="m17 8-5-5-5 5"/><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/></svg></span>
                <b>Drop HTML or image here</b>
                <span class="hint">Max 5MB · .html .png .jpg</span>
                <span class="btn btn-secondary">Choose file</span>
              </label>
            </div>
          </div>
          <div class="demo">
            <div class="demo-label">Selected · progress · remove (SVG)</div>
            <div class="file-row">
              <div class="ico" aria-hidden="true"><svg class="icon" viewBox="0 0 24 24"><path d="M15 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V7Z"/><path d="M14 2v4a2 2 0 0 0 2 2h4"/><path d="M10 9H8"/><path d="M16 13H8"/><path d="M16 17H8"/></svg></div>
              <div>
                <div class="name">newsletter-aug.html</div>
                <div class="meta">128 KB · uploading…</div>
              </div>
              <button class="btn btn-icon rm" type="button" aria-label="Remove"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M18 6 6 18"/><path d="m6 6 12 12"/></svg></button>
            </div>
            <div class="file-progress" aria-hidden="true"><i></i></div>
            <div class="row" style="margin-top:12px">
              <button class="btn btn-partner" type="button">Upload</button>
            </div>
          </div>
          <div class="demo">
            <div class="demo-label">Error</div>
            <div class="file-attach">
              <input class="file-attach__input" id="file-demo-err" type="file" disabled tabindex="-1" />
              <label class="upload has-error" for="file-demo-err">
                <span class="up-ico" aria-hidden="true"><svg class="icon" viewBox="0 0 24 24"><path d="M12 3v12"/><path d="m17 8-5-5-5 5"/><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/></svg></span>
                <b>File too large</b>
                <span class="hint">Max 5MB — choose a smaller file</span>
                <span class="btn btn-secondary">Choose file</span>
              </label>
            </div>
          </div>
          <div class="demo">
            <div class="demo-label">Compact button (still custom)</div>
            <div class="file-attach file-compact">
              <input class="file-attach__input" id="file-demo-compact" type="file" accept="image/*" />
              <label class="btn btn-secondary" for="file-demo-compact">Choose file</label>
              <span style="color:var(--ink-3);font-size:13px">PNG or JPG · camera OK</span>
            </div>
          </div>
        </div>
      </section>

      <!-- Avatar -->
      <section class="section" id="avatar">
        <div class="section-head"><h2>Avatar</h2><span>Utilities</span></div>
        <div class="demo row">
          <div class="avatar-row">
            <div class="avatar lg blue">RA</div>
            <div><b>Rey Aquino</b><span>Team Bravo</span></div>
          </div>
          <div class="avatar">AC</div>
          <div class="avatar sm">NL</div>
          <div class="avatar blue">GG</div>
        </div>
      </section>

      <!-- Search -->
      <section class="section" id="search">
        <div class="section-head"><h2>Search field</h2><span>Utilities</span></div>
        <div class="demo" style="max-width:420px">
          <div class="search">
            <span class="ico" aria-hidden="true">⌕</span>
            <input type="text" inputmode="search" placeholder="Search doctors…" value="Aquino" />
            <button class="clear" type="button" aria-label="Clear"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="M18 6 6 18"/><path d="m6 6 12 12"/></svg></button>
          </div>
        </div>
      </section>

      <!-- Stepper -->
      <section class="section" id="stepper">
        <div class="section-head"><h2>Quantity stepper</h2><span>Utilities</span></div>
        <div class="demo row">
          <div class="stepper" aria-label="Quantity">
            <button type="button" aria-label="Decrease">−</button>
            <span class="val">2</span>
            <button type="button" aria-label="Increase">+</button>
          </div>
          <div class="stepper" aria-label="Doses">
            <button type="button" disabled aria-label="Decrease">−</button>
            <span class="val">1</span>
            <button type="button" aria-label="Increase">+</button>
          </div>
        </div>
      </section>

      <!-- Pagination -->
      <section class="section" id="pagination">
        <div class="section-head"><h2>Pagination</h2><span>Utilities</span></div>
        <div class="demo">
          <div class="pagination">
            <div class="meta">Showing 1–20 of 240</div>
            <div class="controls">
              <label class="meta" for="psize">Per page</label>
              <select id="psize"><option>20</option><option>50</option></select>
              <button class="btn btn-secondary square" type="button" disabled>Prev</button>
              <button class="btn btn-secondary square" type="button">Next</button>
            </div>
          </div>
        </div>
      </section>

      <!-- Dropdown -->
      <section class="section" id="dropdown">
        <div class="section-head"><h2>Dropdown menu</h2><span>Utilities</span></div>
        <div class="demo">
          <div class="menu-wrap">
            <button class="btn btn-icon" type="button" aria-expanded="true" aria-haspopup="menu">···</button>
            <div class="menu" role="menu">
              <button type="button" role="menuitem">Open</button>
              <button type="button" role="menuitem">Download QR</button>
              <hr />
              <button type="button" role="menuitem" class="danger">Remove</button>
            </div>
          </div>
          <p class="note" style="margin:48px 0 0">Overflow actions for tables and cards. Gold focus on trigger; blue wash on item hover.</p>
        </div>
      </section>

      <!-- Tooltip -->
      <section class="section" id="tooltip">
        <div class="section-head"><h2>Tooltip</h2><span>Utilities</span></div>
        <div class="demo">
          <div class="tip-wrap">
            <button class="btn btn-secondary" type="button">Hover or focus me</button>
            <span class="tip" role="tooltip">Short helper — not for essential copy</span>
          </div>
        </div>
      </section>

      <!-- Spinner / Skeleton -->
      <section class="section" id="spinner">
        <div class="section-head"><h2>Spinner · Skeleton</h2><span>Loading</span></div>
        <div class="grid-2">
          <div class="demo">
            <div class="demo-label">Spinner</div>
            <div class="row">
              <span class="spinner" aria-hidden="true"></span>
              <span class="spinner lg" aria-hidden="true"></span>
              <button class="btn btn-partner" type="button" style="gap:10px">
                <span class="spinner on-dark" aria-hidden="true"></span> Saving…
              </button>
            </div>
          </div>
          <div class="demo">
            <div class="demo-label">Skeleton</div>
            <div class="avatar-row" style="margin-bottom:14px">
              <div class="skeleton avatar"></div>
              <div style="flex:1">
                <div class="skeleton line" style="width:70%"></div>
                <div class="skeleton line short"></div>
              </div>
            </div>
            <div class="skeleton block"></div>
          </div>
        </div>
      </section>

      <!-- Accordion -->
      <section class="section" id="accordion">
        <div class="section-head"><h2>Accordion</h2><span>Extended</span></div>
        <div class="accordion">
          <div class="acc-item open">
            <button class="acc-head" type="button" aria-expanded="true">What is GutGuard?<span class="chev" aria-hidden="true"><svg class="icon" viewBox="0 0 24 24"><path d="m6 9 6 6 6-6"/></svg></span></button>
            <div class="acc-body">Clinical + editorial premium health products and programs. This panel uses Doctors bone / paper / rule.</div>
          </div>
          <div class="acc-item">
            <button class="acc-head" type="button" aria-expanded="false">How do refills work?<span class="chev" aria-hidden="true"><svg class="icon" viewBox="0 0 24 24"><path d="m6 9 6 6 6-6"/></svg></span></button>
            <div class="acc-body">Order from the member bottom bar or shop. Tracking arrives by SMS.</div>
          </div>
          <div class="acc-item">
            <button class="acc-head" type="button" aria-expanded="false">Where is my QR?<span class="chev" aria-hidden="true"><svg class="icon" viewBox="0 0 24 24"><path d="m6 9 6 6 6-6"/></svg></span></button>
            <div class="acc-body">On the flip side of your door card and in partner portal.</div>
          </div>
        </div>
      </section>

      <!-- Breadcrumbs -->
      <section class="section" id="breadcrumbs">
        <div class="section-head"><h2>Breadcrumbs</h2><span>Extended</span></div>
        <div class="demo">
          <nav class="crumbs" aria-label="Breadcrumb">
            <a href="#">Admin</a><span class="sep">/</span>
            <a href="#">Orders</a><span class="sep">/</span>
            <span class="cur">GG-24018</span>
          </nav>
        </div>
      </section>

      <!-- Date picker -->
      <section class="section" id="datepicker">
        <div class="section-head"><h2>Date picker</h2><span>Extended</span></div>
        <div class="demo">
          <div class="datepicker" aria-label="Calendar">
            <div class="dp-head">
              <button class="btn btn-icon dense" type="button" aria-label="Previous month"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="m15 18-6-6 6-6"/></svg></button>
              <span>August 2026</span>
              <button class="btn btn-icon dense" type="button" aria-label="Next month"><svg class="icon" viewBox="0 0 24 24" aria-hidden="true"><path d="m9 18 6-6-6-6"/></svg></button>
            </div>
            <div class="dp-grid">
              <span class="dow">Su</span><span class="dow">Mo</span><span class="dow">Tu</span><span class="dow">We</span><span class="dow">Th</span><span class="dow">Fr</span><span class="dow">Sa</span>
              <button type="button" class="mute">26</button><button type="button" class="mute">27</button><button type="button" class="mute">28</button><button type="button" class="mute">29</button><button type="button" class="mute">30</button><button type="button" class="mute">31</button><button type="button">1</button>
              <button type="button">2</button><button type="button">3</button><button type="button">4</button><button type="button">5</button><button type="button">6</button><button type="button">7</button><button type="button">8</button>
              <button type="button">9</button><button type="button">10</button><button type="button">11</button><button type="button" class="today on">12</button><button type="button">13</button><button type="button">14</button><button type="button">15</button>
              <button type="button">16</button><button type="button">17</button><button type="button">18</button><button type="button">19</button><button type="button">20</button><button type="button">21</button><button type="button">22</button>
            </div>
          </div>
        </div>
      </section>

      <!-- Notification bell -->
      <section class="section" id="notify">
        <div class="section-head"><h2>Notification bell</h2><span>Extended</span></div>
        <div class="demo" style="min-height:220px">
          <div class="bell-wrap">
            <button class="bell-btn" type="button" aria-label="Notifications">🔔</button>
            <span class="bell-count">3</span>
            <div class="bell-panel" role="menu">
              <div class="ph">Notifications</div>
              <button class="bell-item unread" type="button"><b>Refill reminder</b><span>4 days of supply left</span></button>
              <button class="bell-item unread" type="button"><b>Session booked</b><span>Thu · Bravo Clinic</span></button>
              <button class="bell-item" type="button"><b>Welcome</b><span>Your card is ready</span></button>
            </div>
          </div>
        </div>
      </section>

      <!-- Chat link row -->
      <section class="section" id="chatrow">
        <div class="section-head"><h2>Chat link row</h2><span>Extended</span></div>
        <div class="demo">
          <button class="chat-row" type="button">
            <span class="chat-tile">TG</span>
            <span><b>Team Bravo chat</b><em>24 members · Telegram</em></span>
            <span class="go">Open →</span>
          </button>
          <p class="note" style="margin-top:12px">Channel tile may use a local brand color; the rest stays Doctors paper / rule / ink.</p>
        </div>
      </section>

      <footer style="margin-top:64px;padding-top:20px;border-top:1px solid var(--rule);color:var(--ink-3);font-size:13px">
        GutGuard Design System · visual source Doctors HTML · open <code style="color:var(--ink)">Showcase/index.html</code> in a browser
      </footer>
    </main>
  </div>

  <script>
    // Lightweight segment/tab toggling for the showcase
    document.querySelectorAll('.segment').forEach(group => {
      group.addEventListener('click', e => {
        const btn = e.target.closest('button');
        if (!btn) return;
        group.querySelectorAll('button').forEach(b => b.classList.remove('on'));
        btn.classList.add('on');
      });
    });
    document.querySelectorAll('.tabs').forEach(group => {
      group.addEventListener('click', e => {
        const btn = e.target.closest('button');
        if (!btn) return;
        group.querySelectorAll('button').forEach(b => {
          b.classList.remove('on');
          b.setAttribute('aria-selected', 'false');
        });
        btn.classList.add('on');
        btn.setAttribute('aria-selected', 'true');
      });
    });
    document.querySelectorAll('.side > button').forEach(btn => {
      btn.addEventListener('click', () => {
        btn.parentElement.querySelectorAll(':scope > button').forEach(b => b.classList.remove('on'));
        if (!btn.style.color || btn.style.color === '') btn.classList.add('on');
        else btn.classList.add('on');
      });
    });
    document.querySelectorAll('.acc-head').forEach(btn => {
      btn.addEventListener('click', () => {
        const item = btn.closest('.acc-item');
        const open = item.classList.toggle('open');
        btn.setAttribute('aria-expanded', open ? 'true' : 'false');
      });
    });
    document.querySelectorAll('.stepper').forEach(step => {
      const val = step.querySelector('.val');
      step.addEventListener('click', e => {
        const btn = e.target.closest('button');
        if (!btn || btn.disabled) return;
        let n = parseInt(val.textContent, 10) || 0;
        if (btn.getAttribute('aria-label') === 'Decrease') n = Math.max(0, n - 1);
        else n += 1;
        val.textContent = String(n);
        const dec = step.querySelector('[aria-label="Decrease"]');
        if (dec) dec.disabled = n <= 0;
      });
    });
    const dp = document.querySelector('.dp-grid');
    if (dp) {
      dp.addEventListener('click', e => {
        const btn = e.target.closest('button');
        if (!btn || btn.classList.contains('mute')) return;
        dp.querySelectorAll('button').forEach(b => b.classList.remove('on'));
        btn.classList.add('on');
      });
    }
    document.querySelectorAll('.switch').forEach(sw => {
      sw.addEventListener('click', () => {
        const on = sw.getAttribute('aria-checked') === 'true';
        sw.setAttribute('aria-checked', on ? 'false' : 'true');
      });
    });
  </script>
</body>
</html>
````