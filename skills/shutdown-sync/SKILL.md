---
name: shutdown-sync
description: End work by summarizing changes, updating the project note, checking Git diff, and optionally committing and pushing.
---

# Shutdown Sync

Use when the user says 收工, 結束工作, shutdown sync, or asks to wrap up a project.

## Workflow

1. Check `git status -sb` and inspect the diff.
2. Summarize what changed and what was verified.
3. Decide which durable findings, pitfalls, or project-state changes should be written back to Firebase, Obsidian, and GitHub according to the project `AGENTS.md`.
4. Update the linked Obsidian project note when useful, and update Firebase/GitHub when the project rules call for those write-backs.
5. Commit and push only when the user asks or the project workflow explicitly requires it.
6. Mention unresolved risks or manual follow-up.

## Safety

- Never stage unrelated files silently.
- Never commit secrets, tokens, `.env`, `.codex`, or private config.
- Keep the wrap-up concise and factual.
