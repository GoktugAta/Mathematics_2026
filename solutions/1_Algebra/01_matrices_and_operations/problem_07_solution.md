# Problem 7 Solution

### 1. Identity and Zero Matrices

```math
I =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix},
\qquad
0 =
\begin{pmatrix}
0 & 0 \\
0 & 0
\end{pmatrix}
```

### 2. Computing AI and IA

```math
AI =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
```

```math
IA =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
```

The identity matrix is the neutral element for matrix multiplication: multiplying by I leaves A unchanged.

### 3. Computing A + 0

```math
A + 0 =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
+
\begin{pmatrix}
0 & 0 \\
0 & 0
\end{pmatrix}
=
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
```

The zero matrix is the neutral element for matrix addition: adding it leaves A unchanged.

### 4. Computing A²

```math
A^2 =
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
4 & 2+2 \\
0 & 4
\end{pmatrix}
=
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}
```

### 5. Computing A³

```math
A^3 = A^2 A =
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
8 & 4+8 \\
0 & 8
\end{pmatrix}
=
\begin{pmatrix}
8 & 12 \\
0 & 8
\end{pmatrix}
```

### 6. Pattern in Successive Powers

The diagonal entries are powers of 2, the lower-left entry stays zero, and the upper-right entry follows the pattern:

```math
1,\ 4,\ 12,\ 32,\ \ldots
```

For every integer n ≥ 1:

```math
A^n =
\begin{pmatrix}
2^n & n2^{n-1} \\
0 & 2^n
\end{pmatrix}
```

To explain this, write:

```math
A = 2I + N,
\qquad
N =
\begin{pmatrix}
0 & 1 \\
0 & 0
\end{pmatrix},
\qquad
N^2 = 0.
```

Since I and N commute and all terms containing higher powers of N vanish, the binomial expansion gives:

```math
A^n = (2I+N)^n = 2^n I + n2^{n-1}N.
```
