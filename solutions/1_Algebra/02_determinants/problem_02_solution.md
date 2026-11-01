# Problem 2 Solution

### 1. Computing the Determinant Using Sarrus' Rule

```math
A =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5
\end{pmatrix}
```

The sum of the downward diagonal products is:

```math
1 \cdot 3 \cdot 5
+ 2 \cdot 4 \cdot 2
+ (-1) \cdot 0 \cdot 1
= 15+16+0
= 31.
```

The sum of the upward diagonal products is:

```math
(-1) \cdot 3 \cdot 2
+ 2 \cdot 0 \cdot 5
+ 1 \cdot 4 \cdot 1
= -6+0+4
= -2.
```

Therefore:

```math
\det(A) = 31-(-2) = 33.
```

### 2. Check Using Row Operations

Adding a multiple of one row to another does not change the determinant.

Apply:

```math
R_3 \leftarrow R_3-2R_1
```

This gives:

```math
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7
\end{pmatrix}
```

Next, apply:

```math
R_3 \leftarrow R_3+R_2
```

This gives the upper triangular matrix:

```math
U =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & 0 & 11
\end{pmatrix}
```

The determinant of a triangular matrix is the product of its diagonal entries. Since both row operations preserve the determinant:

```math
\det(A) = \det(U) = 1 \cdot 3 \cdot 11 = 33.
```

This confirms the result obtained using Sarrus' rule.
