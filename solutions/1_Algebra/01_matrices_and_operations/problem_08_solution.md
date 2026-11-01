# Problem 8 Solution

### 1. First Row Operation

Subtract twice the first row from the second row:

```math
R_2 \leftarrow R_2 - 2R_1
```

```math
R_2 =
\begin{pmatrix}
2 & 4 & 1
\end{pmatrix}
-
2\begin{pmatrix}
1 & 2 & -1
\end{pmatrix}
=
\begin{pmatrix}
0 & 0 & 3
\end{pmatrix}
```

The matrix becomes:

```math
A_1 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}
```

The inverse operation is:

```math
R_2 \leftarrow R_2 + 2R_1
```

### 2. Second Row Operation

Add the first row to the third row:

```math
R_3 \leftarrow R_3 + R_1
```

```math
R_3 =
\begin{pmatrix}
-1 & 1 & 3
\end{pmatrix}
+
\begin{pmatrix}
1 & 2 & -1
\end{pmatrix}
=
\begin{pmatrix}
0 & 3 & 2
\end{pmatrix}
```

The matrix becomes:

```math
A_2 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}
```

The inverse operation is:

```math
R_3 \leftarrow R_3 - R_1
```

### 3. Third Row Operation

Interchange the second and third rows:

```math
R_2 \leftrightarrow R_3
```

The matrix becomes:

```math
A_3 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
```

The inverse operation is the same interchange:

```math
R_2 \leftrightarrow R_3
```

### 4. Reversibility

To recover the original matrix from the final matrix, apply the inverse operations in reverse order:

```math
R_2 \leftrightarrow R_3,
\qquad
R_3 \leftarrow R_3 - R_1,
\qquad
R_2 \leftarrow R_2 + 2R_1.
```

This restores:

```math
A =
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}
```
