---
title: Using the Design System with Cursor
aliases:
  - Cursor adoption guide
  - AGENTS design system
tags: [gutguard, design-system, cursor, agents, playbook]
updated: 2026-08-12
---

# Using the Design System with Cursor

**Before Cursor generates any frontend**, the human and the agent must read this vault’s design system. Prototypes/boss files define *what* to build; **Obsidian defines how it looks**.

Related: [[05 - Playbook]] (team process) · live preview `Showcase/index.html` · [[00 - OWNER — Read only]]

---

## For humans (before you open Cursor)

1. Sync Obsidian so `GutGuard Design System/` is current.
2. Remember: **read-only** unless you are the DS owner ([[00 - OWNER — Read only]]).
3. Skim in this order:
   1. [[00 - GutGuard Design System]]
   2. [[01 - Visual Foundations]] + [[Foundations/Dialects]]
   3. [[Components/Index]] (only the components you’ll need)
   4. Optional: open `Showcase/index.html` in a browser
4. Decide **one dialect** for the screen: editorial · commerce · admin.
5. Drop boss HTML / brief into `Inbox/` or keep the path ready (**owner** manages Inbox on the authority machine if Sync conflicts worry you).
6. In the **product repo**, paste the AGENTS / Cursor rule below (once per project).
7. Then prompt Cursor — e.g.  
   *“Build the Academy dashboard UI. Dialect: commerce. Read the GutGuard Design System vault first; do not invent colors or fonts; do not edit the vault.”*

---

## For Cursor / agents (hard rule)

**Always, before writing UI:**

1. Read (at minimum) from `{GG_DS}` — see path section above:
   - `00 - OWNER — Read only.md`
   - `00 - GutGuard Design System.md`
   - `01 - Visual Foundations.md`
   - `Foundations/Dialects.md`
   - `Components/Index.md`
   - Relevant `Components/<Name>.md` notes
   - `03 - Portable CSS Starter.md` when adding styles
2. Optional visual check: `Showcase/index.html`
3. Then generate frontend using Doctors tokens (bone, ultramarine, Fraunces, Inter Tight).
4. Never treat Academy / Lifestyle / other prototypes as visual source of truth.
5. **Never modify files under `GutGuard Design System/`.** Product repo only. DS changes → ask owner (Najee).

**Vault path:** each teammate uses **their own** synced path to the same folder name `GutGuard Design System`. Obsidian Sync shares the notes; the PC path is local.

Example shape (replace with yours):

`C:\Users\<you>\OneDrive\Documents\Obsidian Vault\GutGuard Design System\`

Najee’s machine (reference only):

`C:\Users\najee\OneDrive\Documents\Obsidian Vault\GutGuard Design System\`

---

## Paste into each product repo

### Option A — `AGENTS.md` (recommended)

Create or append in the project root:

```markdown
# GutGuard UI — Design System gate

Before generating or changing any frontend (HTML, CSS, React, Stitch):

1. Read the Obsidian GutGuard Design System (synced vault) — **READ ONLY**.
2. Do **not** edit, create, or delete files inside `GutGuard Design System/`. Only the DS owner (Najee) may change the vault. Implement UI in this product repo only.
3. Minimum reads:
   - `GutGuard Design System/00 - OWNER — Read only.md`
   - `GutGuard Design System/00 - GutGuard Design System.md`
   - `GutGuard Design System/01 - Visual Foundations.md`
   - `GutGuard Design System/Foundations/Dialects.md`
   - `GutGuard Design System/Components/Index.md`
   - Component notes under `GutGuard Design System/Components/` for UI you touch
   - `GutGuard Design System/03 - Portable CSS Starter.md` for tokens/classes
4. Open `GutGuard Design System/Showcase/index.html` if unsure how a control should look.
5. Pick one dialect per screen (editorial / commerce / admin). Do not mix radius policies.
6. Visual source of truth = Doctors / vault — NOT boss prototypes (Academy, Lifestyle, etc.).
7. Recognition cues: bone `#F4F1EA`, blue `#0608A9`, ink `#0F0F18`, gold `#B08D5B`, Fraunces + Inter Tight, paper grain, uppercase micro-labels.

Local vault path — **replace with YOUR synced path**:
`C:\Users\<you>\…\Obsidian Vault\GutGuard Design System\`

Workflow detail: vault note `07 - Using the DS with Cursor.md` and `05 - Playbook.md`.
```

### Option B — `.cursor/rules/gutguard-design-system.mdc`

Copy from [[Templates/gutguard-design-system]] (or `Templates/gutguard-design-system.mdc`). After paste, set `GG_DS` to **your** vault path — not a teammate’s.

Use **both** if you want belt-and-suspenders (AGENTS.md for all agents; `.mdc` for Cursor).

---

## Suggested first prompt (copy)

```text
We are building <system name>.

Design system (read BEFORE coding) — MY vault path:
C:\Users\<you>\…\Obsidian Vault\GutGuard Design System\

Read 00, 01, Foundations/Dialects, Components/Index, and any component notes we need.
Dialect for this work: <editorial | commerce | admin>
Boss / prototype structure (look is NOT from here): <path>

Do:
1) Confirm which components from the Index you will use
2) Generate the frontend using Doctors / vault visuals only
3) Prefer gg-* tokens from 03 - Portable CSS Starter
```

---

## Checklist for a new system

- [ ] Obsidian Sync on for the shared vault
- [ ] `AGENTS.md` and/or `.cursor/rules/gutguard-design-system.mdc` in the repo
- [ ] Dialect chosen
- [ ] Boss file in `Inbox/` or path given
- [ ] Agent read vault before first UI file
- [ ] QA against [[05 - Playbook]] checklist + `Showcase/index.html`

---

## FAQ

**Is the Playbook enough?**  
[[05 - Playbook]] is process + remap. **This note** is specifically “gate Cursor until the DS is read.”

**What if Cursor can’t see OneDrive?**  
Add the vault folder to the workspace (multi-root) or paste the absolute path in the prompt. The rule says: stop and ask — don’t invent UI.

**Stitch?**  
Still upload [[DESIGN]]; structure from boss; visuals from vault. See [[04 - Stitch Workflow]].
