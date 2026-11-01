# Problem 1 Solution

### 1. Computing AB

```math
AB =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
=
\begin{pmatrix}
2-1 & -2+2 \\
1-1 & -1+2
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I.
```

### 2. Computing BA

```math
BA =
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
=
\begin{pmatrix}
2-1 & 1-1 \\
-2+2 & -1+2
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I.
```

### 3. Conclusion Using the Definition

By definition, B is the inverse of A if:

```math
AB = BA = I.
```

Both products equal the identity matrix. Therefore:

```math
\boxed{B=A^{-1}}.
```
