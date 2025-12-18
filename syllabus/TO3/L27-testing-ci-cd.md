# L27: Testing and CI/CD (EO5, EO6)
**Objectives:** Unit/integration tests, handling flakiness, CI pipeline with gates.

## Resources
- Pytest getting started: https://docs.pytest.org/en/stable/getting-started.html
- JUnit 5 user guide: https://junit.org/junit5/docs/current/user-guide/
- GitHub Actions Python example: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python

## Tasks
- Add unit tests for core logic; one integration test hitting a live endpoint or DB (with test DB).
- Run tests locally; ensure deterministic behavior (no time/random without seeding).
- Create GitHub Actions workflow to run tests on push; fail on lint/test errors.

## Example to Analyze
```yaml
name: ci
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: actions/setup-python@v4
        with: { python-version: '3.11' }
      - run: pip install -r requirements.txt
      - run: pytest
```
What happens when a test fails?

## Knowledge Check
- Difference between unit and integration tests.
- How to reduce flaky tests?
- Why automate tests in CI?

## Exit Criteria
- Tests pass locally and in CI.
- CI fails when tests fail; you know where to view logs.
