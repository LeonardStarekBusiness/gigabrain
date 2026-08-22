---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

## [[COMPLEXITY]]: 
Worst case with bad pivot: $O (n^2)$
Best case: $O(n \log n)$


## Algorithm: 
This is a [[DIVIDE & CONQUER]] algorithm.
1. Choose a Pivot: Select an element from the array as the pivot. The choice of pivot can vary (e.g., first element, last element, random element, or median) but affects performance. Ideally: middle element.
2. Partition the Array: Re arrange the array around the pivot. After partitioning, all elements smaller than the pivot will be on its left, and all elements greater than the pivot will be on its right.
3. Recursively Call: Recursively apply the same process to the two partitioned sub-arrays.
4. Base Case: The recursion stops when there is only one element left in the sub-array, as a single element is already sorted.
![[Pasted image 20260817143641.png]]

## Implementation:
![[Pasted image 20260817143930.png]]