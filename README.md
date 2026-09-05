# LeetCode 145 – Binary Tree Postorder Traversal

## Problem

Given the root of a binary tree, return the **postorder traversal** of its nodes' values.

In postorder traversal, nodes are visited in the following order:

```text
Left → Right → Root
```

## Example 1

**Input:**

```text
root = [1,null,2,3]
```

**Output:**

```text
[3,2,1]
```

## Example 2

**Input:**

```text
root = []
```

**Output:**

```text
[]
```

## Example 3

**Input:**

```text
root = [1]
```

**Output:**

```text
[1]
```

## Approach

Postorder traversal can be implemented using **recursion**.

For every node:

1. Traverse the left subtree.
2. Traverse the right subtree.
3. Process the current node.

This produces the required `Left → Right → Root` order.

## Algorithm

1. Create an empty result list.
2. If the current node is `null`, return.
3. Recursively traverse the left child.
4. Recursively traverse the right child.
5. Add the current node's value to the result.
6. Return the result list.

## Example

For the tree:

```text
      1
     / \
    2   3
```

The postorder traversal is:

```text
2 → 3 → 1
```

## Complexity

* **Time Complexity:** `O(n)`
* **Space Complexity:** `O(n)` in the worst case due to recursion.

Here, `n` is the number of nodes in the tree.

## LeetCode Details

* **Problem Number:** 145
* **Problem Name:** Binary Tree Postorder Traversal
* **Difficulty:** Easy
* **Language:** Python 3
* **File:** `solution.py`

## Topics

* Stack
* Tree
* Depth-First Search
* Binary Tree

## Key Learning

This problem helps understand **postorder tree traversal**.

Postorder traversal is commonly useful when child nodes need to be processed before their parent, such as when deleting or evaluating tree structures.

## Repository Structure

```text
leetcode-145-binary-tree-postorder-traversal/
│
├── solution.py
└── README.md
```

## Author

T.Nandhini
