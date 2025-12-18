# L32: Concurrency and Safety (EO9)
**Objectives:** Recognize races/deadlocks, use locks/queues, design idempotent handlers.

## Resources
- Concurrency primer (threads vs async): https://realpython.com/python-concurrency/
- Race condition explainer: https://en.wikipedia.org/wiki/Race_condition
- Video: Deadlocks explained (~10m): https://www.youtube.com/watch?v=mhtjLJlim7Y

## Tasks
- Python demo: create a race condition with threads incrementing a counter; fix with a Lock or Queue.
- Discuss idempotency for HTTP handlers (PUT vs POST, retry safety).
- Outline deadlock avoidance via lock ordering.

## Example Code to Analyze
```python
import threading
counter = 0
def inc():
    global counter
    for _ in range(100000):
        counter += 1
```
Why is this racy? How to fix?

## Knowledge Check
- Define race condition and deadlock.
- Why do idempotent endpoints matter in distributed systems?
- When to choose queues over locks?

## Exit Criteria
- Before/after demo showing incorrect vs fixed counts.
- Written note on an idempotent design for one endpoint.
