---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

2-3 Trees are a special case of [[B-TREES]].

![[Pasted image 20260819155006.png]]

```cpp
class Node23
{
	Node23 *ptr0; int key0;
	Node23 *ptr1; int key1;
	Node23 *ptr2;
}
```

A 2-3 Tree is always balanced.
IMPORTANT: A leaf node has no children and 1 or 2 keys.
An internal node with 1 key has 2 children.
An internal node with 2 keys has 3 children.

A 2-3 Tree can split, redistribute, or merge to remain balance.
Insertion: splitting:
``` nothingburger
        [20]
       /    \
    [10]   [30 | 40 | 50]   ← overflow

Split the overflowing node and put the middle element in the parent.

	  [20 | 40]
	 /    |    \
  [10]  [30]  [50]

If the parent overflows, split the parent.
If the root overflows, create a new root.
```

Deletion: 
``` nothingburger
Case 1: simply delete.
Case 2: Delete and merge (split parent and descend)
Case 3: Borrow from neightbor and parent.
```

A node with only one key is said to be half full with ptr2 being nullptr and key1 ignored,
and that with two keys is full. It then behaves like a [[BINARY SEARCH TREES]].