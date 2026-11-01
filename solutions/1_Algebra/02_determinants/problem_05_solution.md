# Problem 5 Solution

### 1. Original Matrix

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
```

We simplify A using row replacement operations. Adding a multiple of one row to another does not change the determinant.

### 2. Eliminate the First Entry of Row 2

Apply:

```math
R_2 \leftarrow R_2 - 2R_1
```

The determinant remains unchanged:

```math
A_1 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix},
\qquad
\det(A_1)=\det(A).
```

### 3. Eliminate the First Entry of Row 3

Apply:

```math
R_3 \leftarrow R_3 + R_1
```

The determinant remains unchanged:

```math
A_2 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix},
\qquad
\det(A_2)=\det(A).
```

### 4. Eliminate the Second Entry of Row 3

Apply:

```math
R_3 \leftarrow R_3 + 2R_2
```

The determinant remains unchanged:

```math
U =
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7
\end{pmatrix},
\qquad
\det(U)=\det(A).
```

### 5. Compute the Determinant

U is upper triangular, so its determinant is the product of its diagonal entries:

```math
\det(A)=\det(U)=1\cdot(-3)\cdot(-7)=21.
```

All three row operations preserve the determinant, so no sign or scaling correction is needed.
