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
