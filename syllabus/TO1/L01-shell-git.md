# L01: Shell and Git Fundamentals (EO1)
**Objectives:** Navigate, chain commands, and use Git basics.

## Resources
- Read: “The Linux Command Line” ch.1–3: http://linuxcommand.org/tlcl.php
- Watch: NetworkChuck “Linux for Hackers” (~20m): https://www.youtube.com/watch?v=chPhlsHoEPo
- Git Basics (recording changes): https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository

## Tasks
- Shell: run `ls`, `pwd`, `cd`, `cat`, `less`, `head`, `tail`; practice pipes `cat file | grep word`; redirects `>` vs `>>`.
- Git: `git init`, `git status`, `git add/commit`, `git log`; create a repo, add README, commit.
- Remote: create a GitHub repo, set origin, `git push`, clone it elsewhere to verify.

## Example Code to Analyze
- Inspect a `.gitignore` (e.g., Python template) and identify why entries exist.

## Knowledge Check
- Difference between `>` and `>>`?
- What does `git add` do vs `git commit`?
- How to undo last commit while keeping changes (`git reset --soft HEAD~1`)?

## Exit Criteria
- You have a repo on GitHub with at least one commit.
- You can show `git status` clean after changes are committed.
- You can pipe two commands and redirect output to a file.
