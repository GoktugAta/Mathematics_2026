# Problem 11 Solution

### 1. Creating Zeros with Row Operations

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6
\end{pmatrix}
```

Apply the following operations:

```math
R_2 \leftarrow R_2-R_1,
\qquad
R_3 \leftarrow R_3-R_1.
```

Each operation preserves the determinant because it adds a multiple of another row to the row being changed.

The resulting matrix is:

```math
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3
\end{pmatrix}
```

Next, apply:

```math
R_3 \leftarrow R_3-2R_2.
```

This also preserves the determinant and gives:

```math
U =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix}
```

### 2. Computing the Determinant

The determinant of an upper triangular matrix is the product of its diagonal entries:

```math
\det(A)=\det(U)=1\cdot1\cdot1=\boxed{1}.
```

All operations used are row replacements, so no sign or scaling correction is required.
