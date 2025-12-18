# L26: 12-Factor and Configuration (EO4, EO5)
**Objectives:** Externalized config, stateless services, logs as streams, health checks.

## Resources
- Read: Twelve-Factor App: https://12factor.net/ (focus on Config, Logs, Processes, Concurrency).
- Health checks (readiness/liveness) official K8s docs: https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/

## Tasks
- Externalize app config via environment variables (DB URL, secrets placeholder).
- Add `/health` endpoint to your API; return status OK if dependencies reachable.
- Ensure logs go to stdout in structured form (timestamp, level, message).

## Example to Analyze
```python
import os
DB_URL = os.environ.get("DB_URL", "sqlite:///local.db")
```
Why prefer env vars over checked-in config?

## Knowledge Check
- What makes a service “stateless” in 12-factor terms?
- Difference between liveness and readiness checks?
- Why avoid baking secrets into images?

## Exit Criteria
- App runs with config set via env vars.
- Health endpoint works; logs are stdout-friendly and structured.
