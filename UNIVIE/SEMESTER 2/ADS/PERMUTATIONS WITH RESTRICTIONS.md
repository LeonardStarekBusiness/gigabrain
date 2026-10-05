## Items need to stay together

1. Form Groups.
Number of Groups = $N$
Number of possible permutations in each group = $P_i$
Number of elements that can be swapped, such as same letters in a word: $S_i$
$$ \frac{N! * P_1 * P_2 ... P_i}{S_1! * S_2! ... * S_i!}$$
### Example "HELLO" but E and O are together
$N$= 4, $P_i$ = 2, $S_L$ = 2
$$ \frac{4! * 2!}{2!} = \boxed{24}$$
![[Pasted image 20260901203731.png]]


## Items shall not be together

1. Form Groups.
Number of free items = $F$
Number of items that should be apart: $D$
Number of elements that can be swapped, such as same letters in a word: $SF_i$
$$ \frac{F!}{SF_1! * SF_2! ... SF_i!} * \pmatrix{{F + 1} \\ {D}} \text{  <-- binomial}$$
See [[BINOMIAL COEFFICIENT]].
### Example "SUCCESS" but the S shall not be together
$F$ = 4,  $D$ = 3,
$SF_C$ = 2, 

$$ \frac{4!}{2!} * \frac{5*4*3}{3!} = \boxed{120}$$
![[Pasted image 20260901213654.png]]