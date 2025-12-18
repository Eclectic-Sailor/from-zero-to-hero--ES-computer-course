# BL2: Binary/Hex, Memory, and Pointer Concepts (Pre-C)
**Purpose:** Bridge from Python to C by understanding representation and pointers.

## Resources
- Binary/hex primer: https://web.stanford.edu/class/cs101/bits-bytes.html
- CS50 “Memory”/pointers segment: https://www.youtube.com/watch?v=QcE-ycZk-HM

## Tasks
- Convert numbers: binary ↔ decimal ↔ hex (e.g., 13, 42, 255).
- Draw memory boxes for: an `int x = 5; int *p = &x;` and a pointer to pointer `int **pp = &p;`.
- Explain what lives at an address vs what the pointer variable stores.
- Write a tiny C snippet that declares an int, a pointer to it, prints the value and the address; compile with `gcc -Wall -Wextra`.

## Knowledge Check
- What does `&` do in `int *p = &x;`?
- Why is `*p` different from `p`?
- What happens if you dereference an uninitialized pointer?

## Exit Criteria
- You can read and explain a simple pointer declaration and dereference in C.
- You can convert small numbers between binary/hex/decimal without a calculator.
