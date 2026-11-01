# Problem 7 Solution

### 1. Computing AB

```math
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
=
\begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}.
```

### 2. Computing (AB)⁻¹

The determinant of AB is 6, so:

```math
(AB)^{-1} =
\frac16
\begin{pmatrix}
3 & -3 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13
\end{pmatrix}.
```

### 3. Computing B⁻¹A⁻¹

The individual inverses are:

```math
A^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix},
\qquad
B^{-1} =
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13
\end{pmatrix}.
```

Therefore:

```math
B^{-1}A^{-1} =
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13
\end{pmatrix}
=
(AB)^{-1}.
```

### 4. Meaning of the Reversed Order

In ABx, B acts first and A acts second. To undo the combined transformation, we must first undo A and then undo B.

This is why the inverse has the reversed order:

```math
(AB)^{-1}=B^{-1}A^{-1}.
```

Indeed:

```math
(AB)(B^{-1}A^{-1})
=
A(BB^{-1})A^{-1}
=
AA^{-1}
=
I.
```
