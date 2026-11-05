# Exercise 13. Undoing a Composite Transformation

## Question

The matrices

```math
S =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix},
\qquad
H =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

describe nonuniform scaling and shear. For T = HS, find T⁻¹ in two ways:

1. First compute T, then its inverse.
2. Use (HS)⁻¹ = S⁻¹H⁻¹.

Compare the results. Additionally compute H⁻¹S⁻¹ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

## Solution

### 1. Computing T and Then Its Inverse

First multiply H by S:

```math
T=HS =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}.
```

Since det(T) = 2, the inverse exists. The 2 × 2 inverse formula gives:

```math
T^{-1} =
\frac12
\begin{pmatrix}
1 & -1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1
\end{pmatrix}.
```

### 2. Using the Inverse-of-a-Product Property

The individual inverses are:

```math
S^{-1} =
\begin{pmatrix}
\frac12 & 0 \\
0 & 1
\end{pmatrix},
\qquad
H^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}.
```

Therefore:

```math
(HS)^{-1}=S^{-1}H^{-1}
=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1
\end{pmatrix}.
```

Both methods give the same inverse.

### 3. Checking the Incorrect Order

Reversing the factors in this last product gives:

```math
H^{-1}S^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -1 \\
0 & 1
\end{pmatrix}.
```

This differs from T⁻¹ in its upper-right entry. It does not undo T:

```math
T(H^{-1}S^{-1}) =
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac12 & -1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\neq I.
```

### 4. Geometric Explanation

In Tx = HSx, scaling by S happens first, followed by shearing by H.

To restore the original vector, we must first undo the last operation, the shear, using H⁻¹. Then we undo the scaling using S⁻¹.

Since the rightmost matrix acts first, this reverse sequence is represented by S⁻¹H⁻¹.
