# Exercise 1. Matrix Size and Entries

## Question

Given

```math
A =
\begin{pmatrix}
2 & -1 & 3 \\
0 & 4 & 5
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
1 & 0 \\
-2 & 3 \\
4 & 1
\end{pmatrix},
```

1. State the sizes of matrices A and B.
2. Read off the entries a₁₂, a₂₃, b₂₁, and b₃₂.
3. Write the second row of A and the first column of B as vectors.

## Solution

### 1. Matrix Sizes

Matrix size is written as the number of rows × the number of columns.

A has two rows and three columns, while B has three rows and two columns:

```math
\operatorname{size}(A)=2\times3,
\qquad
\operatorname{size}(B)=3\times2.
```

### 2. Requested Entries

The first index specifies the row, and the second index specifies the column:

```math
a_{12}=-1,
\qquad
a_{23}=5,
\qquad
b_{21}=-2,
\qquad
b_{32}=1.
```

### 3. Row and Column Vectors

The second row of A is a horizontal 1 × 3 vector:

```math
\begin{pmatrix}
0 & 4 & 5
\end{pmatrix}.
```

The first column of B is a vertical 3 × 1 vector:

```math
\begin{pmatrix}
1 \\
-2 \\
4
\end{pmatrix}.
```
