# Exercise 1. Determinant of a 2 × 2 Matrix

## Question

Compute:

```math
\det\begin{pmatrix}
3 & -2 \\
5 & 4
\end{pmatrix},
\qquad
\det\begin{pmatrix}
1 & 7 \\
2 & 14
\end{pmatrix}.
```

Which matrix is invertible? Justify your answer.

## Solution

For a 2 × 2 matrix, the determinant is:

```math
\det\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}=ad-bc.
```

For the first matrix:

```math
3\cdot4-(-2)\cdot5=12+10=22.
```

For the second matrix:

```math
1\cdot14-7\cdot2=14-14=0.
```

A square matrix is invertible if and only if its determinant is nonzero. Therefore, the first matrix is invertible, while the second is not.
