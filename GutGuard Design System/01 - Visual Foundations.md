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

