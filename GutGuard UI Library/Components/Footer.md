---
title: Footer
tags: [gutguard, ui-library, component]
group: Shell
status: draft
code: gutguard-ui/components/shell/Footer.tsx
example: gutguard-ui/showcase/examples/Footer.tsx
parts: [w-footer]
updated: 2026-10-08
---

# Footer

The end of every site page, on the bone background: a site map with the current page marked, the logo and tagline, footer links and the legal lines. All content comes from props.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| (one) | Every website and shop page | `footer`, `.sitemap`, `.smap-*`, `.foot-*`, `.cry` |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `columns` | `{ label, href, current?, sections: { label, href }[] }[]` | — | `current` makes the heading blue and adds "You are here" |
| `tagline` | string | — | Serif italic gold line under the logo ("We Gut You.") |
| `links` | `{ label, href }[]` | — | Footer nav |
| `legal` | string[] | — | One mono line each |
| `homeHref` | string | `/` | Logo link |

## States

Headings, sections and footer links turn blue on hover. Focus-visible: gold ring.

## Responsive

Phone: site map in 2 columns, the bottom row stacks and the legal lines are left-aligned. From `sm` (520px; the original switched at 680px): 5 columns, bottom row in a line, legal right-aligned. Touch screens get extra padding on the section and footer links.

## Source

- Original: footer markup in components/GutguardSite.jsx:296
- Found in: w-footer
- Simplified: section entries are `<a href="#…">` links instead of buttons that scroll by script.

## Accessibility

Two landmarks: `nav aria-label="Site map"` and `nav aria-label="Footer"`. The current page heading has `aria-current="page"`. The logo link is labelled "Gutguard home".
