---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

Give the nodes in an order that respects dependency.
Applicable on a Directed Acyclic [[GRAPHS]].

![[Pasted image 20260823141402.png]]

Different algorithms. Meistens intuitiv tbh. Aber:
### Kahn's algorithm (Joshua KHAN AALAMPOUR)
 Repeat until no nodes left:
1. Find all nodes with indegree 0 and put them in a queue.
2. Take a node from the queue and add it to the ordering.
3. Remove its outgoing edges (indegree of that node -= 1)
4. If any neighbor's indegree becomes 0, put it in the queue.