# Exercise 2. Formula for a 2 × 2 Matrix

## Question

Find the inverse of

```math
A =
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
```

using the formula for a 2 × 2 matrix. At the end, check the result by computing one product with A.

## Solution

### Computing the Inverse

For a 2 × 2 matrix with a nonzero determinant:

```math
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}^{-1}
=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}.
```

First, calculate the determinant:

```math
\det(A)=3\cdot4-2\cdot5=12-10=2.
```

Since the determinant is nonzero, the inverse exists. Applying the formula:

```math
A^{-1}=
\frac12
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
=
\begin{pmatrix}
2 & -1 \\
-\frac52 & \frac32
\end{pmatrix}.
```

### Verification

We multiply A by the proposed inverse:

```math
AA^{-1}
=
\frac12
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
=
\frac12
\begin{pmatrix}
12-10 & -6+6 \\
20-20 & -10+12
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I.
```

The identity product confirms the inverse.
