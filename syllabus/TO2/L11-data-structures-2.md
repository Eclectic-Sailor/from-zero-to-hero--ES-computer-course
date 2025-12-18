# L11: Data Structures II (EO1)
**Objectives:** Hash maps/sets, collision handling, sorting basics.

## Resources
- Watch: CS50 Hash Tables segment: https://www.youtube.com/watch?v=UOxTMOCTEZk
- Read: Hashing data structure intro (collisions/chaining): https://www.geeksforgeeks.org/hashing-data-structure/

## Tasks
- Implement: simple hash map in Python using list of buckets (chaining).
- Implement: insertion sort or selection sort; measure on small lists.
- Discuss: load factor and when to resize.

## Example Code to Analyze
```python
def simple_hash(key, size):
    return hash(key) % size
```
What makes a good hash? Why mod by table size?

## Knowledge Check
- How do collisions happen and how do you handle them?
- Complexity of successful lookup in a hash map (average vs worst).
- Why are built-in dict/set in Python generally O(1) average?

## Exit Criteria
- Hash map get/put/delete works for collisions.
- You can explain how sorting affects complexity vs built-in `sorted`.
