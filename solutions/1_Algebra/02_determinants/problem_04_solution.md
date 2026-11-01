# Problem 4 Solution

### 1. Computing the Determinant

```math
A =
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7
\end{pmatrix}
```

A is upper triangular because all entries below the main diagonal are zero. Its determinant is the product of its diagonal entries:

```math
\det(A) = 2 \cdot (-3) \cdot 7 = -42.
```

### 2. General Rule

For any n × n upper or lower triangular matrix T:

```math
\det(T) = \prod_{i=1}^{n} t_{ii}
= t_{11}t_{22}\cdots t_{nn}.
```

In this example, the diagonal entries are 2, −3, and 7. The entries 4, 1, and 5 above the diagonal do not affect the determinant, so no expansion is needed.
