# Exercise 8. Inverse of a Transformation

## Question

The matrix

```math
S =
\begin{pmatrix}
2 & 0 \\
0 & \frac12
\end{pmatrix}
```

describes a scaling of the plane. Find S⁻¹ and explain geometrically what the inverse transformation does. Check the action of the pair S, S⁻¹ on one simple vector.

## Solution

### Finding the Inverse

To reverse a nonzero scaling factor, we multiply by its reciprocal. Therefore:

```math
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 2
\end{pmatrix}.
```

Indeed:

```math
SS^{-1}=
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
=I.
```

### Geometric Interpretation

S doubles the horizontal coordinate and halves the vertical coordinate.

S⁻¹ reverses these changes: it halves the horizontal coordinate and doubles the vertical coordinate.

### Checking on a Vector

Choose:

```math
v=
\begin{pmatrix}
1 \\
2
\end{pmatrix}.
```

First, apply S:

```math
Sv=
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
S^{-1}(Sv)=
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

The inverse transformation restores the original vector.
