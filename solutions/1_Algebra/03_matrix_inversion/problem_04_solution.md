# Exercise 4. Gauss–Jordan

## Question

Find A⁻¹ using the Gauss–Jordan method for

```math
A =
\begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}.
```

Show the augmented matrix [A | I] after successive operations and explain why obtaining I on the left gives the inverse on the right.

## Solution

### Forming the Augmented Matrix

We apply the same row operations to A and I:

```math
[A \mid I]=
\left(
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
3 & 5 & 0 & 1
\end{array}
\right).
```

### Eliminating Below the First Pivot

Apply:

```math
R_2 \leftarrow R_2-3R_1.
```

```math
\left(
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & -1 & -3 & 1
\end{array}
\right).
```

### Normalizing the Second Pivot

Apply:

```math
R_2 \leftarrow -R_2.
```

```math
\left(
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & 1 & 3 & -1
\end{array}
\right).
```

### Eliminating Above the Second Pivot

Apply:

```math
R_1 \leftarrow R_1-2R_2.
```

```math
\left(
\begin{array}{cc|cc}
1 & 0 & -5 & 2 \\
0 & 1 & 3 & -1
\end{array}
\right)
=[I \mid A^{-1}].
```

Therefore:

```math
\boxed{
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
}.
```

### Why the Method Works

Each row operation is multiplication on the left by an invertible elementary matrix. If E represents the combined operations, then:

```math
[A \mid I]\longrightarrow[EA \mid EI].
```

The left block becomes I, so EA = I. Hence E = A⁻¹, and the right block is EI = E = A⁻¹.
