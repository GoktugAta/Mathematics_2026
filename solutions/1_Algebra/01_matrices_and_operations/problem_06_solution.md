# Problem 6 Solution

### 1. Computing Aᵀ

Transposing interchanges rows and columns:

```math
A^T =
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix}
```

### 2. Computing Bᵀ

```math
B^T =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix}
```

### 3. Computing AB

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
\end{pmatrix}
=
\begin{pmatrix}
1+4-3 & 0+2+9 \\
4+10-6 & 0+5+18
\end{pmatrix}
=
\begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}
```

### 4. Computing (AB)ᵀ

```math
(AB)^T =
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
```

### 5. Computing BᵀAᵀ

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
\end{pmatrix}
=
\begin{pmatrix}
1+4-3 & 4+10-6 \\
0+2+9 & 0+5+18
\end{pmatrix}
=
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
```

### 6. Verification

Both calculations give the same matrix. Therefore:

```math
(AB)^T = B^T A^T =
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix}
```
