# L03: Python from Zero II (EO2)
**Objectives:** Lists, dicts, functions, errors; small log parser.

## Resources
- Read: ATBS ch.4 (lists) and ch.5 (dicts): https://automatetheboringstuff.com/2e/chapter4/ and https://automatetheboringstuff.com/2e/chapter5/
- Review: ATBS ch.3 functions: https://automatetheboringstuff.com/2e/chapter3/
- Video: Corey Schafer Python lists/dicts (YouTube): https://www.youtube.com/watch?v=9oKlZJjq-xc

## Tasks
- Mini-exercises:
  - Sum of list, max of list.
  - Word count from a string using dict.
  - Menu program that maps commands to actions.
- Write a function per exercise; add basic error handling (try/except).
- Build: simple log parser—given lines like `INFO 2024-01-01 something`, count levels (INFO/WARN/ERROR) with a dict and print totals.

## Example Code to Analyze
- A function with default argument pitfall:
```python
def append_item(item, bucket=[]):
    bucket.append(item)
    return bucket
```
Why can this be dangerous? How to fix it?

## Knowledge Check
- How to add/remove items from list and dict?
- Why prefer `if __name__ == "__main__":` guard?
- Explain mutability of lists vs immutability of tuples.

## Exit Criteria
- Log parser runs on a sample file and prints counts.
- You can explain why mutable defaults are risky and show the correct pattern.
