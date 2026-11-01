# Problem 9 Solution

### 1. Choosing the Correct Side

We need to solve:

```math
AX=B.
```

Since A multiplies X on the left, we multiply both sides by A⁻¹ on the left:

```math
A^{-1}(AX)=A^{-1}B.
```

By associativity:

```math
(A^{-1}A)X=IX=X,
```

so:

```math
X=A^{-1}B.
```

### 2. Computing A⁻¹

```math
A =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix},
\qquad
A^{-1} =
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}.
```

### 3. Computing X

```math
X =
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
=
\begin{pmatrix}
3-4 & 1-8 \\
2 & 4
\end{pmatrix}
=
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}.
```

### 4. Verification

```math
AX =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
=
\begin{pmatrix}
-1+4 & -7+8 \\
2 & 4
\end{pmatrix}
=
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
=B.
```

Therefore, the solution is verified.
