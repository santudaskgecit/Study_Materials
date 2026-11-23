# DSA Interview Question Bank (Java)

A curated practice list for senior backend/software engineering interviews at FAANG and strong product companies. Use Java as the implementation language.

**Target:** Complete the 70 core problems over 12 weeks, then work through the stretch set. The aim is to build pattern recognition, implementation fluency and clear interview communication—not to maximize the number of solved problems.

## How to use this question bank

For every problem:
1. Read the constraints and clarify assumptions.
2. Explain a brute-force approach first, then optimize it.
3. State time and space complexity before coding.
4. Implement in Java without AI or autocomplete assistance on the first attempt.
5. Test edge cases: empty input, one element, duplicates, negative values, overflow and boundary conditions where relevant.
6. Record the pattern, key insight and mistake (if any).
7. Re-solve after 1, 7 and 21 days without looking at the previous solution.

**Suggested attempt limits:** Easy: 20–25 minutes; Medium: 30–40 minutes; Hard: 45 minutes before taking a hint. After viewing a hint or solution, close it and implement independently.

## Core question set (70 problems)

### 1. Arrays, strings and hashing — 12

| # | Problem | Level | Main pattern |
|---:|---|---|---|
| 1 | Two Sum | Easy | HashMap |
| 2 | Contains Duplicate | Easy | HashSet |
| 3 | Valid Anagram | Easy | Frequency counting |
| 4 | Best Time to Buy and Sell Stock | Easy | One-pass tracking |
| 5 | Product of Array Except Self | Medium | Prefix/suffix |
| 6 | Maximum Subarray | Medium | Kadane's algorithm |
| 7 | Group Anagrams | Medium | Canonical key / hashing |
| 8 | Top K Frequent Elements | Medium | Frequency map + heap/bucket |
| 9 | Longest Consecutive Sequence | Medium | HashSet |
| 10 | Encode and Decode Strings | Medium | String encoding |
| 11 | Valid Sudoku | Medium | Sets / validation |
| 12 | Subarray Sum Equals K | Medium | Prefix sum + HashMap |

### 2. Two pointers and sliding window — 8

| # | Problem | Level | Main pattern |
|---:|---|---|---|
| 13 | Valid Palindrome | Easy | Two pointers |
| 14 | Two Sum II – Input Array Is Sorted | Medium | Two pointers |
| 15 | 3Sum | Medium | Sorting + two pointers |
| 16 | Container With Most Water | Medium | Greedy two pointers |
| 17 | Longest Substring Without Repeating Characters | Medium | Variable window + set/map |
| 18 | Longest Repeating Character Replacement | Medium | Sliding window + counts |
| 19 | Permutation in String | Medium | Fixed sliding window |
| 20 | Minimum Window Substring | Hard | Variable window + counts |

### 3. Stack, queue and linked list — 9

| # | Problem | Level | Main pattern |
|---:|---|---|---|
| 21 | Valid Parentheses | Easy | Stack |
| 22 | Min Stack | Medium | Stack design |
| 23 | Evaluate Reverse Polish Notation | Medium | Stack |
| 24 | Daily Temperatures | Medium | Monotonic stack |
| 25 | Reverse Linked List | Easy | Pointer manipulation |
| 26 | Merge Two Sorted Lists | Easy | Linked-list merge |
| 27 | Linked List Cycle | Easy | Fast/slow pointers |
| 28 | Remove Nth Node From End of List | Medium | Two pointers |
| 29 | Reorder List | Medium | Middle + reverse + merge |

### 4. Binary search, sorting and intervals — 8

| # | Problem | Level | Main pattern |
|---:|---|---|---|
| 30 | Binary Search | Easy | Search boundaries |
| 31 | Search in Rotated Sorted Array | Medium | Modified binary search |
| 32 | Find Minimum in Rotated Sorted Array | Medium | Binary search |
| 33 | Time Based Key-Value Store | Medium | HashMap + binary search |
| 34 | Koko Eating Bananas | Medium | Binary search on answer |
| 35 | Merge Intervals | Medium | Sorting + intervals |
| 36 | Insert Interval | Medium | Interval merging |
| 37 | Non-overlapping Intervals | Medium | Greedy interval scheduling |

### 5. Trees and binary search trees — 9

| # | Problem | Level | Main pattern |
|---:|---|---|---|
| 38 | Maximum Depth of Binary Tree | Easy | DFS |
| 39 | Invert Binary Tree | Easy | Recursive tree traversal |
| 40 | Same Tree | Easy | DFS |
| 41 | Binary Tree Level Order Traversal | Medium | BFS |
| 42 | Validate Binary Search Tree | Medium | Bounds / inorder |
| 43 | Kth Smallest Element in a BST | Medium | Inorder traversal |
| 44 | Lowest Common Ancestor of a BST | Medium | BST properties |
| 45 | Binary Tree Right Side View | Medium | BFS / DFS |
| 46 | Construct Binary Tree from Preorder and Inorder Traversal | Medium | Recursion + index map |

### 6. Heap and priority queue — 4

| # | Problem | Level | Main pattern |
|---:|---|---|---|
| 47 | Kth Largest Element in an Array | Medium | Heap / quickselect |
| 48 | Last Stone Weight | Easy | Max heap |
| 49 | K Closest Points to Origin | Medium | PriorityQueue |
| 50 | Find Median from Data Stream | Hard | Two heaps |

