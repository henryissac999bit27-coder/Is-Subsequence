# 392. Is Subsequence

**Difficulty:** Easy | **Topics:** Two Pointers, String | [LeetCode Link](https://leetcode.com)

## Problem Description
Given two strings `s` and `t`, return `true` if `s` is a subsequence of `t`, or `false` otherwise.

A **subsequence** is formed from the original string by deleting some (can be none) characters without disturbing the relative positions of the remaining characters. (e.g., `"ace"` is a subsequence of `"abcde"` while `"aec"` is not).

### Examples
- **Input:** `s = "abc"`, `t = "ahbgdc"`  
  **Output:** `true`
- **Input:** `s = "axc"`, `t = "ahbgdc"`  
  **Output:** `false`

## Solution Explanation
The solution uses the **Two-Pointer Technique**:
1. Initialize pointer `i` for `s` and `j` for `t`.
2. Traverse through string `t`.
3. If `s.charAt(i)` matches `t.charAt(j)`, increment `i`.
4. Always increment `j` to continue checking the next character in `t`.
5. If `i` equals the length of `s`, it means all characters were found in sequence.

### Complexity Analysis
- **Time Complexity:** $O(T)$, where $T$ is the length of the target string `t`. We perform a single scan.
- **Space Complexity:** $O(1)$, since no extra data structures are used.
