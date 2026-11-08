# Exercise 4. Gauss–Jordan

## Question

Find A⁻¹ using the Gauss–Jordan method for:

```math
A =
\begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}.
```

Show the augmented matrix [A | I] after successive operations and explain why obtaining I on the left gives the inverse on the right.

## Solution

### 1. Forming the Augmented Matrix

Place the identity matrix to the right of A:

```math
[A \mid I] =
\left(
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
3 & 5 & 0 & 1
\end{array}
\right).
```

We apply every row operation to the entire augmented matrix.

### 2. Eliminating Below the First Pivot

Apply:

```math
R_2\leftarrow R_2-3R_1.
```

```math
\left(
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & -1 & -3 & 1
\end{array}
\right).
```

### 3. Normalizing the Second Pivot

Apply:

```math
R_2\leftarrow -R_2.
```

```math
\left(
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & 1 & 3 & -1
\end{array}
\right).
```

### 4. Eliminating Above the Second Pivot

Apply:

```math
R_1\leftarrow R_1-2R_2.
```

```math
\left(
\begin{array}{cc|cc}
1 & 0 & -5 & 2 \\
0 & 1 & 3 & -1
\end{array}
\right).
```

The left block is now I, so:

```math
A^{-1} =
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}.
```

### 5. Why the Method Works

Each row operation is equivalent to multiplication on the left by an invertible elementary matrix. Let E represent their combined effect.

Applying the operations to both blocks gives:

```math
[A \mid I]\longrightarrow[EA \mid EI].
```

The left block becomes I, so EA = I. Since E is invertible, A = E⁻¹ and therefore A⁻¹ = E.

The right block is EI = E, which explains why it contains A⁻¹.

### 6. Verification

```math
AA^{-1} =
\begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
=
\begin{pmatrix}
-5+6 & 2-2 \\
-15+15 & 6-5
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=I.
```

The product confirms the inverse.
