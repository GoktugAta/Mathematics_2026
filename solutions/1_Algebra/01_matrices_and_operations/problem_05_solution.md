# Exercise 5. Matrix Times Vector

## Question

Let

```math
A =
\begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix},
\qquad
x =
\begin{pmatrix}
4 \\
2
\end{pmatrix}.
```

Compute Ax. Then express Ax as a linear combination of the columns of A, with coefficients coming from the vector x.

## Solution

### 1. Computing Ax

Multiply each row of A by the column vector x:

```math
Ax =
\begin{pmatrix}
2 & -1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
4 \\
2
\end{pmatrix}
=
\begin{pmatrix}
2\cdot4-1\cdot2 \\
1\cdot4+3\cdot2
\end{pmatrix}
=
\begin{pmatrix}
6 \\
10
\end{pmatrix}.
```

### 2. Linear Combination of the Columns

The columns of A are:

```math
a_1 =
\begin{pmatrix}
2 \\
1
\end{pmatrix},
\qquad
a_2 =
\begin{pmatrix}
-1 \\
3
\end{pmatrix}.
```

The entries of x give the coefficients 4 and 2:

```math
Ax=4a_1+2a_2
=
4\begin{pmatrix}
2 \\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1 \\
3
\end{pmatrix}
=
\begin{pmatrix}
8 \\
4
\end{pmatrix}
+
\begin{pmatrix}
-2 \\
6
\end{pmatrix}
=
\begin{pmatrix}
6 \\
10
\end{pmatrix}.
```

Thus, matrix-vector multiplication combines the columns of A using the corresponding entries of x as coefficients.
