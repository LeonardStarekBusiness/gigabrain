---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

Purpose: Multiple children -> smaller height $h$ -> fewer disk operations.

Properties:
1. A node can have $n$ keys.
2. All leaves are at the same level.
3. Internal nodes have $n + 1$ children.
4. Ordered: Left subtree $<$ leftmost key etc... ja eh logisch.

![[Pasted image 20260822194203.png]]

B-Trees have the parameter $t$. (=branching factor)
1. Every internal node has at least $t$ children, at most $2t$.
2. Every node has at least $t - 1$ keys, at most $2t - 1$ keys (since keys = children - 1).
(Special case: [[2-3 TREES]], no fixed $t$)

$$Height <= \frac{log_t (n + 1)}{2}$$
=> Operations are $O (\log_t n)$