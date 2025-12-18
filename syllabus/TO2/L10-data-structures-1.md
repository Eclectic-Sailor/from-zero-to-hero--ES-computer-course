# L10: Data Structures I (EO1)
**Objectives:** Arrays/lists, stacks, queues; operations and time complexity.

## Resources
- Watch: CS50 2023 “Arrays” (~40m): https://www.youtube.com/watch?v=dpw9EHDh2bM
- Read: Stack/queue intro: https://www.geeksforgeeks.org/stack-data-structure/ and https://www.geeksforgeeks.org/queue-data-structure/

## Tasks
- Implement: dynamic array (using Python list), stack, queue in Python.
- Operations: push/pop/peek for stack; enqueue/dequeue/peek for queue.
- Complexity: label each operation’s Big-O.

## Example Code to Analyze
```python
from collections import deque
q = deque()
q.append(1); q.append(2); q.popleft()
```
Why is `deque` good for queues vs list pop(0)?

## Knowledge Check
- When is array access O(1)?
- Trade-offs: array vs linked list for insert/delete vs indexing.

## Exit Criteria
- Implementations pass simple tests for correctness.
- You can explain time complexity for each operation.
