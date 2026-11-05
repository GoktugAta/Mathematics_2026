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

The size of a matrix is its number of rows × its number of columns.

A has 2 rows and 3 columns, so its size is:

```math
2\times3.
```

B has 3 rows and 2 columns, so its size is:

```math
3\times2.
```

### 2. Requested Entries

The first index indicates the row, and the second index indicates the column. Reading the specified positions gives:

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

The second row of A is the horizontal 1 × 3 vector:

```math
\begin{pmatrix}
0 & 4 & 5
\end{pmatrix}.
```

The first column of B is the vertical 3 × 1 vector:

```math
\begin{pmatrix}
1 \\
-2 \\
4
\end{pmatrix}.
```
