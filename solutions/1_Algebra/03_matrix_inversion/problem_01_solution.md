# Exercise 1. Definition of the Inverse

## Question

For

```math
A =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix},
```

check, without using a formula, whether B = A⁻¹. Compute AB and BA and relate the result to the definition of the inverse.

## Solution

### Computing AB

We multiply each row of A by each column of B:

```math
AB =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
=
\begin{pmatrix}
2-1 & -2+2 \\
1-1 & -1+2
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
```

### Computing BA

```math
BA =
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
=
\begin{pmatrix}
2-1 & 1-1 \\
-2+2 & -1+2
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}.
```

### Conclusion

By definition, an inverse must satisfy both AB = I and BA = I. Both products equal the identity matrix, so:

```math
\boxed{B=A^{-1}}.
```
