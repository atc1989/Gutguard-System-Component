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
