# Bucket Sort

## Overview

Bucket sort is a sorting technique that involves dividing elements into various groups, or buckets. These buckets are formed by uniformly distributing the elements. Once the elements are divided into buckets, they can be sorted using any other sorting algorithm. Finally, the sorted elements are gathered together in an ordered fashion.

## Algorithm Steps

Create n empty buckets and for every element in the array:

1. Insert into bucket
2. Sort individual bucket
3. Concatenate all sorted buckets

## Prerequisites (When to Use Bucket Sort)

1. **Uniform Distribution**:
   - The input data must be uniformly distributed over a known range (e.g. [0, 1) or [0, k])
   - This ensures elements are spread evenly across buckets

2. **Known Range**:
   - You need to know the min and max values of the data beforehand to create appropriate buckets

## Time Complexity Analysis

### Average Case: O(n)

While the worst case is O(n²), the average time complexity of O(n) is achieved because:

- Splitting n elements into k buckets (where k ≈ n) takes O(n)
- Inserting into buckets is O(1) per element (assuming ideal distribution)
- Sorting each bucket is fast: if each bucket has a few items, insertion sort is efficient
- Combining all buckets takes O(n)

Therefore, when:

- The data is uniformly distributed
- The number of buckets is proportional to n
- The sort inside each bucket is fast (like insertion sort)

Total = O(n) (distribution) + O(n) (in-bucket sorts) + O(n) (concatenation) → O(n)

## Requirements Table

| Requirement          | Why It Matters                                  |
| -------------------- | ----------------------------------------------- |
| Uniform distribution | Ensures even bucket fill → faster sorting       |
| Known value range    | Allows correct bucket placement                 |
| Small buckets        | Enables fast in-bucket sorting (e.g. insertion) |
| Proper bucket count  | Prevents overloading a single bucket            |

## Example Problems

1. [Top K Frequent Elements](https://leetcode.com/problems/top-k-frequent-elements/description/)
