---
title: PersonRow
tags: [gutguard, ui-library, component]
group: Patterns
status: draft
code: gutguard-ui/components/patterns/PersonRow.tsx
example: gutguard-ui/showcase/examples/PersonRow.tsx
parts: [l-family, l-team, g-sponsor]
updated: 2026-10-08
---

# PersonRow

A person in a paper box: avatar, name, a line under it, something on the right. Use for family plans, team members and the sponsor. Use `ListRow` for non-person actions.

## Variants

| Variant | Use for | Replaces |
|---|---|---|
| `family` (default) | Plan you pay for someone, "MANAGE ›" | Lifestyle family row |
| `team` | Team member: status, caps left, extra content below | Lifestyle My Team member card |
| `sponsor` | Who invited you | Lifestyle landing sponsor row |

## Props

| Prop | Type | Default | Notes |
|---|---|---|---|
| `variant` | see above | `family` | |
| `initials` | string | — | `Avatar` (bone on family, ink on sponsor); omit on team |
| `name` | ReactNode | — | Serif (family, team) or sans (sponsor) |
| `note` | ReactNode | — | Muted text after the name: "· via Malou" |
| `description` | ReactNode | — | Line under the name; pass a `Badge dot` for status |
| `trailing` | ReactNode | — | A string renders as the blue mono action ("Manage ›") |
| `children` | ReactNode | — | Extra content under the row (team: 7-day dots, Follow up) |
| `as` | `"button"` \| `"div"` | `div` | `button` when the whole row opens something |
| …rest | button / div attributes | | |

## States

`as="button"`: active scale .97, focus-visible gold ring. `div`: none.

## Responsive

Same on all widths.

## Source

- Original: Lifestyle inline markup in components/prototype/LifestyleMember.jsx:586 (family), :998 (team) and LifestyleLanding.jsx:632 (sponsor)
- Found in: l-family, l-team, g-sponsor

## Accessibility

Use `as="button"` only when the row has no buttons inside; team rows with "Follow up" stay `div`. Avatar is `aria-hidden`; the name is read.
