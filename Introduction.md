# Pengantar Analisis Algoritma

## Definisi Algoritma

### Levitin

Urutan instruksi untuk menyelesaikan masalah

### Cormen

Urutan instruksi untuk mengubah input menjadi output

## Algoritma GCD

### Euclid

```
gcd(m,n) = gcd(n, m mod n)
```

### Censecutive Integer

Mencari nilai terbesar mendekati min(m,n) yang mampu membagi habis m dan n. Pencarian nilai dilakukan dengan men-decrement min(m,n) secara bertahap

### Middle-School Procedure

Mencari seluruh faktor prima yang sama antara m dan n, lalu kalikan seluruh faktor prima tersebut.

## Analisis Algoritma

Sebuah algoritma dikatakan **benar**, jika mampu memberikan output yang sesuai untuk setiap kombinasi input. Seberapa baiknya algoritma bergantung pada:

1. Kebenaran
2. Kecepatan
3. Penggunaan Memori

## Efisiensi Algoritma

Waktu yang dibutuhkan untuk mengeksekusi sebuah algoritma dapat menggunakan rumus:

$$
T = \frac{T(n)}{MIPS}
$$

## Algoritma Umum

1. Sorting

> Stability: Letak relatif antara 2 elemen tetap terjaga

> In Place: Tidak memakan memori tambahan

2. Searching
3. String
4. Graph
5. Combinatorial
6. Graph
7. Numerical

## Struktur Data Umum

1. List

> Array bersifat static dan direct access, sedangkan List bersifat dynamic dan traversal access

2. Stack

> Bersifat LIFO, dan hanya terdiri dari operasi push dan pop

3. Queue

> Bersifat FIFO, dan hanya terdiri dari operasi enqueue dan dequeue

4. Priority Queue

> Diurutkan berdasarkan prioritas

5. Graph

> Dilambangkan G = <V,E>

> Dapat direpresentasikan menggunakan adjacency matrix atau adjacency linked list

> Berdasarkan bobot edge, dapat diklasifikan menjadi weighted graph dan unweighted graph

> Berdasarkan looping, dapat diklasifikan menjadi Cyclic Graph dan Acyclic Graph

> Berdasarkan arah, dapat diklasifikan menjadi directed dan undirected Graph.

6. Tree

> Berupa Acyclic Graph

> Node paling atas disebut Root, sedangkan node paling bawah disebut Leaf

> Ancestor adalah seluruh Node yang berada di atasnya, sedangkan Descendants merupakan seluruh Node yang berada di bawahnya

> Parent merupakan Ancesotor terdekat, sedangkan Child merupakan Descendant terdekat.

> Node dengan Parent yang sama disebut Sibling

> Tinggi sebuah Node diukur dari Node tersebut sampai Root.

> Tinggi sebuah Tree diukur dari Leaf terdalam sampai Root.

7. Set and Dictionary

> Set adalah kumpulan elemen yang unik dan tidak terurut

> List adalah kumpulan elemen yang tidak unik dan terurut

> Bag adalah kumpulan elemen yang tidak unik dan tidak terurut

> Dictionary mengimplementasikan seaching, add, dan delete