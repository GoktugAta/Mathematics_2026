# Exercise 10. Detecting Dependence

## Question

Without carrying out a full determinant calculation, explain why:

```math
\det\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5
\end{pmatrix}=0.
```

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

## Solution

The second row is twice the first:

```math
R_2=2R_1.
```

Thus, the rows are linearly dependent. A square matrix with linearly dependent rows has determinant zero.

This can also be seen by performing:

```math
R_2\leftarrow R_2-2R_1.
```

This operation preserves the determinant and gives:

```math
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 5
\end{pmatrix}.
```

A matrix with a zero row has determinant zero. Therefore:

```math
\det(A)=0.
```

Since a square matrix is invertible if and only if its determinant is nonzero, A is not invertible.
