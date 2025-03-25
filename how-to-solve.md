# How To Solve

## High Level

### The Opening

- Brute force. Make sure it's correct with edge cases.
- Calculate time and space complexity.

### The Midgame

- Discuss trade-offs, think about [best conceivable runtime](TODO:)
- Use your own good example to test your ideas
- Ask again about constraints
- It is ok to ask for a hint

### The Endgame

- Finalize the approach and carefully implement.
- **VERIFY IT**
  
## Step By Step

### Cracking The Coding Interview

1. _**Listen**_: Pay attention to unique info ("sorted", "repeatedly")
2. _**Draw an example**_:
   1. Specific
   2. Not too small
   3. Not special case
3. _**State**_: Brute-force + time complexity
4. _**Optimize**_: **BUD** - **B**ottleneck, **U**nnecessary work, **D**uplicate work
5. _**Walk-Through**_: Understand **exactly** what your'e about to code
6. _**Implement**_: Error checks, naming
7. _**Test**_:
   1. Conceptual test- read
   2. Weird looking code- make sure every suspicious code has a reason
   3. Hotspots- Base case, integer division, null nodes in binary tree and linked lists
   4. Small tests
   5. Special cases

### Optimize step notes

1. Unused info
2. Fresh example (TODO: explain)
3. Solve incorrectly  to figure out the issue
4. Make time vs space tradeoff (maybe an extra state can help optimize)
5. Precompute (sorting, first pass)
6. Hash
7. Think about best conceivable runtime (BCR) (TODO: what do I mean by "BCR && O(1) space -> improve"?)

### When can we solve with sliding window or 2 pointers

1. If a window is a valid solution, any sub-window is a valid solution
2. If a window is an invalid solution, every containing window is an invalid solution
