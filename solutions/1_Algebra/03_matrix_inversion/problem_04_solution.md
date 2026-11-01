# Problem 4 Solution

### 1. Form the Augmented Matrix

```math
[A \mid I]
=
\left(
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
3 & 5 & 0 & 1
\end{array}
\right).
```

### 2. Eliminate the First Entry of Row 2

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

### 3. Make the Second Pivot Equal to 1

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

### 4. Eliminate the Second Entry of Row 1

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
=
[I \mid A^{-1}].
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

### 5. Why the Method Works

Each row operation is equivalent to multiplication on the left by an elementary matrix. Let E be the product of these elementary matrices.

Applying the same operations to both sides of the augmented matrix gives:

```math
[A \mid I]
\longrightarrow
[EA \mid EI].
```

Since the left side becomes I:

```math
EA=I
\quad\Longrightarrow\quad
E=A^{-1}.
```

The right side becomes EI = E = A⁻¹, which explains why it contains the inverse.
