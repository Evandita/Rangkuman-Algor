# Bentuk Rekursif

$$
T(n) = aT(\frac{n}{b}) + f(n)
$$

$$
T(1) = f(1)
$$

$$
a \ge 1, b > 1
$$

# Metode Analisis

## Substitusi

Menebak fungsi tebak menggunakan metode **tebak**. Penebakan dapat dihasilkan melalui analisis iteratif Algoritma.

#### Langkah-langkah:

- Mencari O(g(n))
- Substitusi persamaan berikut:

$$
a(cg(\frac{n}{b})) + f(n) \le cg(n)
$$

- Identifikasi apakah tebakan g(n) berhasil

## Recursion Tree

Mengubah fungsi rekursif menjadi pohon dan diikuti dengan subsitusi.

#### Langkah-langkah:

- Lengkapi informasi pada tabel berikut

Recursive Calls           | # Nodes   | Tree                     | Row Sums
--------------------------|-----------|--------------------------|----------
T(n/b^0) = T(n)           | a^0       | f(n)                     | f(n)
T(n/b^1)                  | a^1       | f(n/b) ... f(n/b)        | a f(n/b)
T(n/b^2)                  | a^2       | f(n/b^2) ... f(n/b^2)    | a^2 f(n/b^2)
...                       | ...       | ...                      | ...
T(n/b^(b log n)) = T(1)   | a^b log n | c ... c                  | a^(b log n) c

- Temukan nilai T(n) menggunakan rumus berikut

$$
T(n) = \sum_{i=1}^{^{b}log(n)}f(\frac{n}{b^i})(a^i) + \theta (f(n))
$$

- Temukan nilai O(g(n)) dengan mengubah sigma menuju tak hingga. Gunakan rumus berikut untuk mendapatkan hasil deret geometri tak hingga.

$$
\sum_{i=1}^{\infty}ar^{n} = \frac{a}{1-r}
$$

- Gunakan metode substitusi untuk membuktikan apakah g(n) yang didapat benar.


## Master Theorem

Menggunakan kasus sebagai berikut:

#### Kasus 1

Syarat:

$$
f(n) < n^{^{b}log(a)}
$$

maka, 

$$
f(n) = O( n^{^{b}log(a)-\epsilon}),\epsilon > 0
$$

$$
T(n) = \theta ( n^{^{b}log(a)})
$$


#### Kasus 2

Syarat:

$$
f(n) = n^{^{b}log(a)}
$$

maka,

$$
T(n) = \theta ( n^{^{b}log(a)} lg(n))
$$

#### Kasus 3

Syarat:

$$
f(n) > n^{^{b}log(a)}
$$

maka,

$$
f(n) = \Omega( n^{^{b}log(a)+\epsilon}),\epsilon > 0
$$

$$
T(n) = \theta(f(n))
$$

Untuk `c < 1` dan `n besar`, dapat dibuktikan

$$
af(\frac{n}{b}) \le cf(n)
$$
