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
