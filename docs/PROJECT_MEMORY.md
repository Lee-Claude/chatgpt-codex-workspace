# Project Memory

This file stores durable, non-sensitive context that should persist across ChatGPT, Codex, and Claude Code sessions.

## What belongs here

- Stable project goals
- Important architecture or workflow context
- Long-lived conventions
- Reusable background information needed by multiple assistants

## What does not belong here

Because this repository is public, do not store customer-identifiable information, private company data, secrets, API keys, credentials, unpublished financial data, contracts, quotations, invoices, or other confidential material here.

## Current shared context

- This repository is intended to act as a shared workspace for ChatGPT, Codex, and Claude Code.
- Repository-level operating rules live in `AGENTS.md`.
- Tool-specific behavior lives in `CODEX.md` and `CLAUDE.md`.
- Durable information should be written into repository files rather than relying on assistant chat history.
