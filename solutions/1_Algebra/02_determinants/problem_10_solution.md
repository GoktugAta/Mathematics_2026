# Problem 10 Solution

### 1. Identifying Row Dependence

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5
\end{pmatrix}
```

The second row is twice the first row:

```math
R_2=2R_1.
```

Equivalently:

```math
R_2-2R_1=0.
```

Therefore, the rows are linearly dependent.

### 2. Consequence for the Determinant

A matrix with linearly dependent rows has determinant zero. Hence, without a full determinant calculation:

```math
\boxed{\det(A)=0}.
```

This can also be seen by applying the determinant-preserving operation:

```math
R_2 \leftarrow R_2-2R_1.
```

It produces a zero row:

```math
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 5
\end{pmatrix}
```

A matrix with a zero row has determinant zero.

### 3. Noninvertibility

A square matrix is invertible if and only if its determinant is nonzero. Since det(A) = 0, A is not invertible.
