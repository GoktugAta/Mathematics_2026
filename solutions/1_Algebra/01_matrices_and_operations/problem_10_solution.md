# Problem 10 Solution

### 1. Computing Ab₁ and Ab₂

The columns of B are:

```math
b_1 =
\begin{pmatrix}
1 \\
-1 \\
3
\end{pmatrix},
\qquad
b_2 =
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}
```

Multiplying A by the first column:

```math
Ab_1 =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 \\
-1 \\
3
\end{pmatrix}
=
\begin{pmatrix}
1-2+0 \\
0-1+3
\end{pmatrix}
=
\begin{pmatrix}
-1 \\
2
\end{pmatrix}
```

Multiplying A by the second column:

```math
Ab_2 =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}
=
\begin{pmatrix}
2+0+0 \\
0+0+1
\end{pmatrix}
=
\begin{pmatrix}
2 \\
1
\end{pmatrix}
```

### 2. Computing AB

```math
AB =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1
\end{pmatrix}
=
\begin{pmatrix}
1-2+0 & 2+0+0 \\
0-1+3 & 0+0+1
\end{pmatrix}
=
\begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}
```

### 3. Comparison and Explanation

The first column of AB equals Ab₁, and the second column equals Ab₂:

```math
AB =
\begin{pmatrix}
\vert & \vert \\
Ab_1 & Ab_2 \\
\vert & \vert
\end{pmatrix}
=
\begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}
```

By the definition of matrix multiplication, entry (i, j) of AB is the dot product of row i of A with column j of B. These are exactly the entries of Abⱼ.

Therefore, multiplying A by B applies A separately to each column of B.
