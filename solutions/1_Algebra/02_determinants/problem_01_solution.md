# Problem 1 Solution

### 1. Determinant Formula

For a 2 × 2 matrix:

```math
\det\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
= ad-bc.
```

### 2. First Matrix

```math
A =
\begin{pmatrix}
3 & -2 \\
5 & 4
\end{pmatrix}
```

```math
\det(A) = 3 \cdot 4 - (-2)\cdot 5
= 12+10
= 22.
```

### 3. Second Matrix

```math
B =
\begin{pmatrix}
1 & 7 \\
2 & 14
\end{pmatrix}
```

```math
\det(B) = 1 \cdot 14 - 7 \cdot 2
= 14-14
= 0.
```

### 4. Invertibility

A square matrix is invertible if and only if its determinant is nonzero.

Since det(A) = 22, the first matrix is invertible.

Since det(B) = 0, the second matrix is not invertible. Its second row is twice its first row, so its rows are linearly dependent.
