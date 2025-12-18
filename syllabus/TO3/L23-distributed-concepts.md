# L23: Distributed Systems Concepts (EO3)
**Objectives:** CAP, replication/partitioning, leader election intuition (Raft), idempotency/backpressure.

## Resources
- CAP theorem explainer: https://mwhittaker.github.io/blog/an_illustrated_proof_of_the_cap_theorem/
- Raft visual summary (~10m): https://thesecretlivesofdata.com/raft/
- Queue/backpressure primer: https://sre.google/sre-book/load-balancing-frontend/#backpressure-d4r9r

## Tasks
- Design exercise: sketch read/write paths for a replicated service (leader/followers).
- Define how you ensure idempotency for a write endpoint.
- Describe how you’d handle backpressure when queue grows (drop? buffer? throttle?).

## Example to Analyze
- Why might you choose quorum reads/writes? Trade-offs vs single-leader reads.

## Knowledge Check
- What does CAP actually say?
- When do partitions effectively happen?
- How does idempotency help retries?

## Exit Criteria
- One-page design note with CAP stance, replication strategy, idempotent handler, and backpressure plan.
