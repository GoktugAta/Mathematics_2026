# Exercise 11. Shortening the Calculation with Row Operations

## Question

Compute:

```math
\det\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6
\end{pmatrix}
```

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

## Solution

Adding a multiple of one row to another does not change the determinant.

First apply:

```math
R_2\leftarrow R_2-R_1,
\qquad
R_3\leftarrow R_3-R_1.
```

Both operations preserve the determinant and give:

```math
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3
\end{pmatrix}.
```

Next apply:

```math
R_3\leftarrow R_3-2R_2.
```

This also preserves the determinant:

```math
U =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix}.
```

We now have an upper triangular matrix, so its determinant is the product of its diagonal entries:

```math
\det(A)=\det(U)=1\cdot1\cdot1=1.
```

All operations used are row replacements, so no sign or scaling correction is needed.
