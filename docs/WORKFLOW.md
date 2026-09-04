# Shared Workflow

This repository is designed to let ChatGPT, Codex, and Claude Code collaborate through durable files rather than relying on shared chat history.

## Start of a task

1. Read `AGENTS.md`.
2. Read the tool-specific instruction file if applicable (`CODEX.md` or `CLAUDE.md`).
3. Read `docs/TASKS.md`, `docs/HANDOFF.md`, and any project-specific documentation relevant to the task.
4. Inspect existing files before editing them.
5. Confirm that the planned work does not expose sensitive information in this public repository.

## During a task

- Make the smallest change that solves the problem.
- Keep the repository usable after each meaningful step.
- Record durable decisions in `docs/DECISIONS.md` or the relevant project decision log.
- Update `docs/TASKS.md` when task status changes materially.
- Avoid copying chat transcripts into the repository unless they have been intentionally summarized and sanitized.

## Handoff between assistants

When work is unfinished or another assistant may continue it, update `docs/HANDOFF.md` with:

- current objective
- what has already been done
- files changed
- verification performed
- blockers or uncertainties
- exact next action

A new assistant should trust repository state over an assumed memory of another assistant's conversation.

## Completion

Before marking a task done:

1. Run relevant checks when available.
2. Review the diff or changed files for accidental secrets or personal data.
3. Update task status.
4. Update the handoff so the repository reflects the final state.
5. Keep commit messages specific to the change made.

## Destructive or high-impact changes

Do not perform broad deletion, history rewriting, mass renaming, dependency migration, or irreversible restructuring without explicit user direction. If such a change is required, explain the impact before execution and preserve a rollback path whenever practical.
