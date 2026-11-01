# Problem 12 Solution

### 1. Computing A²

```math
A^2 =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
```

### 2. Computing A³

```math
A^3 = A^2 A =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
```

### 3. Computing A⁴

```math
A^4 = A^3 A =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}
```

### 4. Conjecture for Aⁿ

The diagonal entries remain 1, the lower-left entry remains 0, and the upper-right entry increases by 1 with each multiplication by A.

We conjecture that for every integer n ≥ 1:

```math
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
```

### 5. Proof by Mathematical Induction

For n = 1, the formula gives the original matrix:

```math
A^1 =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

Assume the formula holds for some integer n ≥ 1:

```math
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
```

Multiplying by A gives:

```math
A^{n+1} = A^n A =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
1 \cdot 1 + n \cdot 0 & 1 \cdot 1 + n \cdot 1 \\
0 \cdot 1 + 1 \cdot 0 & 0 \cdot 1 + 1 \cdot 1
\end{pmatrix}
=
\begin{pmatrix}
1 & n+1 \\
0 & 1
\end{pmatrix}
```

This is exactly the conjectured formula with n replaced by n + 1. Therefore, by mathematical induction, the formula holds for every integer n ≥ 1.
