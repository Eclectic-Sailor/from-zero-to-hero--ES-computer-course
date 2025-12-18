# L04: Big-O and Tracing (EO3)
**Objectives:** Trace small snippets and label common time complexities.

## Resources
- Read: “A Common-Sense Guide to Big O”: https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation/
- Watch: CS50 complexity clip (~15m): https://www.youtube.com/watch?v=__vX2sjlpXU

## Tasks
- Trace 5 snippets: count operations in single loops, nested loops, constant-time accesses.
- Classify: O(1), O(n), O(n^2) for given code.
- Write one O(n) and one O(n^2) function yourself (explain why).

## Example Code to Analyze
```python
def contains(target, arr):
    for x in arr:
        if x == target:
            return True
    return False
```
What is its time complexity? What about searching in a sorted list with binary search?

## Knowledge Check
- How does input size affect runtime for O(n) vs O(n^2)?
- Why do we ignore constants in Big-O?
- Give a real-life example of O(1) vs O(n).

## Exit Criteria
- You can correctly label 5/5 sample snippets with their Big-O class.
- You can explain the difference between best/average/worst case in plain terms.
