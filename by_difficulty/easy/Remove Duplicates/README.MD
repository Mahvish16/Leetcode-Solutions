# LeetCode - 83. Remove Duplicates from Sorted List

## Problem Description
Given the **head** of a sorted linked list, delete all duplicates such that each element appears only once. Return the linked list **sorted** as well.

---

### Example 1:
**Input:**  
`head = [1,1,2]`  

**Output:**  
`[1,2]`

---

### Example 2:
**Input:**  
`head = [1,1,2,3,3]`  

**Output:**  
`[1,2,3]`

---

## Constraints
- The number of nodes in the list is in the range `[0, 300]`.
- `-100 <= Node.val <= 100`
- The list is guaranteed to be **sorted** in ascending order.

---

## Approach
1. **Observation**: Since the linked list is sorted, any duplicates will appear **next to each other**.
2. **Traversal**: Start with the head node and iterate through the list.
3. **Duplicate Check**:  
   - Compare the current node with the next node.  
   - If both have the same value, skip the next node by adjusting the `next` pointer.  
   - Otherwise, move to the next node.
4. **Continue** this process until the end of the list is reached.
5. **Return** the modified head of the linked list.

This ensures that all duplicates are removed while maintaining the sorted order.

---

## Complexity Analysis
- **Time Complexity:** `O(n)`  
  - Each node is visited at most once, where `n` is the number of nodes in the linked list.
- **Space Complexity:** `O(1)`  
  - No extra data structures are used; modifications are done in-place.

---

## Topics
- Linked List  
- Two Pointers  

---

## Companies
This is a frequently asked interview problem at various top tech companies.

---

## How to Run
1. Open the problem on [LeetCode - Remove Duplicates from Sorted List](https://leetcode.com/problems/remove-duplicates-from-sorted-list/).  
2. Implement your solution in the editor.  
3. Test using the given cases and additional custom cases.
