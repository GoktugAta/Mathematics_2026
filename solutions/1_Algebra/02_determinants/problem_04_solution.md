# Exercise 4. Triangular Matrix

## Question

Without expanding the determinant, compute:

```math
\det\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7
\end{pmatrix}.
```

State the rule for an arbitrary triangular matrix and explain using this example.

## Solution

The matrix is upper triangular because all entries below its main diagonal are zero.

The determinant of any upper or lower triangular matrix is the product of its diagonal entries. For an n × n triangular matrix T:

```math
\det(T)=t_{11}\cdot t_{22}\cdots t_{nn}.
```

In this example, the diagonal entries are 2, −3, and 7. Therefore:

```math
\det(A)=2\cdot(-3)\cdot7=-42.
```

The entries above the diagonal do not affect this product, so no determinant expansion is needed.
