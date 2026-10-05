---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

Heaps are almost complete  [[BINARY TREES]].
When written out as an array (levelorder): 
- Index of left child is $2 * i + 1$
- Index of right $2 * i + 2$

Max heap: every node is >= its children.
Min heap: every node is <= its children.

Max-heapify: If a node is smaller than one of its children, swap it with its larger child and recursively continue down the tree.
![[Pasted image 20260817193731.png]]

Inserting into a max heap: Insert at the end and "bubble up" if the max heap property is violated.

Heaps can be used to implement priority queues (extract_min() & extract_max() using min heap / max heap).