# Local Setup

This repository is ready on GitHub. The remaining step is to open the same repository on the computer where Codex and Claude Code run.

Repository URL:

```text
https://github.com/Lee-Claude/chatgpt-codex-workspace.git
```

## macOS / Linux

```bash
git clone https://github.com/Lee-Claude/chatgpt-codex-workspace.git
cd chatgpt-codex-workspace
```

If the repository was already cloned:

```bash
cd chatgpt-codex-workspace
git pull --ff-only
```

## Windows PowerShell

```powershell
git clone https://github.com/Lee-Claude/chatgpt-codex-workspace.git
Set-Location chatgpt-codex-workspace
```

If the repository was already cloned:

```powershell
Set-Location chatgpt-codex-workspace
git pull --ff-only
```

## Codex verification

Open Codex with this repository as the working directory. Before asking it to modify anything, use a read-only check such as:

```text
Read the repository instructions and tell me which instruction files and shared task-context files apply. Do not modify anything.
```

A correct response should recognize `AGENTS.md` as the primary repository instruction entry point and should also follow its direction to read `CODEX.md` plus the relevant shared context files.

## Claude Code verification

Open Claude Code from this repository directory. Use a read-only check such as:

```text
Read the repository instructions and summarize the rules that apply before making changes. Do not modify anything.
```

A correct response should use `CLAUDE.md` together with the shared rules in `AGENTS.md` and should recognize the public-repository privacy guard.

## First real project

For substantial work, create a sanitized project directory under:

```text
projects/<project-name>/
```

Do not copy raw customer documents, contracts, quotations, credentials, personal information, or confidential company material into this public repository. Use sanitized summaries or a private repository for sensitive work.

## Normal synchronization

Before starting work on another machine or with another tool:

```bash
git pull --ff-only
```

After reviewed changes are committed locally:

```bash
git push
```

The repository files—not prior chat history—should be treated as the durable cross-tool context.
