# Claude Code Instructions

Claude Code should treat `AGENTS.md` as the shared repository-wide source of truth and follow it before making changes.

## Claude-specific workflow

1. Read `AGENTS.md` first, then read the files directly relevant to the requested task.
2. Do not duplicate shared rules from `AGENTS.md` here; this file is only for Claude Code behavior.
3. Before editing, inspect the current implementation and identify the smallest safe change.
4. Prefer editing existing files over creating parallel or duplicate versions unless a new file is clearly required.
5. Do not perform broad refactors, dependency upgrades, migrations, or deletions unless the task explicitly calls for them.
6. When a task spans multiple steps, keep the repository in a usable state after each meaningful step.
7. Run relevant checks when available and report what was changed, what was verified, and any remaining uncertainty.

## Coordination

- Repository files are the durable shared context between Claude Code, Codex, and ChatGPT.
- Do not assume access to conversations from the other assistants.
- Put durable project decisions, conventions, and handoff notes into repository files when they need to persist across tools.
- If a tool-specific instruction conflicts with a more specific instruction in a subdirectory, follow the more specific instruction for that scope unless it would violate a higher-priority safety or privacy rule.

## Public repository caution

This repository is public. Apply the privacy and sensitive-data rules in `AGENTS.md` before committing any user, customer, company, credential, or confidential material.
