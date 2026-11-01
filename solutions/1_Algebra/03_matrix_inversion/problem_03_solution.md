# Problem 3 Solution

```math
A =
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}.
```

### 1. Explanation Using the Determinant

```math
\det(A)=2\cdot2-4\cdot1=4-4=0.
```

A square matrix is invertible if and only if its determinant is nonzero. Therefore, A has no inverse.

### 2. Explanation Using Row Dependence

The first row is twice the second row:

```math
R_1=2R_2.
```

Thus, the rows are linearly dependent. Applying:

```math
R_1 \leftarrow R_1-2R_2
```

produces a zero row:

```math
\begin{pmatrix}
0 & 0 \\
1 & 2
\end{pmatrix}.
```

The matrix has rank 1 and cannot be reduced to the 2 × 2 identity matrix. Hence, A is not invertible.
