# Workspace Rules

This repository is a shared workspace for ChatGPT, Codex, and Claude Code.

## Core operating rules

1. Read this file before making repository changes.
2. Prefer small, reversible changes over broad rewrites.
3. Preserve existing working behavior unless the task explicitly requires changing it.
4. Before modifying an existing file, inspect the current file first.
5. Do not delete or overwrite user-authored content unless explicitly required.
6. When requirements are ambiguous, state the assumption or ask before making a destructive change.
7. Keep commits focused and use clear commit messages.

## Public-repository privacy guard

This repository is PUBLIC.

Never commit any of the following unless the user has explicitly confirmed that the content is safe for public release:

- API keys, access tokens, passwords, private keys, secrets, credentials, or recovery codes
- Customer names, personal addresses, phone numbers, email addresses, IDs, banking data, signatures, or other personal data
- Customer contracts, quotations, invoices, internal commercial documents, or confidential project files containing identifiable data
- Private company data, unpublished financial information, or confidential third-party material

If potentially sensitive material is detected, stop before committing it and warn the user. Recommend one of these options: redact/anonymize the data, exclude the file from Git, or move the work to a private repository.

## Coordination between assistants

- Treat repository files as the durable source of truth for project-specific instructions.
- Do not assume another assistant has seen prior chat history unless that information has been written into the repository.
- Record durable project decisions in an appropriate repository document rather than relying only on conversation history.
- Avoid duplicating the same rule across many files. Keep shared rules here and tool-specific rules in their dedicated files when needed.

## Scope

More specific AGENTS.md files placed in subdirectories may add or override instructions for files inside those directories.
