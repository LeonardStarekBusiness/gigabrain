---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

## Complexity
$O (E + |V| \log |V|)$

## Algorithm

1. Create a list $Visited = \{\}$
2. Starting node A: Keep track of distance from A and previous node.
Put 0 for A and $\infty$ for all others.
![[Pasted image 20260830160528.png]]
3. Visit every edge from (current node) and update table.
4. Set node to finished.
5. Choose closest, unvisited node & Repeat from step 3.