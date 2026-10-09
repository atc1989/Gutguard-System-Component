---
title: Ownership — read only for the team
aliases:
  - DO NOT EDIT
  - Owner lock
tags: [gutguard, design-system, governance]
updated: 2026-08-12
---

# Ownership — do not edit this vault

> [!danger] Read-only for everyone except the owner
> This **GutGuard Design System** folder is the shared source of truth via Obsidian Sync.
> **Only the designated owner may change these notes** (and the Showcase HTML).
> Everyone else: **read, copy templates into your product repos, implement UI — do not edit the vault.**

## Owner

| Field | Value |
|---|---|
| Owner | Najee |
| Authoritative machine | Najee’s PC (this vault path under Najee’s user profile) |
| Contact | Ask Najee for DS changes |

## What teammates may do

- Read all notes and open `Showcase/index.html`
- Copy `Templates/` into their project `AGENTS.md` / `.cursor/rules/`
- Use the DS when building products
- Suggest changes in chat / Linear / Slack — **owner applies them here**

## What teammates must not do

- Edit, rename, or delete notes in this folder
- “Improve” tokens, components, or the showcase on their machine (Sync would overwrite the team copy)
- Point Cursor at this vault with write intent (`Write` / `StrReplace` / delete)

## For Cursor agents (any machine)

If the workspace includes this vault path:

1. **READ only** — never modify files under `GutGuard Design System/`
2. Implement UI in the **product repo**, not in Obsidian
3. If a DS change is needed, tell the user: *“Ask the design-system owner (Najee) to update the vault.”*

## Why Sync can’t lock it for real

Obsidian Sync is two-way. This is a **team rule + Cursor rule**, not a filesystem permission. Discipline + the templates below keep the vault stable.

Owner Cursor rule snippet lives in [[Templates/gutguard-design-system]] — includes “do not write to the vault.”
