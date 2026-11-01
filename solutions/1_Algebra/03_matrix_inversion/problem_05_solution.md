# Problem 5 Solution

### 1. Form the Augmented Matrix

```math
[A \mid I] =
\left(
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
1 & 0 & 1 & 0 & 0 & 1
\end{array}
\right).
```

### 2. Eliminate the First Entry of Row 3

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

### 3. Eliminate the Second Entry of Row 3

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

### 4. Normalize the Third Pivot

Apply:

```math
R_3 \leftarrow \frac{1}{2}R_3.
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

### 5. Eliminate the Third Entry of Row 2

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

### 6. Eliminate the Second Entry of Row 1

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

Thus:

```math
A^{-1} =
\frac12
\begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1
\end{pmatrix}.
```

### 7. Verification by Multiplication

```math
AA^{-1} =
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
= I.
```
