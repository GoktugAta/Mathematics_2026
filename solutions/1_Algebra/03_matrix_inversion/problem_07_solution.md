# Exercise 7. Inverse of a Product

## Question

For

```math
A =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix},
```

compute (AB)⁻¹ and B⁻¹A⁻¹. Check that the results are the same and explain the meaning of the reversed order.

## Solution

### Computing AB

```math
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
=
\begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}.
```

### Computing (AB)⁻¹

Since det(AB) = 6, the inverse formula gives:

```math
(AB)^{-1}=
\frac16
\begin{pmatrix}
3 & -3 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13
\end{pmatrix}.
```

### Computing B⁻¹A⁻¹

The individual inverses are:

```math
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix},
\qquad
B^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13
\end{pmatrix}.
```

Their product is:

```math
B^{-1}A^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13
\end{pmatrix}
=(AB)^{-1}.
```

### Explaining the Reversed Order

In ABx, B acts first and A acts second. To undo the transformation, we first undo A and then undo B. Therefore:

```math
(AB)^{-1}=B^{-1}A^{-1}.
```

The cancellation works in both directions:

```math
(AB)(B^{-1}A^{-1})
=A(BB^{-1})A^{-1}
=I,
```

```math
(B^{-1}A^{-1})(AB)
=B^{-1}(A^{-1}A)B
=I.
```
