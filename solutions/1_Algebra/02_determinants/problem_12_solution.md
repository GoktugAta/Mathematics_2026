# Problem 12 Solution

### 1. Performing the Required Row Operation

```math
A(t) =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1
\end{pmatrix}
```

Apply:

```math
R_2 \leftarrow R_2-2R_1.
```

This operation does not change the determinant. The resulting matrix is:

```math
M(t) =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1
\end{pmatrix}
```

### 2. Computing the Determinant

Expanding along the first column:

```math
\det(A(t))=\det(M(t))
=
1\begin{vmatrix}
0 & t-6 \\
1 & 1
\end{vmatrix}
=
0-(t-6)
=
6-t.
```

### 3. Finding the Noninvertible Case

A square matrix is not invertible exactly when its determinant is zero:

```math
6-t=0
\quad\Longrightarrow\quad
\boxed{t=6}.
```

### 4. What Happens to the Rows?

When t = 6, the original second row is twice the first row:

```math
\begin{pmatrix}
2 & 4 & 6
\end{pmatrix}
=
2\begin{pmatrix}
1 & 2 & 3
\end{pmatrix}.
```

Thus, the rows are linearly dependent. The required row operation produces a zero second row, confirming that the determinant is zero and the matrix is not invertible.
