---
title: Boss HTML / Next.js → Obsidian → Stitch workflow
tags: [gutguard, stitch, workflow, cursor]
updated: 2026-08-12
---

# Stitch workflow

Goal: when the boss sends HTML or a Next.js app, Cursor reads this vault’s design system, Stitch generates on-brand screens, and we implement against the portable CSS.

## Paths

| Role | Path |
|---|---|
| Obsidian vault | `C:\Users\najee\OneDrive\Documents\Obsidian Vault\` |
| Design system | `GutGuard Design System\` |
| Stitch brief | `GutGuard Design System\DESIGN.md` |
| Portable CSS | `GutGuard Design System\03 - Portable CSS Starter.md` |
| Inbox for boss drops | `GutGuard Design System\Inbox\` |

## Operator steps (human)

1. Drop the boss file/folder into `Inbox\` (or paste the path in Cursor chat).
2. In Cursor **Customize → MCPs**, confirm `stitch` shows tools **> 0** (not “0 tools enabled”).
3. Tell Cursor: *“Run the GutGuard Stitch workflow on `<path>` using dialect `<editorial|commerce|admin>`.”*

## Agent steps (Cursor)

1. Read `DESIGN.md`, dialect notes (`01` + `Foundations/Dialects`), and relevant notes under `Components/`.
2. Inspect the boss HTML / Next.js screens (routes, components, copy, structure).
3. Create or select a Stitch project for this deliverable.
4. Upload / apply `DESIGN.md` as the design system for that project.
5. Generate screens in Stitch that preserve boss structure/content but GutGuard visual language.
6. Export HTML/screenshots from Stitch.
7. Implement into the Next.js/HTML target using tokens/classes from the portable CSS starter.
8. Log outputs under `Inbox\<deliverable-name>\` (notes + export paths).
9. If the boss system introduced new reusable UI, update `Systems/` + `Components/Index`.

## Prompt template

```text
Run the GutGuard Stitch workflow.

Input: <path to boss HTML or Next.js>
Dialect: <editorial | commerce | admin>
Design system: GutGuard Design System/DESIGN.md + 03 Portable CSS Starter

Do:
1) Summarize screens/routes in the input
2) Apply DESIGN.md in Stitch
3) Generate each screen on-brand
4) Export and propose Next.js/HTML implementation plan using gg-* tokens/classes
```

## Stitch MCP health

If MCP shows **Connected / 0 tools enabled**, Cursor is dropping Stitch’s oversized tool schemas. Use the local proxy:

- Proxy script: `%USERPROFILE%\.cursor\stitch-mcp-proxy.mjs`
- MCP config: `%USERPROFILE%\.cursor\mcp.json` must run `node` + that proxy with `STITCH_API_KEY`

Then toggle the `stitch` server off/on (or restart Cursor) until tool count is > 0.
