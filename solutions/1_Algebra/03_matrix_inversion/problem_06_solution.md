# Exercise 6. Solving a System Using the Inverse

## Question

Solve Ax = b, where

```math
A =
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix},
\qquad
b =
\begin{pmatrix}
5 \\
7
\end{pmatrix},
```

using x = A⁻¹b. Then substitute the resulting vector back into the equation and check the result.

## Solution

### Computing the Inverse

```math
\det(A)=2\cdot3-1\cdot1=5.
```

Since the determinant is nonzero, A is invertible. The 2 × 2 inverse formula gives:

```math
A^{-1}=
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}.
```

### Computing the Solution

Multiplying Ax = b on the left by A⁻¹ gives x = A⁻¹b:

```math
x=
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
5 \\
7
\end{pmatrix}
=
\frac15
\begin{pmatrix}
15-7 \\
-5+14
\end{pmatrix}
=
\begin{pmatrix}
\frac85 \\
\frac95
\end{pmatrix}.
```

### Checking by Substitution

```math
Ax=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac85 \\
\frac95
\end{pmatrix}
=
\begin{pmatrix}
\frac{16}{5}+\frac95 \\
\frac85+\frac{27}{5}
\end{pmatrix}
=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
=b.
```

Thus, the solution satisfies the original system.
