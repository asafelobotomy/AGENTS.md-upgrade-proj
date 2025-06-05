# AGENTS_CI.md

> **Shell Script Linting & Continuous Integration**  
> _This file documents the use of ShellCheck for linting and GitHub Actions for
automated validation of maintenance scripts._

---

## 🧪 Script Linting

- **`shellcheck`**  
  A static analysis tool for shell scripts. It identifies syntax errors,
  stylistic issues, and unsafe practices in POSIX/Bash scripts.
  _Used to ensure the long-term maintainability and security of
  maintenance scripts._

### Usage

To manually check your script:

```bash
shellcheck <your_script.sh>
```

---

## GitHub Actions

This repository includes workflows for ShellCheck, Markdown linting, Proselint,
and YAML linting.
