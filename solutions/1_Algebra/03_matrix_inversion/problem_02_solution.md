# Problem 2 Solution

### 1. Formula for a 2 × 2 Inverse

For a matrix with a nonzero determinant:

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

### 2. Computing the Inverse

```math
A =
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix},
\qquad
\det(A)=3\cdot4-2\cdot5=2.
```

Since the determinant is nonzero, the inverse exists:

```math
A^{-1}
=
\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}.
```

### 3. Verification

```math
AA^{-1}
=
\frac{1}{2}
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
=
\frac{1}{2}
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

The product confirms the result.
