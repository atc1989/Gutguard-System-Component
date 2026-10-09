---
title: Sync and team guide — UI Library update (Oct 2026)
tags: [gutguard, ui-library, guide, sync]
created: 2026-10-08
owner: Najee
---

# Sync and team guide

What changed in the vault on 8 Oct 2026, how it reaches the team through Obsidian Sync, and how to use it.

> [!important] Short version
> - **Notes and images sync on their own.** Teammates see them once Najee's Obsidian has synced.
> - **The showcase page (`index.html`) does not sync by default.** Obsidian Sync skips HTML unless **Sync all other types** is turned on, on Najee's device *and* on each teammate's device.
> - **The code (`gutguard-ui`) is not in the vault**, so it does not sync at all. See [[#Getting the code]].

---

## 1. What changed

| Where in the vault | What | Syncs by default? |
|---|---|---|
| `GutGuard UI Library/` (new folder) | [[README]], [[00 - Component Inventory]], this guide, `Components/` (43 notes), `Sections/` (10 notes) | ✅ Notes |
| `GutGuard Design System/Showcase/ui-library/` (new) | 123 screenshots (`.webp`) of every component, section and screen | ✅ Images |
| `GutGuard Design System/Showcase/index.html` | New **UI Library** part: 62 entries with phone and desktop screenshots | ❌ **HTML: needs "Sync all other types"** |
| `GutGuard Tech Stack/06 - Tailwind Bridge.md` (new) | Tailwind v4 is allowed on new apps through the GutGuard tokens | ✅ Notes |
| `GutGuard Tech Stack/` 00, 01, 03, 05, 07, `Templates/AGENTS-tech-stack`, `Systems/GEMA` | Updated to point to the Tailwind bridge | ✅ Notes |
| `GutGuard Design System/Claude outputs/Gutguard Tech Stack (2026-09-29).md` | Styling line updated | ✅ Notes |

**Not changed:** project locks and checklists (`Bien To Do/`, `One Account/`). Those projects stay on portable CSS.

**Not in the vault:** the code and the live showcase, `D:\Users\najee\Downloads\Gutguard_Components_1\gutguard-ui` on Najee's PC.

---

## 2. Owner (Najee): make sure it goes out

Obsidian Sync only uploads while Obsidian is **open** with this vault.

1. Open Obsidian on this vault and wait for the Sync icon (bottom-right status bar) to show it has finished.
2. **Settings → Sync → Selective sync → turn on "Sync all other types".** Without it, the updated `index.html` stays on this PC.
3. While there, check that **Images** is on, and that **Excluded folders** doesn't list `GutGuard UI Library` or `GutGuard Design System/Showcase`.
4. Check it went out: **Settings → Sync → Sync activity**, and look for `index.html` and the `ui-library/*.webp` files. Or open **Version history** on `Showcase/index.html`.

> [!warning] OneDrive and Obsidian Sync together
> This vault sits inside OneDrive *and* uses Obsidian Sync. Obsidian advises against running two sync services on one vault, because it can cause duplicate or conflicted files. If you see files named `… (1).md` or "conflicted copy", keep one service for the vault (Obsidian Sync) and stop OneDrive from syncing this folder.

---

## 3. Teammates: see the changes

1. Open Obsidian on the shared GutGuard vault and let Sync finish.
2. **Settings → Sync → Selective sync → turn on "Sync all other types"**, so you receive `Showcase/index.html`. On a phone or tablet, force-quit and reopen Obsidian after changing it.
3. Start with [[README]] (GutGuard UI Library). It lists every component, section and screen, with links to their notes.
4. **Open the visual showcase:** in the file explorer, right-click `GutGuard Design System/Showcase/index.html` → **Open in default app** (or *Reveal in system explorer*, then double-click it). It opens in your browser. The new part is under **UI Library** in the left menu.
5. **Building UI?** Read [[06 - Tailwind Bridge]] (Tech Stack) first.

> [!danger] Read-only
> The ownership rules still apply ([[00 - OWNER — Read only]]). Teammates read and copy; only Najee edits these folders. Suggest changes in chat, Linear or Slack.

---

## 4. Getting the code

The components themselves (Next.js + Tailwind) live in the `gutguard-ui` project, which is **not** in the vault. Until it's in a shared Git repository, teammates get it from Najee:

- **Recommended:** Najee pushes `gutguard-ui` to the team's GitHub. Then: clone → `npm install` → `npm run dev` → open http://localhost:3000.
- To use components in another app, follow `README.md` in the project, section "Using the components in another Next.js project".

---

## 5. Keeping it current (owner)

When a component, section or screen changes, refresh the screenshots and the showcase page from `gutguard-ui`:

```bash
npm run build
npx next start -p 3400
node scripts/export-obsidian-showcase.mjs
```

Then stop the server, and let Obsidian sync (step 2 above).

---

## 6. Troubleshooting

| Problem | Cause | Fix |
|---|---|---|
| Notes are there, but the showcase has no **UI Library** part | `index.html` didn't sync | Turn on **Sync all other types** on *both* devices (owner and teammate) |
| UI Library part shows broken images | `.webp` images didn't sync | Turn on **Images** in Selective sync; check `Showcase/ui-library/` exists |
| Nothing new at all | Owner's Obsidian hasn't synced yet, or a folder is excluded | Owner: open Obsidian and let it sync; check **Excluded folders** |
| Duplicate / "conflicted copy" files | OneDrive and Obsidian Sync both syncing | See the warning in section 2 |
| A file won't upload | Bigger than the plan limit (Standard 5 MB) | Not an issue today: the largest file is 431 KB |

Changing these settings later doesn't remove anything already synced. Turning on a file type only syncs from then on.

---

Reference: Obsidian Help, [Sync settings and selective syncing](https://obsidian.md/help/sync/settings).
