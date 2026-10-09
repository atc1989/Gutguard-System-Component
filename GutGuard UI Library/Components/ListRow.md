---
title: ListRow
tags: [gutguard, ui-library, component]
group: Components
status: draft
code: gutguard-ui/components/ui/ListRow.tsx
example: gutguard-ui/showcase/examples/ListRow.tsx
parts: [l-plan-sheet, l-points, g-first]
updated: 2026-10-08
---

# ListRow

Lifestyle row with a bold title and a sub line. Tappable rows end in a blue "›"; static rows hold their own action on the right. Use for menus of actions in sheets; use `PersonRow` for people and `IconRow` for non-interactive feature lists.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| button (default) | Action in a sheet: Change plan, Pause | Lifestyle `button.tap` rows (plan sheet) |
| `href` → link | Row that navigates: Add a one-time order, Skip the trial | Lifestyle `a.tap` rows |
| `as="div"` | Static row with a button on the right: rewards | E-Points reward rows |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `title` | ReactNode | — | |
| `description` | ReactNode | — | Grey sub line |
| `icon` | ReactNode | — | Lucide icon in a bone circle |
| `trailing` | ReactNode | blue "›" when tappable | Pass a `Button size="sm"` on static rows |
| `href` | string | — | Renders `<a>` |
| `as` | `"button"` \| `"div"` | `button` | `div` for rows that contain a button |
| …rest | button / anchor / div attributes | | `onClick`, `disabled` … |

## States

Active: scale .97 (tappable). Focus-visible: global gold ring. Static rows have no states; their trailing Button has its own.

## Responsive

Same on all widths (full width of its column).

## Source

- Original: Lifestyle inline rows in components/prototype/LifestyleMember.jsx:379 (plan sheet, E-Points sheet) and LifestyleLanding.jsx:751 (first step)
- Found in: l-plan-sheet, l-points, g-first

## Accessibility

Real `<button type="button">` or `<a>`; the "›" and icon are `aria-hidden`. Never put a button inside a tappable row: use `as="div"`.
