# Problem 8 Solution

### 1. Finding the Inverse

```math
S =
\begin{pmatrix}
2 & 0 \\
0 & \frac12
\end{pmatrix}.
```

The inverse of a diagonal scaling matrix is obtained by taking the reciprocal of each diagonal entry:

```math
S^{-1} =
\begin{pmatrix}
\frac12 & 0 \\
0 & 2
\end{pmatrix}.
```

Indeed:

```math
SS^{-1} =
\begin{pmatrix}
2 & 0 \\
0 & \frac12
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 \\
0 & 2
\end{pmatrix}
=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
= I.
```

### 2. Geometric Interpretation

S doubles the horizontal coordinate and halves the vertical coordinate.

Its inverse reverses these changes: S⁻¹ halves the horizontal coordinate and doubles the vertical coordinate.

### 3. Checking on a Simple Vector

Choose:

```math
v =
\begin{pmatrix}
1 \\
2
\end{pmatrix}.
```

First apply S:

```math
Sv =
\begin{pmatrix}
2 & 0 \\
0 & \frac12
\end{pmatrix}
\begin{pmatrix}
1 \\
2
\end{pmatrix}
=
\begin{pmatrix}
2 \\
1
\end{pmatrix}.
```

Then apply S⁻¹:

```math
S^{-1}(Sv) =
\begin{pmatrix}
\frac12 & 0 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
2 \\
1
\end{pmatrix}
=
\begin{pmatrix}
1 \\
2
\end{pmatrix}
=v.
```

Thus, the inverse transformation restores the original vector.
