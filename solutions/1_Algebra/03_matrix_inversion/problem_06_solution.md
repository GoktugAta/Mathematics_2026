# Problem 6 Solution

### 1. Computing the Inverse

```math
A =
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix},
\qquad
\det(A)=2\cdot3-1\cdot1=5.
```

Therefore:

```math
A^{-1} =
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}.
```

### 2. Solving the System

Multiply b by A⁻¹:

```math
x=A^{-1}b
=
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
5 \\
7
\end{pmatrix}
=
\frac15
\begin{pmatrix}
15-7 \\
-5+14
\end{pmatrix}
=
\begin{pmatrix}
\frac85 \\
\frac95
\end{pmatrix}.
```

### 3. Checking by Substitution

```math
Ax =
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac85 \\
\frac95
\end{pmatrix}
=
\begin{pmatrix}
\frac{16}{5}+\frac95 \\
\frac85+\frac{27}{5}
\end{pmatrix}
=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
=b.
```

Thus, the solution is verified.
