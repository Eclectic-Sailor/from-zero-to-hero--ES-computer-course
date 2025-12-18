# L02: Python from Zero I (EO2)
**Objectives:** Variables, types, input/output, conditionals, loops; build a small game.

## Resources
- Read: Automate the Boring Stuff (ATBS) ch.1–2: https://automatetheboringstuff.com/2e/chapter1/
- Watch: NetworkChuck Python beginner (~20m): https://www.youtube.com/watch?v=rfscVS0vtbw
- Guided practice: Exercism Python track: https://exercism.org/tracks/python

## Tasks
- REPL: practice ints, floats, strings, booleans; `type()`; simple arithmetic.
- Write “guess the number” game: random number 1–20, prompt user until correct; count attempts.
- Add input validation: handle non-int input without crashing (try/except).

## Example Code to Analyze
- A simple conditional chain:
```python
x = 7
if x > 10:
    print("big")
elif x > 5:
    print("medium")
else:
    print("small")
```
Trace output and why.

## Knowledge Check
- Difference between `while` and `for` loops?
- What happens if you compare string to int in Python?
- Show how to import and use `random.randint`.

## Exit Criteria
- Game runs, handles bad input gracefully, and reports attempts.
- You can explain how the loop stops.
