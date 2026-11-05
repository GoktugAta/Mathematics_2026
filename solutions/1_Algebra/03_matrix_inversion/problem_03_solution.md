# Exercise 3. When Does the Inverse Not Exist?

## Question

For

```math
A =
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix},
```

explain in two ways why A⁻¹ does not exist: using the determinant and using dependence between the rows.

## Solution

### Explanation Using the Determinant

```math
\det(A)=2\cdot2-4\cdot1=0.
```

A square matrix is invertible if and only if its determinant is nonzero. Since the determinant is zero, A has no inverse.

### Explanation Using Row Dependence

The first row is twice the second:

```math
R_1=2R_2.
```

Therefore, the rows are linearly dependent. Applying the row operation

```math
R_1 \leftarrow R_1-2R_2
```

gives:

```math
\begin{pmatrix}
0 & 0 \\
1 & 2
\end{pmatrix}.
```

The matrix has only one independent row and cannot be reduced to the 2 × 2 identity matrix. Thus, A is not invertible.
