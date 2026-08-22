---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

## [[COMPLEXITY]]: 
$O(n \log n)$


## Algorithm: 
This is a [[DIVIDE & CONQUER]] algorithm.
1. *Divide* the unsorted array into two sub-arrays, half the size of the original.
2. Continue to divide the sub-arrays as long as the current piece of the array has more than one element.
3. *Conquer* : Merge two sub-arrays together by always putting the lowest value first.
4. Keep merging until there are no sub-arrays left.

![[Pasted image 20260816213438.png]]

## Implementation:

![[Pasted image 20260817142033.png]]
Merge() implementation. Merge the sub-arrays back using a temporary array.
![[Pasted image 20260817142529.png]]