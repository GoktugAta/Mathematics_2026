# Exercise 7. Choosing a Method Deliberately

## Question

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. One system with a triangular coefficient matrix:

```math
\begin{cases}
2x-y=3, \\
4y=8;
\end{cases}
```

2. Three systems Ax = bᵢ with the same invertible matrix A, when A⁻¹ is already known.
3. One 3 × 3 system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary. Do not judge a method by its name alone — refer to the number of right-hand sides and the structure of the matrix.

## Solution

### 1. Triangular System: Back Substitution

The coefficient matrix is upper triangular:

```math
A =
\begin{pmatrix}
2 & -1 \\
0 & 4
\end{pmatrix}.
```

No elimination is needed because the second equation already contains only y.

From the second equation:

```math
4y=8
\quad\Longrightarrow\quad
y=2.
```

Substitute into the first equation:

```math
2x-2=3
\quad\Longrightarrow\quad
2x=5
\quad\Longrightarrow\quad
x=\frac52.
```

Therefore:

```math
\begin{pmatrix}
x \\
y
\end{pmatrix}
=
\begin{pmatrix}
\frac52 \\
2
\end{pmatrix}.
```

Checking:

```math
2\left(\frac52\right)-2=3,
\qquad
4(2)=8.
```

Back substitution directly uses the triangular structure. Computing an inverse or performing further elimination would be unnecessary.

### 2. Three Right-Hand Sides with a Known Inverse

Use the inverse that is already available:

```math
x_i=A^{-1}b_i,
\qquad i=1,2,3.
```

The same inverse is reused for all three right-hand sides. Only the matrix-vector multiplication changes.

Equivalently, collect the vectors as columns and compute:

```math
\begin{pmatrix}
x_1 & x_2 & x_3
\end{pmatrix}
=
A^{-1}
\begin{pmatrix}
b_1 & b_2 & b_3
\end{pmatrix}.
```

Here, each xᵢ is a solution vector. Recomputing the inverse would be unnecessary.

### 3. One 3 × 3 System with No Inverse Given

Use Gaussian elimination on the augmented matrix:

```math
[A \mid b].
```

Reduce it to row echelon form using row operations, then use back substitution.

If a contradictory row appears, the system has no solution. If free variables remain, choose values for them to obtain one solution vector. If every variable has a pivot, back substitution gives the unique solution.

Since there is only one right-hand side, computing the entire inverse would involve unnecessary work. Gaussian elimination acts directly on the required system.

If additional right-hand sides were later introduced, the elimination operations or an LU factorization, with pivoting if needed, could be reused.
