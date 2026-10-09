---
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
