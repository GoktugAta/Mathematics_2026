# Exercise 5. A 3 × 3 Matrix

## Question

Use Gauss–Jordan elimination to find the inverse of

```math
A =
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}.
```

Check the result by multiplication.

## Solution

### Forming the Augmented Matrix

```math
[A \mid I]=
\left(
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
1 & 0 & 1 & 0 & 0 & 1
\end{array}
\right).
```

### Eliminating the First Entry of Row 3

Apply:

```math
R_3 \leftarrow R_3-R_1.
```

```math
\left(
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & -1 & 1 & -1 & 0 & 1
\end{array}
\right).
```

### Eliminating the Second Entry of Row 3

Apply:

```math
R_3 \leftarrow R_3+R_2.
```

```math
\left(
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & 0 & 2 & -1 & 1 & 1
\end{array}
\right).
```

### Normalizing the Third Pivot

Apply:

```math
R_3 \leftarrow \frac12R_3.
```

```math
\left(
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & 0 & 1 & -\frac12 & \frac12 & \frac12
\end{array}
\right).
```

### Eliminating Above the Third Pivot

Apply:

```math
R_2 \leftarrow R_2-R_3.
```

```math
\left(
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 0 & \frac12 & \frac12 & -\frac12 \\
0 & 0 & 1 & -\frac12 & \frac12 & \frac12
\end{array}
\right).
```

### Eliminating Above the Second Pivot

Apply:

```math
R_1 \leftarrow R_1-R_2.
```

```math
\left(
\begin{array}{ccc|ccc}
1 & 0 & 0 & \frac12 & -\frac12 & \frac12 \\
0 & 1 & 0 & \frac12 & \frac12 & -\frac12 \\
0 & 0 & 1 & -\frac12 & \frac12 & \frac12
\end{array}
\right).
```

The left block is now I, so the right block is A⁻¹:

```math
A^{-1}=
\frac12
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1
\end{pmatrix}.
```

### Verification

```math
AA^{-1}=
\frac12
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1
\end{pmatrix}
=
\frac12
\begin{pmatrix}
2 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 2
\end{pmatrix}
=I.
```

The product confirms the inverse.
