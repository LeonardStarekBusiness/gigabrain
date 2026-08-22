---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

Exist singly and doubly linked list.

```cpp
class LinkedListNode {
	int data;
	LinkedListNode *next;
}
```

``` cpp
class DoublyLinkedListNode {
	int data;
	DoublyLinkedListNode *prev;
	DoublyLinkedListNode *next;
}
```
You can implement a [[STACK]] using a [[DYNAMIC ARRAY]] and a linked list.
You can implement a [[QUEUE & DEQUE]] with a doubly linked list.