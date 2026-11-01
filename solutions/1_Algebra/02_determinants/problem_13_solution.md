# Problem 13 Solution

### 1. Original Matrix

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}
```

### 2. Eliminate the First Entry of Row 2

Apply:

```math
R_2 \leftarrow R_2-2R_1.
```

Adding a multiple of another row does not change the determinant:

```math
A_1 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2
\end{pmatrix},
\qquad
\det(A_1)=\det(A).
```

### 3. Eliminate the First Entry of Row 3

Apply:

```math
R_3 \leftarrow R_3-R_1.
```

The determinant remains unchanged:

```math
A_2 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1
\end{pmatrix},
\qquad
\det(A_2)=\det(A).
```

### 4. Eliminate the Second Entry of Row 3

Apply:

```math
R_3 \leftarrow R_3+2R_2.
```

The determinant remains unchanged:

```math
U =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix},
\qquad
\det(U)=\det(A).
```

### 5. Computing the Determinant

Since U is upper triangular:

```math
\det(A)=\det(U)=1\cdot1\cdot1=\boxed{1}.
```

Every row operation used preserves the determinant, so no correction is needed.
