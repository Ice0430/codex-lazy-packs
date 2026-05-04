---
name: project-init-sync
description: Initialize a classroom tool project with AGENTS.md, README, .gitignore, Obsidian project note, Git/GitHub linkage, and optional Firebase references.
---

# Project Init Sync

Use when the user says 初始化班級工具工作模式, 初始化專案, or asks to set up a classroom tool workspace.

## Workflow

1. Inspect the existing folder before creating anything.
2. Preserve existing app logic and config.
3. Create or update `AGENTS.md` with project paths, repo URL, Obsidian note path, Firebase project ID, and start/shutdown rules.
4. Ensure `.gitignore` protects secrets and local agent config.
5. Create or update a concise `README.md`.
6. Create an Obsidian project note under the configured vault when available.
7. Check GitHub remote and Firebase project status when relevant.
8. Commit and push only after reviewing the exact file scope.

## Safety

- Do not delete, move, or rewrite existing notes broadly.
- Do not commit API keys, service account files, tokens, `.env`, `.codex`, or `.claude`.
- Use `npx.cmd` for Firebase commands on Windows PowerShell.
