# Invert-Binary-Tree

The problem is to invert a given binary tree. Inverting a binary tree means swapping the left and right children of all nodes in the tree.

Example:
Input:

        1
       / \
      2   3
     / \
    4   5
Output:

        1
       / \
      3   2
         / \
        5   4


We can solve this problem using Depth-First Search (DFS) and recursion. The approach is as follows:
Base case: If the tree is empty (root is None), return None.
Recursive case: For each node:
Invert the left and right subtrees recursively.
Swap the left and right children of the current node.
Return: Return the root of the modified tree after all swaps.


Time and Space Complexity
Time Complexity: O(n) where n is the number of nodes in the tree. We visit each node exactly once.
Space Complexity: O(h) where h is the height of the tree (due to recursion stack space). In the worst case, the tree is unbalanced, and the space complexity is O(n).
