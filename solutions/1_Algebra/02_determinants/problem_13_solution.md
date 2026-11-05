# Exercise 13. Determinant by Elimination

## Question

Compute the determinant of

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}
```

using elimination. Record the effect of every row operation used on the value of the determinant.

## Solution

### 1. First Operation

Apply:

```math
R_2\leftarrow R_2-2R_1.
```

This adds a multiple of another row, so the determinant is unchanged:

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

### 2. Second Operation

Apply:

```math
R_3\leftarrow R_3-R_1.
```

The determinant is unchanged:

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

### 3. Third Operation

Apply:

```math
R_3\leftarrow R_3+2R_2.
```

The determinant is unchanged:

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

### 4. Computing the Determinant

The resulting matrix is upper triangular:

```math
\det(A)=\det(U)=1\cdot1\cdot1=1.
```

Every operation preserves the determinant, so no correction is required.
