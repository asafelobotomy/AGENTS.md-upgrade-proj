# AGENTS_CI.md

> **Shell Script Linting & Continuous Integration**  
> _This file documents the use of ShellCheck for linting and GitHub Actions for
automated validation of shell scripts and documentation._

---

## 🧪 Script Linting

- **`shellcheck`**  
  A static analysis tool for shell scripts. It identifies syntax errors,
  stylistic issues, and unsafe practices in POSIX/Bash scripts.
  _Used to ensure the long-term maintainability and security._

### Usage

To manually check your script:

```bash
shellcheck <your_script.sh>
```

---

## GitHub Actions

This repository includes workflows for ShellCheck, Markdown linting, Proselint,
and YAML linting.

- [YAML Lint Workflow](.github/workflows/yamllint.yml)
- [Markdown Lint Workflow](.github/workflows/markdownlint.yml)
- [Proselint Workflow](.github/workflows/proselint.yml)

Make sure to run these checks locally if possible before pushing changes. All pull requests should pass the automated checks for code quality and documentation standards.
