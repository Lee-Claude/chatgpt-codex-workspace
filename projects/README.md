# Projects

Create one subdirectory here for each substantial project that needs its own durable context.

Recommended structure:

```text
projects/
  project-name/
    README.md
    AGENTS.md        # only when project-specific rules are needed
    DECISIONS.md
    HANDOFF.md
```

## Guidelines

- Keep project names short and descriptive.
- Put shared cross-project rules in the repository root, not inside every project.
- Add a project-level `AGENTS.md` only when the project needs rules that differ from or extend the root instructions.
- Do not place customer-identifying or confidential source material here while this repository is public.
- Prefer sanitized summaries and reusable technical knowledge over raw customer documents.
