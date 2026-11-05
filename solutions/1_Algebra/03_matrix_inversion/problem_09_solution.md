# Exercise 9. Matrix Equation

## Question

Given

```math
A =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix},
```

solve the equation AX = B for X. Before calculating, decide on which side of the equation A⁻¹ must be used. Then check the result by computing AX.

## Solution

### Choosing the Correct Side

A multiplies X on the left, so we multiply both sides of AX = B by A⁻¹ on the left:

```math
A^{-1}(AX)=A^{-1}B.
```

By associativity:

```math
(A^{-1}A)X=IX=X.
```

Therefore:

```math
X=A^{-1}B.
```

### Computing the Inverse

```math
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}.
```

### Computing X

```math
X=
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

### Verification

```math
AX=
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

Thus, X satisfies the original matrix equation.
