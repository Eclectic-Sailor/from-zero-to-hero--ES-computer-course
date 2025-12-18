# L12: Graphs and Traversals (EO1)
**Objectives:** Represent graphs; implement BFS and DFS; shortest path in unweighted graphs.

## Resources
- Watch: MIT OCW 6.006 BFS/DFS lecture: https://www.youtube.com/watch?v=AfYqN3fGapc
- Read: Adjacency list vs matrix primer: https://www.geeksforgeeks.org/graph-and-its-representations/

## Tasks
- Implement adjacency list representation.
- Implement BFS and DFS; record traversal order.
- Solve: shortest path (fewest edges) in unweighted graph using BFS.

## Example Code to Analyze
```python
from collections import deque
def bfs(graph, start):
    seen = set([start]); q = deque([start]); order = []
    while q:
        node = q.popleft(); order.append(node)
        for nei in graph[node]:
            if nei not in seen:
                seen.add(nei); q.append(nei)
    return order
```
Why does BFS find shortest path in edge count?

## Knowledge Check
- When to choose BFS vs DFS?
- Complexity of BFS/DFS in terms of V and E.
- How would you detect a cycle?

## Exit Criteria
- BFS/DFS functions work on sample graphs.
- You can find and output a shortest path (list of nodes) in an unweighted graph.
