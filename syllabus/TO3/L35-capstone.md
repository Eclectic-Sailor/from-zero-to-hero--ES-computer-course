# L35: Integration Capstone (EO1–EO9)
**Objectives:** Build a full-stack-ish service combining auth, DB, caching, async, tests/CI, security/DevSecOps, ML endpoint, observability, and perf check.

## Project Outline
- Service with: DB, auth (JWT/OIDC flow if possible), caching, queue/async worker, containerization, tests, CI with scans, basic metrics/logging/tracing, health checks, small ML model endpoint (e.g., classifier), and a rollback plan.

## Resources
- FastAPI full-stack example repo (reference): https://github.com/tiangolo/full-stack-fastapi-template
- Queue examples with Celery/RQ: https://realpython.com/flask-by-example-implementing-a-redis-task-queue/
- GitHub Actions marketplace (lint/test templates): https://github.com/marketplace?type=actions
- Locust quickstart for perf: https://docs.locust.io/en/stable/quickstart.html
- Architecture diagram inspiration (C4 model intro): https://c4model.com/

## Tasks
- API + DB: CRUD + auth; parameterized SQL; validation; error handling.
- Caching: in-memory cache for a hot read path.
- Async: queue for one background job (e.g., send email or long-running compute).
- ML: reuse L20/L21 model; expose a predict endpoint.
- Security: threat model; secrets handling plan; dependency/secret scans in CI.
- DevOps: Dockerize; optional compose; GitHub Actions runs tests + scans.
- Observability: structured logs; metrics for requests/latency; simple tracing if possible.
- Perf: run a smoke load test; note p95; define an SLO-lite; have rollback steps.

## Deliverables
- Code repo with README containing: architecture diagram, setup/run steps, routes, CI status, security notes, perf snapshot, and rollback plan.
- Threat model doc (even brief) and IR checklist attached/linked.

## Knowledge Check / Demo
- Walk through auth flow, cache path, and queue usage.
- Show CI passing and what happens on a failing scan/test.
- Explain ML endpoint inputs/outputs and validation.
- Explain observability outputs (logs/metrics) and perf numbers.

## Exit Criteria
- Working service (containerized) with CI green.
- Documented architecture, security, and perf notes.
- Smoke perf test results and defined SLO target + rollback plan.
