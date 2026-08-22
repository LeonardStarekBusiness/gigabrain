---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

Hash function: map a key to an index in the hash table.
Solutions fo collisions:
1. Chaining: Every element in the hash table is a linked list. <br>  Best case: $\Theta (1)$ no collisions. <br> Worst case: $\Theta (n)$ if everything maps to the same index. Degradation to a linked list.
 ![[Pasted image 20260817185114.png]]
2. Probing: Pick another empty slot. $i$ = number of probing attempts.
	1. Linear Probing: Pick the next slot.
	$$ h_i(k) = (h(k) + i) $$
	2. Quadratic Probing: Move by squares to avoid clustering. =offset by 1, 4, 9, 16 ...
	$$ h_i(k) = (h(k) + i^2) $$
	3. Double Hashing: First hash determines starting position. Second hash determines offset size.
	$$ h_i(k) = (h_1(k) + i \cdot h_2(k))$$