# L33: Advanced Algorithms Intuition (EO9)
**Objectives:** Understand approximate/randomized structures; implement a simple Bloom filter; discuss trade-offs.

## Resources
- Bloom filter explainer: https://llimllib.github.io/bloomfilter-tutorial/
- Bloom filter overview (Wikipedia): https://en.wikipedia.org/wiki/Bloom_filter
- Video: Probabilistic data structures (~12m): https://www.youtube.com/watch?v=IGSOjNTmGpo

## Tasks
- Implement a simple Bloom filter in Python with k hash functions (can use built-in hash variants).
- Demonstrate false positives; measure rate for small tests.
- Discuss when to use Bloom filters vs exact sets.

## Example Code to Analyze
```python
import mmh3  # or built-in hash variants
```
Why multiple hashes? How do false positives arise?

## Knowledge Check
- What trade-off do Bloom filters make?
- Can they have false negatives?
- Where might approximate structures be useful?

## Exit Criteria
- Bloom filter demo works and shows false positives.
- Short note on when you’d pick approximate vs exact.
