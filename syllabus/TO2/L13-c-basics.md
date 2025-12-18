# L13: C Basics (EO2)
**Objectives:** Compile/run C; use pointers, arrays/strings, structs, basic file I/O.

## Resources
- Watch: CS50 “Memory”/“Pointers”: https://www.youtube.com/watch?v=QcE-ycZk-HM
- Read: Beej’s Guide to C (intro/pointers/strings): https://beej.us/guide/bgc/

## Tasks
- Install/verify gcc/clang: `gcc --version`.
- Write programs for:
  - Read stdin and echo lines.
  - Array iteration; pointer arithmetic demo.
  - Struct with fields; function that takes struct pointer.
  - File I/O: open/read file, count lines.
- Compile with `gcc -Wall -Wextra -o prog file.c`.

## Example Code to Analyze
```c
int nums[3] = {1,2,3};
int *p = nums;
printf("%d %d\n", *(p+1), nums[1]);
```
Why are these equivalent? What could make them differ?

## Knowledge Check
- Difference between stack vs heap allocation.
- What happens if you free memory you didn’t malloc?
- Why must you check return values (e.g., fopen)?

## Exit Criteria
- Programs compile without warnings.
- You can explain and demonstrate pointer dereference and address-of operator.
