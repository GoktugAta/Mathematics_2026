# Exercise 10. Columns of a Matrix Product

## Question

Given

```math
A =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1
\end{pmatrix},
```

denote the columns of B by b₁ and b₂.

1. Compute Ab₁ and Ab₂.
2. Compute the matrix AB.
3. Compare the results and explain why the columns of AB are exactly the vectors Ab₁ and Ab₂.

## Solution

### 1. Computing Ab₁ and Ab₂

The columns of B are:

```math
b_1 =
\begin{pmatrix}
1 \\
-1 \\
3
\end{pmatrix},
\qquad
b_2 =
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}.
```

Multiplying A by each column gives:

```math
Ab_1 =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 \\
-1 \\
3
\end{pmatrix}
=
\begin{pmatrix}
1-2+0 \\
0-1+3
\end{pmatrix}
=
\begin{pmatrix}
-1 \\
2
\end{pmatrix}.
```

```math
Ab_2 =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}
=
\begin{pmatrix}
2+0+0 \\
0+0+1
\end{pmatrix}
=
\begin{pmatrix}
2 \\
1
\end{pmatrix}.
```

### 2. Computing AB

```math
AB =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1
\end{pmatrix}
=
\begin{pmatrix}
1-2+0 & 2+0+0 \\
0-1+3 & 0+0+1
\end{pmatrix}
=
\begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}.
```

### 3. Comparing the Columns

The first column of AB is Ab₁, and the second is Ab₂:

```math
AB=
\begin{pmatrix}
Ab_1 & Ab_2
\end{pmatrix}.
```

By the definition of matrix multiplication, entry (i, j) of AB is the dot product of row i of A with column j of B. This is exactly entry i of Abⱼ.

Therefore, multiplying A by B applies A separately to each column of B.
