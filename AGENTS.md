# AGENTS Repository Guide

This repository provides documentation for Arch Linux maintenance tasks.
The instructions below apply to all contributions.

There is no included script; adapt these notes to fit your workflow.

## Documentation Layout

- `AGENTS_CI.md` &ndash; shows how ShellCheck and GitHub Actions lint scripts.
- `AGENTS_SYSTEM.md` &ndash; lists required system utilities.
- `AGENTS_SECURITY.md` &ndash; describes security and backup tools.

Refer to these files if you need details about dependencies or CI features.

## Contribution Workflow

1. **Create small commits** in present tense (e.g. `Add root AGENTS guide`).
2. **Include a brief body** if the commit needs more context.
3. **Run relevant checks** before committing:
   - If you maintain a shell script, execute `shellcheck` on it.
4. **Open a Pull Request** summarizing what changed and which checks ran.

## Pull Request Body

- State the motivation for the change.
- Mention any tests or ShellCheck runs.
- Reference the AGENTS files when appropriate.

---

This `AGENTS.md` is the entry point for instructions.
Other AGENTS files provide additional context.
