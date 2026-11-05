# Exercise 14. A Matrix That Is Its Own Inverse

## Question

Assume that a square matrix A satisfies:

```math
A^2=I.
```

Show that:

```math
A^{-1}=A.
```

Then give an example of a 2 × 2 matrix different from I and −I that satisfies this condition, and verify it by multiplication.

## Solution

### 1. Using the Definition of the Inverse

We are given:

```math
A^2=AA=I.
```

By definition, a matrix B is the inverse of A when AB = BA = I.

Taking B = A satisfies both conditions because AA = I. Therefore, A is invertible and:

```math
A^{-1}=A.
```

### 2. An Example

Choose:

```math
A =
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}.
```

This matrix is different from both I and −I.

### 3. Verification

```math
A^2 =
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
=
\begin{pmatrix}
0+1 & 0+0 \\
0+0 & 1+0
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I.
```

Thus, this matrix is its own inverse. Geometrically, it swaps the two coordinates; performing the swap twice restores the original vector.
