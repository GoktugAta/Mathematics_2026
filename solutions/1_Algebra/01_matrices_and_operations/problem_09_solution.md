# Problem 9 Solution

### 1. Computing RSx

The rightmost transformation acts first, so we first apply S:

```math
Sx =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 \\
2
\end{pmatrix}
=
\begin{pmatrix}
2 \\
2
\end{pmatrix}
```

Then we apply R:

```math
RSx =
\begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
2 \\
2
\end{pmatrix}
=
\begin{pmatrix}
-2 \\
2
\end{pmatrix}
```

### 2. Computing SRx

First, we apply R:

```math
Rx =
\begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 \\
2
\end{pmatrix}
=
\begin{pmatrix}
-2 \\
1
\end{pmatrix}
```

Then we apply S:

```math
SRx =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-2 \\
1
\end{pmatrix}
=
\begin{pmatrix}
-4 \\
1
\end{pmatrix}
```

### 3. Comparison

```math
RSx =
\begin{pmatrix}
-2 \\
2
\end{pmatrix}
\neq
\begin{pmatrix}
-4 \\
1
\end{pmatrix}
= SRx
```

Thus, the order of the transformations matters.

### 4. Geometric Explanation

S doubles the horizontal coordinate and leaves the vertical coordinate unchanged. R rotates a vector 90 degrees counterclockwise.

For RSx, the horizontal coordinate is doubled before rotation. The rotation then turns this stretched horizontal component into a vertical component.

For SRx, the vector is rotated first. S then doubles the horizontal coordinate of the rotated vector.

Because the scaling acts only along the horizontal axis, changing its order with the rotation produces different results.
