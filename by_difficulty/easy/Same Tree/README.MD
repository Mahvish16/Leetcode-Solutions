Same Tree

## Problem Description
Given the roots of two binary trees `p` and `q`, write a function to check if they are the same or not.  

Two binary trees are considered the same if they are:
1. Structurally identical.
2. The nodes have the same value.


## Examples

### Example 1:
**Input:**
p = [1,2,3]
q = [1,2,3]

**Output:**
true

### Example 2:
**Input:**
p = [1,2]
q = [1,null,2]

**Output:**
false

### Example 3:
**Input:**
p = [1,2,1]
q = [1,1,2]

**Output:**
false

## Constraints
- The number of nodes in both trees is in the range `[0, 100]`.
- `-10^4 <= Node.val <= 10^4`

## Approach
- Use recursion or iterative traversal to compare both trees.
- At each node:
  - If both nodes are `None`, they are the same at this branch.
  - If one is `None` and the other is not, they differ.
  - If values differ, return `false`.
  - Recursively check left and right subtrees.

## Complexity Analysis
- **Time Complexity:** `O(n)` where `n` is the number of nodes in the tree (each node is visited once).
- **Space Complexity:** `O(h)` where `h` is the height of the tree (recursion stack).