# Handoff Notes

Use this file for short-lived but important context that another assistant should know before continuing work.

## Handoff format

When leaving a handoff, include:

- Current task
- What has already been done
- Files changed
- What remains
- Known risks or uncertainties
- Recommended next action

## Current handoff

**Current task:** Connect the completed shared workspace to the user's local Codex / Claude Code environment.

**Completed:**
- Repository created and connected.
- `AGENTS.md` established as the repository-wide instruction entry point.
- `CLAUDE.md` added for Claude Code-specific behavior.
- `CODEX.md` added for Codex-specific behavior.
- `docs/PROJECT_MEMORY.md`, `docs/DECISIONS.md`, and `docs/HANDOFF.md` established for durable shared context.
- `docs/TASKS.md`, `docs/WORKFLOW.md`, `docs/PRIVACY.md`, and `docs/HANDOFF_TEMPLATE.md` added.
- `projects/README.md` added to define the project workspace pattern.
- `.gitignore`, `SECURITY.md`, and a pull-request template added for safety and review discipline.
- Root `README.md` expanded into the human navigation page.
- Public-repository privacy guard is active throughout the workspace documentation.

**Remaining:**
- Clone or open `Lee-Claude/chatgpt-codex-workspace` in the user's local machine environment.
- Verify Codex reads root `AGENTS.md` and follows `CODEX.md` as directed.
- Verify Claude Code reads `CLAUDE.md` and the shared repository rules.
- Begin placing real, sanitized projects under `projects/`.

**Known risk:** This repository is public. Do not commit customer-identifiable information, credentials, confidential contracts/offers, private correspondence, banking information, or other sensitive material.

**Recommended next action:** On the user's computer, clone/open the repository and perform a small read-only verification in Codex and Claude Code before starting real project work.
