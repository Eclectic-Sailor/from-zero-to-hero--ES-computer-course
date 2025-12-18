# L29: DevSecOps and Supply Chain Basics (EO6)
**Objectives:** Dependency and secret scanning, SAST/DAST basics, SBOM idea, IaC security checklist.

## Resources
- pip-audit: https://github.com/pypa/pip-audit
- git-secrets: https://github.com/awslabs/git-secrets
- SAST vs DAST explainer: https://snyk.io/learn/sast-vs-dast/
- SBOM overview (CycloneDX project page): https://owasp.org/www-project-cyclonedx/
- IaC security cheat sheet (OWASP): https://cheatsheetseries.owasp.org/cheatsheets/Infrastructure_as_Code_Security_Cheat_Sheet.html

## Tasks
- Add dependency scanning to CI (pip-audit).
- Add secret scanning (git-secrets pre-commit hook or CI step).
- Run a linter (flake8/ruff) as part of CI.
- Write a brief note on SBOMs and when you’d generate one.

## Example to Analyze
- Why does dependency scanning belong in CI, and how do you act on findings?

## Knowledge Check
- Difference between SAST and DAST.
- Why shouldn’t secrets be in env vars committed to repo?
- What do you do when a library is flagged vulnerable?

## Exit Criteria
- CI fails on vulnerable deps or detected secrets.
- Short note explaining SBOM purpose and where it fits in the pipeline.
