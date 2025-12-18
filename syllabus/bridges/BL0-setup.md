# BL0: Tooling Setup
**Goal:** Ready-to-work environment (editor, shell, Git, Python, HTTP client, GitHub).

## Resources
- VS Code install docs: https://code.visualstudio.com/download
- Git install: https://git-scm.com/downloads
- Python 3.x: https://www.python.org/downloads/
- httpie (or curl if already present): https://httpie.io/cli
- (Optional) WSL on Windows: https://learn.microsoft.com/windows/wsl/install

## Tasks
- Install VS Code + Git + Python 3.x + httpie (or verify versions).
- Verify: `git --version`, `python3 --version`, `pip --version`, `http` (or `curl --version`).
- Configure Git: `git config --global user.name "Your Name"` and `git config --global user.email you@example.com`.
- Create/verify GitHub account; set up SSH key (GitHub docs) or HTTPS auth.
- Create a test repo locally (`git init bl0-setup`), add a README, commit, and push to GitHub.

## Knowledge Check
- Show `git status` after modifying a file; explain what `git add` does.
- Explain the difference between `>` and `>>` in the shell.

## Exit Criteria
- You can clone/pull/push a repo.
- `python3` runs; `http example.com` (or `curl -I example.com`) succeeds.
- You have a working editor with syntax highlighting for Python/C/Java.
