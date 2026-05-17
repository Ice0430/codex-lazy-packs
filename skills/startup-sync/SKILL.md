---
name: startup-sync
description: Start work in a project by reading AGENTS.md, checking Git state, reviewing linked Obsidian notes, and confirming external service status before making changes.
---

# Startup Sync

Use when the user says 開始工作, 開工, 啟動同步, or wants to resume a project.

## Workflow

1. Read the project `AGENTS.md` first.
2. Check `git status -sb` and current branch.
3. Pull only when the user asks or the project instructions explicitly require it.
4. Read the linked Obsidian project note if one is listed in `AGENTS.md`.
5. Read the project's durable write-back targets from `AGENTS.md`; by default these are Firebase, Obsidian, and GitHub when the project has them.
6. Check Firebase/GitHub status only if the current task depends on them.
7. Report a concise current-state summary and continue the requested work.

## Safety

- Do not overwrite user changes.
- Do not commit or push unless requested or required by the current workflow.
- Prefer project-local instructions over generic assumptions.
