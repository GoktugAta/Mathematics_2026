# Exercise 5. Row Operations

## Question

For

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix},
```

find det(A) by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

## Solution

### 1. First Row Operation

Apply:

```math
R_2\leftarrow R_2-2R_1.
```

Adding a multiple of another row preserves the determinant:

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

### 2. Second Row Operation

Apply:

```math
R_3\leftarrow R_3+R_1.
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

### 3. Third Row Operation

Apply:

```math
R_3\leftarrow R_3+2R_2.
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

### 4. Computing the Determinant

The resulting matrix is upper triangular, so:

```math
\det(A)=\det(U)=1\cdot(-3)\cdot(-7)=21.
```

All operations preserve the determinant, so no correction is required.
