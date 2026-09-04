# ChatGPT × Codex × Claude Code Workspace

A public shared workspace for durable coordination between ChatGPT, OpenAI Codex, and Claude Code.

The repository is intentionally lightweight: shared rules live at the root, durable context lives under `docs/`, and substantial work can be organized under `projects/`.

## Start here

1. Read [`AGENTS.md`](AGENTS.md) — repository-wide rules for every assistant.
2. If using Codex, also read [`CODEX.md`](CODEX.md).
3. If using Claude Code, also read [`CLAUDE.md`](CLAUDE.md).
4. Check [`docs/TASKS.md`](docs/TASKS.md) for current work.
5. Check [`docs/HANDOFF.md`](docs/HANDOFF.md) before continuing work started by another assistant.
6. Read [`docs/PRIVACY.md`](docs/PRIVACY.md) before adding customer, company, credential, or potentially sensitive material.
7. Use [`docs/LOCAL_SETUP.md`](docs/LOCAL_SETUP.md) to connect the repository to the local Codex / Claude Code environment.

## Repository structure

```text
.
├── AGENTS.md                  # Shared rules / primary instruction entry point
├── CODEX.md                   # Codex-specific behavior
├── CLAUDE.md                  # Claude Code-specific behavior
├── SECURITY.md                # Sensitive-data incident guidance
├── .gitignore                 # Local secret and noise exclusions
├── .github/
│   └── PULL_REQUEST_TEMPLATE.md
├── docs/
│   ├── PROJECT_MEMORY.md      # Durable non-sensitive background
│   ├── DECISIONS.md           # Important decisions and rationale
│   ├── TASKS.md               # Shared lightweight task board
│   ├── HANDOFF.md             # Current cross-assistant handoff
│   ├── HANDOFF_TEMPLATE.md    # Standard handoff format
│   ├── WORKFLOW.md            # Shared operating workflow
│   ├── PRIVACY.md             # Public-repository privacy rules
│   └── LOCAL_SETUP.md         # Local Codex / Claude Code connection guide
└── projects/
    └── README.md              # Convention for project-specific workspaces
```

## Working model

GitHub is the durable source of truth. ChatGPT, Codex, and Claude Code should not assume they share conversation history. Important context that must survive across tools should be written into repository files after being sanitized for public release.

For a new task, read the rules and current handoff, inspect existing files, make the smallest safe change, run relevant checks, then update the task board and handoff if the state changed materially.

## Public repository warning

**Everything committed here should be treated as public.** Do not commit API keys, passwords, tokens, private keys, customer-identifying data, contracts, quotations, invoices, banking information, private correspondence, or confidential company/third-party material unless it has been deliberately sanitized and approved for public release.

Deleting a file later does not automatically erase it from Git history. See [`docs/PRIVACY.md`](docs/PRIVACY.md) and [`SECURITY.md`](SECURITY.md).

## Project folders

For substantial work, create a directory under `projects/`. Add a more specific `AGENTS.md` only when that project genuinely needs additional or overriding instructions.

## Current state

The GitHub-side shared-workspace bootstrap is complete and verified. The remaining practical step is local-machine setup: clone or open this repository inside Codex / Claude Code and run the read-only checks in [`docs/LOCAL_SETUP.md`](docs/LOCAL_SETUP.md).
