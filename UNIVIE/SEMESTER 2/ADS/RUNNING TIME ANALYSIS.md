---
name: Algorithmen und Datenstrukturen
semester: 2026S
bereich: univie
kürzel: ADS
---

## Step-by-Step

1. Is the runtime a mathematical function of n?
    1. YES: $T(n)$ angeben.
2.  NO:
    1. Worst Case Input & dessen Time Complexity: $T_W(n)$ angeben.
    2. Best Case Input & dessen Time Complexity: $T_B(n)$ angeben.

If not a  dependent nested loop: easy.
It it is:
1. Build sum of times the instruction is called, inner with respect to outer.
2. Deduce the complexity of the algorithm with the identities.
![[Pasted image 20260901193526.png]]

### Test Example: 

Nested Loops
1. Independent Nested Loops: Frequency count einfach multiplizieren.
2. Dependent Nested Loops: Evaluate the inner loop for each iteration of the outer loop (Summe aufstellen)

Harmonic Sum (sehr wichtig!!).
![[Pasted image 20260826025036.png]]

## Test Example
![[Pasted image 20260830135807.png]]

![[Pasted image 20260830140419.png]]