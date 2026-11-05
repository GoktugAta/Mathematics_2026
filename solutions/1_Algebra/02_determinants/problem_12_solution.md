# Exercise 12. A Parameter Revealed by a Row Operation

## Question

For

```math
A(t) =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1
\end{pmatrix},
```

find the values of t for which the matrix is not invertible.

Before computing the determinant, perform the operation:

```math
R_2\leftarrow R_2-2R_1
```

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

## Solution

### 1. Performing the Required Operation

Apply:

```math
R_2\leftarrow R_2-2R_1.
```

This row replacement preserves the determinant and gives:

```math
M(t) =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1
\end{pmatrix}.
```

### 2. Computing the Determinant

Expanding along the first column:

```math
\det(A(t))
=\det(M(t))
=
\begin{vmatrix}
0 & t-6 \\
1 & 1
\end{vmatrix}
=0-(t-6)=6-t.
```

### 3. Finding the Exceptional Value

The matrix is not invertible exactly when its determinant is zero:

```math
6-t=0
\quad\Longrightarrow\quad
t=6.
```

### 4. Row Dependence at t = 6

At t = 6, the original second row is twice the first:

```math
\begin{pmatrix}
2 & 4 & 6
\end{pmatrix}
=
2\begin{pmatrix}
1 & 2 & 3
\end{pmatrix}.
```

Therefore, the rows are linearly dependent. The required operation produces a zero second row, explaining why the determinant vanishes.
