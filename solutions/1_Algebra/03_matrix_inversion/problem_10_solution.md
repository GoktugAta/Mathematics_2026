# Exercise 10. Inverse of a Diagonal Matrix

## Question

Given

```math
D =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix},
\qquad
E =
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5
\end{pmatrix},
```

without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

## Solution

### 1. Deciding Invertibility

A diagonal matrix is invertible if and only if every diagonal entry is nonzero.

The diagonal entries of D are 2, −3, and 5, so D is invertible.

E has a zero diagonal entry and a zero second row. Therefore, E is not invertible. In particular:

```math
\det(E)=2\cdot0\cdot5=0.
```

### 2. Finding the Inverse of D

For an invertible diagonal matrix, the inverse contains the reciprocals of the diagonal entries:

```math
D^{-1} =
\begin{pmatrix}
\frac12 & 0 & 0 \\
0 & -\frac13 & 0 \\
0 & 0 & \frac15
\end{pmatrix}.
```

### 3. Checking by Multiplication

```math
DD^{-1} =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 & 0 \\
0 & -\frac13 & 0 \\
0 & 0 & \frac15
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
=I.
```

Multiplication in the reverse order gives the same identity matrix because both matrices are diagonal. Thus, the inverse is verified.
