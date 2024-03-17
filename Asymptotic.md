# Asymptotic Notation

## Big Theta `Θ(n)`

Misalkan f(n) = Θ(g(n)), maka berlaku sifat berikut

$$
c_{1}g(n) \leq f(n) \leq c_{2}g(n)
$$

Dengan, 

$$
c_{1}, c_{2}, n_{0} > 0
$$

$$
n \geq n_{0}
$$

## Big Oh `O(n)`

Misalkan f(n) = O(g(n)), maka berlaku sifat berikut

$$
f(n) \leq cg(n)
$$

Dengan, 

$$
c, n_{0} > 0
$$

$$
n \geq n_{0}
$$

## Big Omega `Ω(n)`

Misalkan f(n) = Ω(g(n)), maka berlaku sifat berikut

$$
cg(n) \leq f(n)
$$

Dengan, 

$$
c, n_{0} > 0
$$

$$
n \geq n_{0}
$$

## Small Oh `o(n)`

Misalkan f(n) = o(g(n)), maka berlaku sifat berikut

$$
\displaystyle \lim_{n \to \infty} \frac{f(n)}{g(n)}=0
$$

## Small Omega `ω(n)`

Misalkan f(n) = ω(g(n)), maka berlaku sifat berikut

$$
\displaystyle \lim_{n \to \infty} \frac{f(n)}{g(n)}= \infty
$$

## Property

### Transivity

$$
f(n) = Θ(g(n)) \wedge  g(n) = Θ(h(n)) \Rightarrow f(n) = Θ(h(n))
$$
$$
f(n) = O(g(n)) \wedge  g(n) = O(h(n)) \Rightarrow f(n) = O(h(n))
$$
$$
f(n) = Ω(g(n)) \wedge  g(n) = Ω(h(n)) \Rightarrow f(n) = Ω(h(n))
$$
$$
f(n) = o(g(n)) \wedge  g(n) = o(h(n)) \Rightarrow f(n) = o(h(n))
$$
$$
f(n) = ω(g(n)) \wedge  g(n) = ω(h(n)) \Rightarrow f(n) = ω(h(n))
$$

### Reflexivity

$$
f(n) = Θ(f(n))
$$
$$
f(n) = O(f(n))
$$
$$
f(n) = Ω(f(n))
$$

### Symmetry

$$
f(n) = Θ(g(n)) \Leftrightarrow g(n) = Θ(f(n))
$$

### Complementarity

$$
f(n) = O(g(n)) \Leftrightarrow g(n) = Ω(f(n))
$$
$$
f(n) = o(g(n)) \Leftrightarrow g(n) = ω(f(n))
$$

## Monotonicity

### Monotonically Increasing

$$
f(n) \leq f(n+1)
$$

### Monotonically Decreasing

$$
f(n) \geq f(n+1)
$$

### Strictly Increasing

$$
f(n) < f(n+1)
$$

### Strictly Decreasing

$$
f(n) > f(n+1)
$$

## Others

$$
\displaystyle \lim_{n \to \infty} \frac{n^{b}}{a^{n}}=0 \Rightarrow n^{b} = o(a^{n})
$$

$$
\displaystyle \lim_{n \to \infty} \frac{lg^{a}n}{n^{b}}=0 \Rightarrow   lg^{a}n= o(n^{b})\wedge n^{b}=  ω(lg^{a}n)
$$

$$
lg(n!) = Θ(n lg n)
$$