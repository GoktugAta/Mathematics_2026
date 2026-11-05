# Exercise 12. Finding Inverses Without Starting from Scratch

## Question

It is known that:

```math
A^{-1} =
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}.
```

Without finding A, compute (3A)⁻¹, (Aᵀ)⁻¹, and (A²)⁻¹. Justify each result using the appropriate property.

## Solution

### 1. Computing (3A)⁻¹

For a nonzero scalar c and an invertible matrix A:

```math
(cA)^{-1}=\frac1cA^{-1}.
```

This works because the scalar factors c and 1/c cancel when the matrices are multiplied. Therefore:

```math
(3A)^{-1} =
\frac13
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
=
\begin{pmatrix}
\frac23 & -\frac13 \\
-1 & \frac23
\end{pmatrix}.
```

### 2. Computing (Aᵀ)⁻¹

The inverse of a transpose equals the transpose of the inverse:

```math
(A^T)^{-1}=(A^{-1})^T.
```

Thus, we interchange the rows and columns of the given inverse:

```math
(A^T)^{-1} =
\begin{pmatrix}
2 & -3 \\
-1 & 2
\end{pmatrix}.
```

### 3. Computing (A²)⁻¹

Using the inverse-of-a-product property:

```math
(A^2)^{-1}
=(AA)^{-1}
=A^{-1}A^{-1}
=(A^{-1})^2.
```

Therefore:

```math
(A^2)^{-1} =
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
=
\begin{pmatrix}
4+3 & -2-2 \\
-6-6 & 3+4
\end{pmatrix}
=
\begin{pmatrix}
7 & -4 \\
-12 & 7
\end{pmatrix}.
```

All three results were obtained directly from the given inverse without computing A.
