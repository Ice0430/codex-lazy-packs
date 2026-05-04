---
name: shutdown-sync
description: End work by summarizing changes, updating the project note, checking Git diff, and optionally committing and pushing.
---

# Shutdown Sync

Use when the user says 收工, 結束工作, shutdown sync, or asks to wrap up a project.

## Workflow

1. Check `git status -sb` and inspect the diff.
2. Summarize what changed and what was verified.
3. Update the linked Obsidian project note when useful.
4. Commit and push only when the user asks or the project workflow explicitly requires it.
5. Mention unresolved risks or manual follow-up.

## Safety

- Never stage unrelated files silently.
- Never commit secrets, tokens, `.env`, `.codex`, or private config.
- Keep the wrap-up concise and factual.
