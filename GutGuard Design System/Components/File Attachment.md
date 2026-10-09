---
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
