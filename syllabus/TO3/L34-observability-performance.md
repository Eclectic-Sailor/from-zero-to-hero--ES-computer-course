# L34: Observability and Performance (EO8)
**Objectives:** Logging/metrics/tracing basics; RED/USE thinking; simple load test and profiling.

## Resources
- Observability primer (logs/metrics/traces): https://thenewstack.io/what-is-observability/
- RED method overview: https://grafana.com/blog/2019/03/27/the-red-method-how-to-instrument-your-services/
- Locust load testing: https://locust.io/
- Autocannon CLI: https://github.com/mcollina/autocannon

## Tasks
- Add structured logging (JSON-like) and metrics (request count/latency) to your API.
- Run a small load test; capture p50/p95/p99 latencies.
- Identify one hotspot and profile with basic timing; attempt a small optimization or cache.

## Example to Analyze
- What’s the difference between p95 and average latency, and why does it matter?

## Knowledge Check
- Why logs, metrics, and traces all matter.
- What is an SLO/error budget conceptually?
- How to avoid logging sensitive data?

## Exit Criteria
- Metrics/structured logs present; load test results recorded.
- You can explain p95/p99 and one performance finding.
