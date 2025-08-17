Climbing Stairs  

**Difficulty:** Easy  
**Problem Link:** [LeetCode - Climbing Stairs](https://leetcode.com/problems/climbing-stairs/)  

---

## Problem Description  
You are climbing a staircase. It takes `n` steps to reach the top.  
Each time you can either climb **1 step** or **2 steps**.  
Determine the number of distinct ways to reach the top.  

---

## Examples  

**Example 1**  
Input: n = 2
Output: 2
Explanation:

1 step + 1 step

2 steps

markdown
Copy code

**Example 2**  
Input: n = 3
Output: 3
Explanation:

1 step + 1 step + 1 step

1 step + 2 steps

2 steps + 1 step

yaml
Copy code

---

## Approach  
This problem can be solved using **Dynamic Programming**.  

- To reach step `n`, there are two possible previous steps:  
  - From step `n-1` (taking 1 step)  
  - From step `n-2` (taking 2 steps)  

This leads to the recurrence relation:  

ways(n) = ways(n-1) + ways(n-2)

yaml
Copy code

This relation is equivalent to the **Fibonacci sequence**.  
By using two variables to track the last two states, we can achieve an optimized solution.  

---

## Complexity Analysis  
- **Time Complexity:** O(n) – a single pass is made through the steps.  
- **Space Complexity:** O(1) – only two variables are used for computation.  

---

## File  
- Solution implementation: [`climbing_stairs.py`](./climbing_stairs.py)  