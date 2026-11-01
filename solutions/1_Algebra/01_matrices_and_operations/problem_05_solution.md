# Problem 5 Solution

### 1. Computing Ax

$$
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
2 \cdot 4 + (-1) \cdot 2 \\
1 \cdot 4 + 3 \cdot 2
\end{pmatrix}
=
\begin{pmatrix}
6 \\
10
\end{pmatrix}
$$

### 2. Linear Combination of the Columns of A

The columns of $A$ are:

$$
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
\end{pmatrix}
$$

Using the entries of $x$ as coefficients:

$$
Ax = 4a_1 + 2a_2
=
4
\begin{pmatrix}
2 \\
1
\end{pmatrix}
+
2
\begin{pmatrix}
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
\end{pmatrix}
$$

Thus, $Ax$ is a linear combination of the columns of $A$,
with coefficients $4$ and $2$ from the vector $x$.
