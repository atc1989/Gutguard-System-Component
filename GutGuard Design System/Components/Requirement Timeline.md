---
title: Requirement Timeline
tags: [gutguard, design-system, components]
updated: 2026-08-14
status: draft
sources:
  - gentrep-academy-dashboard.html (.reqs, .req, .spine, .rail, .node, .req-card)
system: [[Systems/Gentrep-Academy-Dashboard]]
---

# Requirement Timeline

Vertical checklist of unlock requirements with a spine/rail and cards.

## Anatomy

```
(node)  ┌─ card ─────────────────┐
  │     │ TYPE (uppercase)       │
 rail   │ Title                  │
  │     │ Description            │
  │     │ [ Button ]             │
  │     │ optional Event Rows    │
        └────────────────────────┘
```

- Node states: default · done (gold fill) · booked (gold ring) · missed (clay)
- Card states: default · `.active` (blue border + soft blue shadow) · `.missed`
- Types seen: document · attendance · demonstration · derived

## Related

- Actions use [[Components/Button]]
- Attendance expand uses [[Components/Event Row]]
- Related spirit to [[Components/Task Item]] but richer

## Responsive

See [[Foundations/Breakpoints]].

Spine + cards in a single column on mobile; keep card padding readable. From desktop, same single column inside content well unless product specifies two-up.

## Finalize
- [ ] Unify node colors with GG semantic tokens
- [ ] Mark **Final** or system-only
