# L24: Caching and Performance (EO3, EO8)
**Objectives:** Cache strategies, eviction/stampede prevention, basic perf testing and timing.

## Resources
- Caching strategies overview: https://aws.amazon.com/caching/
- Perf testing primer (TTFB/latency): https://www.section.io/engineering-education/understanding-ttfb/
- Guided cache example in Python (Flask + cache): https://realpython.com/flask-by-example-implementing-a-redis-task-queue/ (focus on caching parts)

## Tasks
- Add an in-memory cache to a small service (or mock) with TTL and eviction policy.
- Measure before/after latency on a hot endpoint (simple timing loop).
- Discuss stampede prevention (lock per key or jitter).

## Example to Analyze
```python
cache = {}
def get_item(key):
    if key in cache:
        return cache[key]
    val = expensive()
    cache[key] = val
    return val
```
What happens under concurrency? How to protect?

## Knowledge Check
- Why caches can make writes tricky (stale/invalidation)?
- What is p99 latency?
- How to avoid cache stampede?

## Exit Criteria
- Timing results (before vs after cache).
- Short note on eviction choice and stampede mitigation.
