# Exercise 9. Composing Transformations

## Question

Let

```math
S =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix},
\qquad
R =
\begin{pmatrix}
0 & -1 \\
1 & 0
\end{pmatrix}.
```

The matrix S describes nonuniform scaling, while R describes a 90° counterclockwise rotation. For

```math
x =
\begin{pmatrix}
1 \\
2
\end{pmatrix},
```

compute RSx and SRx. Compare the results and explain geometrically why the order of these transformations matters.

## Solution

### 1. Computing RSx

The rightmost matrix acts first. First apply S:

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
\end{pmatrix}.
```

Then apply R:

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
\end{pmatrix}.
```

### 2. Computing SRx

First apply R:

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
\end{pmatrix}.
```

Then apply S:

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
\end{pmatrix}.
```

### 3. Comparison and Geometric Explanation

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
=SRx.
```

S doubles only the horizontal coordinate.

For RSx, this horizontal stretching occurs before the rotation. The rotation then turns the stretched horizontal component into a vertical component.

For SRx, rotation occurs first, and S then stretches the horizontal component of the rotated vector.

Because the scaling acts along a fixed horizontal axis, changing its order with the rotation changes the result.
