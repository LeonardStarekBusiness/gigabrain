---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

A binary search tree (BST) is a [[BINARY TREES]] where for every node, all elements in the left subtree are less than or equal to the element at the node, and those in the right subtree are greater than or equal. [[BINARY SEARCH]] can be performed.
Inorder traversal processes elements in sorted order.

![[Pasted image 20260817200331.png]]

The *balance factor* of a node is the *height* of the left node - *height* of the right node. Best case: fully balanced. Worst case: linked list.
Worst case insertion time: $\Theta (n)$ when degraded into linked list.
Best case: $\Theta (\log n)$
Removing: 4 cases. Naive:
1. No children: jus delete vro
2. Only left child: Node becomes left subtree.
3. Only right child: Node becomes right subtree.
4. Both children: Node becomes left subtree, right subtree becomes  right subtree of new node:
![[Pasted image 20260817201253.png]]
Problem: Height may double. Better algorithms exist to keep height the same or reduce by 1.

[[AVL TREES]] are BST that balance themselves with rotations.
[[2-3 TREES]] are also a balanced form of tree with less rotations.