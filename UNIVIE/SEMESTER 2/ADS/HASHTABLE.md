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


## EXAM QUESTION

Number of valid permutations of operations without failed accesses.
1. Form Groups of operations that hash to the same key.
2. For each Group:
	1. [[BINOMIAL COEFFICIENT]] $$\prod_{\text{of each group}}\pmatrix{\text{n of operations left to handle} \\ \text{n of operations in the group}} \times \text{possible swaps in that group} $$

### Exam question example
insert(1), insert(2), insert(11), delete(1), delete(2), delete(11)

$$ \text{Group 1}\left\{ \begin{array}{l} insert(1), delete(1) \\ insert(11), delete(11) \end{array} \right.$$ 
$$\text{  6 operations left, 4 in group, 2 can be swapped.} $$
$$  $$
$$ \text{Group 2}\left\{ \begin{array}{l} insert(2), delete(2) \end{array} \right. 
$$
$$\\ \text{  2 operations left, 2 in group, none can be swapped (1).} $$

$$ 2\pmatrix{6 \\ 4} * \pmatrix{2 \\ 2} = \boxed{30}$$