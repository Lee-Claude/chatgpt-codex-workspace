# Codex Instructions

Codex should treat `AGENTS.md` as the primary repository-wide instruction file. This document adds Codex-specific execution guidance and does not replace `AGENTS.md`.

## Codex-specific workflow

1. Read `AGENTS.md` first, then read this file before making substantive repository changes.
2. Inspect the current implementation and relevant neighboring files before editing.
3. Prefer the smallest change that fully satisfies the request; avoid unrelated cleanup.
4. Preserve working behavior, interfaces, file structure, and user-authored content unless the task explicitly requires changing them.
5. Do not perform broad refactors, dependency upgrades, migrations, mass formatting, or file deletion unless explicitly requested or clearly required.
6. When changes affect executable code, run the narrowest relevant checks available, then broader checks only when useful.
7. If a check cannot be run, say so explicitly rather than claiming validation.
8. Keep intermediate states recoverable and commits focused.
9. At completion, summarize: files changed, key decisions, checks performed, and any remaining risks or follow-up items.

## Cross-assistant handoff

- Treat repository documents as durable shared context between ChatGPT, Codex, and Claude Code.
- Do not assume access to another assistant's conversation history.
- Record durable decisions or handoff notes in repository files when they are needed by another assistant later.
- Avoid creating duplicate instruction sources; shared rules belong in `AGENTS.md`.

## Public repository caution

This repository is public. Before committing user, customer, company, credential, contract, quotation, invoice, or other potentially confidential material, apply the privacy guard in `AGENTS.md`. If sensitive content is detected, stop and warn the user before committing it.
