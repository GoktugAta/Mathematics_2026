# Problem 15 Solution

### 1. Computing (AB)C

First, compute AB:

```math
AB =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
=
\begin{pmatrix}
1+4+0 & 0+2+0 \\
0+2-1 & 0+1+3
\end{pmatrix}
=
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
```

Then multiply by C:

```math
(AB)C =
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
=
\begin{pmatrix}
10+0 & 5-2 \\
2+0 & 1-4
\end{pmatrix}
=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
```

### 2. Computing A(BC)

First, compute BC:

```math
BC =
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
=
\begin{pmatrix}
2+0 & 1+0 \\
4+0 & 2-1 \\
-2+0 & -1-3
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
```

Then multiply by A on the left:

```math
A(BC) =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
=
\begin{pmatrix}
2+8+0 & 1+2+0 \\
0+4-2 & 0+1-4
\end{pmatrix}
=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
```

### 3. Comparing the Results

Both calculation paths give the same matrix:

```math
(AB)C = A(BC) =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
```

### 4. Comparing the Number of Operations

Using standard matrix multiplication, multiplying an m × n matrix by an n × p matrix requires mnp scalar multiplications and mp(n − 1) scalar additions.

These counts include operations involving zero or one, without simplification.

| Calculation | Scalar multiplications | Scalar additions |
|---|---:|---:|
| AB | 12 | 8 |
| (AB)C | 8 | 4 |
| First path total | 20 | 12 |
| BC | 12 | 6 |
| A(BC) | 12 | 8 |
| Second path total | 24 | 14 |

Both paths use two matrix multiplications, but the first path requires fewer scalar operations because AB is a 2 × 2 matrix, while BC is a 3 × 2 matrix.

### 5. Meaning of Associativity

Associativity means that changing the grouping of a matrix product does not change the result, provided the products are defined:

```math
(AB)C = A(BC).
```

The order of A, B, and C remains unchanged. Only the choice of which pair to multiply first changes.

In this example, both groupings produce the same matrix, but computing AB first requires fewer scalar operations.
