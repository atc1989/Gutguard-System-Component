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
