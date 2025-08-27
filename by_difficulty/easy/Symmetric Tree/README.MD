# Symmetric Tree

## Problem Statement
Given the `root` of a binary tree, check whether it is a mirror of itself (i.e., symmetric around its center).

### Example 1:

1
/
2 2
/ \ /
3 4 4 3

**Input:** root = [1,2,2,3,4,4,3]  
**Output:** true  

### Example 2:

1
/
2 2
\
3 3


**Input:** root = [1,2,2,null,3,null,3]  
**Output:** false  


## Constraints
- The number of nodes in the tree is in the range `[1, 1000]`.
- `-100 <= Node.val <= 100`


## Approach
To determine if a tree is symmetric:
1. Check if the left and right subtrees are mirrors of each other.
2. For two trees to be mirrors:
   - Their root values must be equal.
   - The left subtree of one must be a mirror of the right subtree of the other, and vice versa.


## Time and Space Complexity
- **Time Complexity:** `O(n)` where `n` is the number of nodes (since each node is visited once).
- **Space Complexity:** `O(h)` where `h` is the height of the tree (recursion stack space). In the worst case, `O(n)` for a skewed tree.


## Related Topics
- Binary Tree
- Depth-First Search (DFS)
- Breadth-First Search (BFS)