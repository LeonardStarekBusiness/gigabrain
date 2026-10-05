Choosing $k$ elements from a set of size $n$.

$$ \pmatrix{n \\ k} = \frac{n * (n-1) * (n-2) \text{ ... (k times)}}{k!}$$

Super formally:

$$ \frac{\prod_{i=0}^{k-1}(n-i)}{k!} $$

Example: Choosing $n = 3$ elements from a set of size $k = 5$.
$$ \pmatrix{5 \\ 3} = \frac{5 * 4 * 3}{3!} = \boxed{10} $$