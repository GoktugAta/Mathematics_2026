# Problem 6 Solution

### 1. Computing $A^T$ and $B^T$

```math
A^T =
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
```

```math
B^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
```

### 2. Computing $AB$ and $(AB)^T$

```math
AB =
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix} =
\begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}
```

```math
(AB)^T =
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
```

### 3. Computing $B^T A^T$ and Verification

```math
B^T A^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix} =
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
```

Since $(AB)^T = B^T A^T = \begin{pmatrix} 2 & 8 \\ 11 & 23 \end{pmatrix}$, the property is verified.
