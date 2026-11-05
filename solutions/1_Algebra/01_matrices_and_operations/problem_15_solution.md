# Exercise 15. Associativity of Multiplication and Different Calculation Paths

## Question

Given

```math
A =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix},
\qquad
C =
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix},
```

compute (AB)C and A(BC). Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

## Solution

### 1. Computing (AB)C

First compute AB:

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
\end{pmatrix}.
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
\end{pmatrix}.
```

### 2. Computing A(BC)

First compute BC:

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
\end{pmatrix}.
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
\end{pmatrix}.
```

### 3. Comparing the Results

The two calculation paths produce the same matrix:

```math
(AB)C=A(BC)=
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}.
```

### 4. Comparing Operation Counts

Using standard matrix multiplication, an m × n matrix multiplied by an n × p matrix requires mnp scalar multiplications and mp(n − 1) scalar additions.

The following counts include operations involving zero and one, without simplification.

| Calculation | Scalar multiplications | Scalar additions |
|---|---:|---:|
| AB | 12 | 8 |
| (AB)C | 8 | 4 |
| First path total | 20 | 12 |
| BC | 12 | 6 |
| A(BC) | 12 | 8 |
| Second path total | 24 | 14 |

Both paths use two matrix multiplications. However, AB has only four entries, while BC has six. Computing AB first therefore requires fewer scalar operations overall.

### 5. Meaning of Associativity

Associativity means that changing the grouping of a matrix product does not change its value:

```math
(AB)C=A(BC).
```

The order of A, B, and C remains the same; only the pair multiplied first changes. In this example, the final result is identical, but the computational effort differs.
