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

**Current task:** Build the shared ChatGPT / Codex / Claude Code workspace foundation.

**Completed:**
- Repository created and connected.
- `AGENTS.md` added as the repository-wide rules file.
- `CLAUDE.md` added for Claude Code-specific behavior.
- `CODEX.md` added for Codex-specific behavior.
- Public-repository privacy guard established.
- Shared project memory and decision log created under `docs/`.

**Remaining:**
- Add task-tracking conventions.
- Improve README so humans understand the workspace structure.
- Add ignore/safety defaults where useful.
- Later connect or clone this repository into the user's local Codex / Claude Code environment.

**Risk:** This repository is public. Do not commit customer-identifiable, confidential, credential, or secret material.
