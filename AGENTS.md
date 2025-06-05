# AGENTS Repository Guide

This repository provides documentation and examples for system maintenance tasks. The instructions below apply to all contributions.

The repository does not contain a specific maintenance script; use these files as a reference for your own solution.

## Documentation Layout

- `AGENTS_CI.md` &ndash; explains how ShellCheck and GitHub Actions lint the script.
- `AGENTS_SYSTEM.md` &ndash; lists required system utilities.
- `AGENTS_SECURITY.md` &ndash; describes security and backup tools.

Refer to these files if you need details about dependencies or CI features.

## Contribution Workflow

1. **Create small commits** using present‑tense summaries (e.g. `Add root AGENTS guide`).
2. **Include a brief body** if the commit needs more context.
3. **Run relevant checks** before committing:
   - If you maintain a shell script, execute `shellcheck` on it.
4. **Open a Pull Request** summarising what changed and what checks were run.

## Pull Request Body

- State the motivation for the change.
- Mention any tests or ShellCheck runs.
- Reference the AGENTS files when appropriate.

---

This `AGENTS.md` is the entry point for instructions. Other AGENTS files provide additional context.