### 7. Graphs — 7

| # | Problem | Level | Main pattern |
|---:|---|---|---|
| 51 | Number of Islands | Medium | Grid DFS/BFS |
| 52 | Max Area of Island | Medium | Grid traversal |
| 53 | Clone Graph | Medium | DFS/BFS + HashMap |
| 54 | Rotting Oranges | Medium | Multi-source BFS |
| 55 | Course Schedule | Medium | Topological sort / cycle detection |
| 56 | Pacific Atlantic Water Flow | Medium | Reverse graph traversal |
| 57 | Network Delay Time | Medium | Dijkstra / priority queue |

### 8. Backtracking and recursion — 5

| # | Problem | Level | Main pattern |
|---:|---|---|---|
| 58 | Subsets | Medium | Backtracking |
| 59 | Combination Sum | Medium | Backtracking + pruning |
| 60 | Permutations | Medium | Backtracking |
| 61 | Word Search | Medium | Grid backtracking |
| 62 | Letter Combinations of a Phone Number | Medium | Recursive choice tree |

### 9. Dynamic programming and greedy — 8

| # | Problem | Level | Main pattern |
|---:|---|---|---|
| 63 | Climbing Stairs | Easy | 1D DP |
| 64 | House Robber | Medium | 1D DP |
| 65 | Coin Change | Medium | Unbounded DP |
| 66 | Longest Increasing Subsequence | Medium | DP / binary search |
| 67 | Unique Paths | Medium | Grid DP |
| 68 | Decode Ways | Medium | DP with states |
| 69 | Jump Game | Medium | Greedy |
| 70 | Partition Equal Subset Sum | Medium | 0/1 knapsack |

## Selected stretch problems (after the core set)

Attempt these once the core patterns are comfortable, especially for roles with a stronger algorithmic bar.

| Problem | Level | What it adds |
|---|---|---|
| Trapping Rain Water | Hard | Two pointers / prefix maxima |
| Sliding Window Maximum | Hard | Monotonic deque |
| Largest Rectangle in Histogram | Hard | Monotonic stack |
| Word Ladder | Hard | BFS |
| Alien Dictionary | Hard | Graph + topological sort |
| N-Queens | Hard | Backtracking |
| Regular Expression Matching | Hard | 2D dynamic programming |
| Edit Distance | Medium | 2D dynamic programming |
| Merge k Sorted Lists | Hard | Heap + linked lists |
| Median of Two Sorted Arrays | Hard | Binary search / partitioning |

## 12-week practice sequence

| Week | Focus | Core questions |
|---:|---|---|
| 1 | Arrays, strings, hashing fundamentals | 1–6 |
| 2 | Hashing, prefix sums, two pointers | 7–16 |
| 3 | Sliding window | 17–20; re-solve selected Week 1 problems |
| 4 | Stack, queue and linked lists | 21–29 |
| 5 | Binary search, sorting and intervals | 30–37 |
| 6 | Tree fundamentals and traversal | 38–43 |
| 7 | Advanced tree patterns, heaps | 44–50 |
| 8 | Graph BFS/DFS and grid traversal | 51–54 |
| 9 | Graph algorithms and backtracking | 55–62 |
| 10 | DP foundations and greedy | 63–70 |
| 11 | Mixed timed practice | Revisit weak patterns; attempt 2–3 stretch problems |
| 12 | Interview simulation | Mixed sets, company-tagged questions and mock interviews |

The sequence is a guide, not a strict deadline. If a pattern is not clear, spend more time on it before moving forward.

## Daily 60-minute DSA routine

- **10 minutes:** Recall a previously learned pattern and its complexity.
- **35 minutes:** Solve one new problem (or make a serious attempt at a medium problem).
- **10 minutes:** Review edge cases, complexity and a cleaner solution.
- **5 minutes:** Update the tracker and schedule the next re-solve.

On days when a medium problem takes longer, finish the learning cycle rather than rushing to start another question. Aim for 8–12 quality attempts per week, including re-solves.

## Java-specific expectations

- Be fluent with `HashMap`, `HashSet`, `ArrayList`, `ArrayDeque`, `PriorityQueue`, sorting and custom comparators.
- Know when to use `int` versus `long`; check multiplication, sums and comparator overflow.
- Understand `equals()` / `hashCode()`, immutable map keys and object identity.
- Prefer `ArrayDeque` for stack/queue use cases; understand why legacy `Stack` is generally not preferred.
- Write helper methods with clear contracts and avoid unnecessary abstractions.
- Practise implementing common structures and graph adjacency lists from scratch.

## Progress tracker

Copy this table into your personal tracker or add a status column as you practise.

| Status | Meaning |
|---|---|
| Not started | Have not attempted |
| Attempted | Tried independently, not yet solved |
| Solved with hint | Needed a hint or editorial |
| Solved independently | Solved and explained without help |
| Re-solved | Reimplemented later from a blank editor |

A problem is interview-ready only when you can solve it independently, explain the reasoning and complexity, and handle follow-up variations. Revisit any problem initially solved with a hint.
