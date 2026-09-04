# Decision Log

Record durable decisions that affect future work in this repository.

For each decision, capture:

- Date
- Decision
- Why it was made
- Alternatives considered when relevant
- Consequences or follow-up actions

## Decisions

### 2026-09-04 — Use one shared repository as the durable coordination layer

**Decision:** Use this GitHub repository as the persistent shared context for ChatGPT, Codex, and Claude Code.

**Reason:** The assistants do not reliably share conversation history with one another, while repository files can provide a durable source of truth.

**Consequence:** Important cross-tool rules, decisions, and handoff notes should be written into this repository when they need to persist.

### 2026-09-04 — Keep the repository public with a privacy guard

**Decision:** Keep this repository public for easier sharing and review.

**Reason:** The user wants to be able to share the workspace with other people for reference and review.

**Consequence:** Sensitive or identifiable customer/company information must not be committed without explicit confirmation that it is safe for public release. Redact, exclude, or move such work to a private repository when necessary.
