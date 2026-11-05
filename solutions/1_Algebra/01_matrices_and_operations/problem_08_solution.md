# Exercise 8. Row Operations and Their Reversibility

## Question

For

```math
A =
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix},
```

perform, in order:

1. R₂ ← R₂ − 2R₁.
2. R₃ ← R₃ + R₁.
3. Interchange R₂ and R₃.

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

## Solution

### 1. First Operation

Subtract twice the first row from the second:

```math
R_2\leftarrow R_2-2R_1.
```

The new second row is:

```math
\begin{pmatrix}
2 & 4 & 1
\end{pmatrix}
-
2\begin{pmatrix}
1 & 2 & -1
\end{pmatrix}
=
\begin{pmatrix}
0 & 0 & 3
\end{pmatrix}.
```

The matrix becomes:

```math
A_1 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}.
```

The operation that reverses this step is:

```math
R_2\leftarrow R_2+2R_1.
```

### 2. Second Operation

Add the first row to the third:

```math
R_3\leftarrow R_3+R_1.
```

The matrix becomes:

```math
A_2 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}.
```

The operation that reverses this step is:

```math
R_3\leftarrow R_3-R_1.
```

### 3. Third Operation

Interchange the second and third rows:

```math
R_2\leftrightarrow R_3.
```

The matrix becomes:

```math
A_3 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}.
```

A row interchange is reversed by performing the same interchange again:

```math
R_2\leftrightarrow R_3.
```

### 4. Reversing the Entire Process

To recover A from A₃, apply the inverse operations in reverse order:

```math
R_2\leftrightarrow R_3,
\qquad
R_3\leftarrow R_3-R_1,
\qquad
R_2\leftarrow R_2+2R_1.
```

These steps restore the original matrix.
