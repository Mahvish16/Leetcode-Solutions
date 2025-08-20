Binary Tree Inorder Traversal

## Problem Statement
Given the root of a binary tree, return the inorder traversal of its nodes' values.

- **LeetCode Problem:** [94. Binary Tree Inorder Traversal](https://leetcode.com/problems/binary-tree-inorder-traversal/)  
- **Difficulty:** Easy  
- **Topics:** Tree, Depth-First Search, Binary Tree  

## Example 1
**Input:**
root = [1,null,2,3]

**Output:**
[1,3,2]

**Explanation:**  
The binary tree structure is:

1
 \
  2
 /
3

Inorder traversal visits: left → root → right  
So the result is: **[1,3,2]**

## Example 2
**Input:**
root = []

**Output:**
[]

## Example 3
**Input:**
root = [1]

**Output:**
[1]

## Constraints
- The number of nodes in the tree is in the range `[0, 100]`.
- `-100 <= Node.val <= 100`


## Approach

### 1. Recursive Inorder Traversal
- Traverse the left subtree.
- Visit the root node.
- Traverse the right subtree.
- Collect values in a list and return.

### 2. Iterative Inorder Traversal (Using Stack)
- Use an explicit stack to simulate recursion.
- Traverse down the left subtree pushing nodes onto the stack.
- Pop from the stack when there are no more left nodes.
- Visit the node, then move to the right subtree.
- Continue until both stack is empty and all nodes are processed.


## Time & Space Complexity

### Recursive Approach
- **Time Complexity:** `O(n)` (visits each node once)
- **Space Complexity:** `O(n)` (recursion stack in worst case)

### Iterative Approach
- **Time Complexity:** `O(n)`
- **Space Complexity:** `O(n)` (explicit stack)