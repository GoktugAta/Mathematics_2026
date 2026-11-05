# Exercise 6. Transpose

## Question

For

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix},
```

compute Aᵀ, Bᵀ, and AB. Then verify in this example that:

```math
(AB)^T=B^TA^T.
```

## Solution

### 1. Computing the Transposes

Transposing interchanges rows and columns:

```math
A^T =
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix},
\qquad
B^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}.
```

### 2. Computing AB

Multiply each row of A by each column of B:

```math
AB =
\begin{pmatrix}
1+4-3 & 0+2+9 \\
4+10-6 & 0+5+18
\end{pmatrix}
=
\begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}.
```

Therefore:

```math
(AB)^T =
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}.
```

### 3. Computing BᵀAᵀ

```math
B^TA^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
=
\begin{pmatrix}
1+4-3 & 4+10-6 \\
0+2+9 & 0+5+18
\end{pmatrix}
=
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}.
```

Both calculations produce the same matrix, confirming:

```math
(AB)^T=B^TA^T.
```
