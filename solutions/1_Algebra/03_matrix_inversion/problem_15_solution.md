# Exercise 15. Two Methods for Solving the Same System

## Question

For

```math
A =
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix},
\qquad
b =
\begin{pmatrix}
7 \\
8
\end{pmatrix},
```

solve Ax = b in two ways:

1. Using A⁻¹b.
2. Using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## Solution

### 1. Solving with the Inverse

First compute the determinant:

```math
\det(A)=2\cdot3-1\cdot1=5.
```

Since it is nonzero, A is invertible. The inverse is:

```math
A^{-1} =
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}.
```

Now multiply by b:

```math
x=A^{-1}b
=
\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
7 \\
8
\end{pmatrix}
=
\frac15
\begin{pmatrix}
21-8 \\
-7+16
\end{pmatrix}
=
\begin{pmatrix}
\frac{13}{5} \\
\frac95
\end{pmatrix}.
```

### 2. Solving with Gaussian Elimination

Start with the augmented matrix:

```math
[A \mid b] =
\left(
\begin{array}{cc|c}
2 & 1 & 7 \\
1 & 3 & 8
\end{array}
\right).
```

Eliminate the first entry of the second row:

```math
R_2\leftarrow R_2-\frac12R_1.
```

This gives:

```math
\left(
\begin{array}{cc|c}
2 & 1 & 7 \\
0 & \frac52 & \frac92
\end{array}
\right).
```

The second equation gives:

```math
\frac52x_2=\frac92
\quad\Longrightarrow\quad
x_2=\frac95.
```

Substitute into the first equation:

```math
2x_1+\frac95=7
\quad\Longrightarrow\quad
2x_1=\frac{26}{5}
\quad\Longrightarrow\quad
x_1=\frac{13}{5}.
```

Thus:

```math
x =
\begin{pmatrix}
\frac{13}{5} \\
\frac95
\end{pmatrix}.
```

### 3. Checking the Solution

```math
Ax =
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{13}{5} \\
\frac95
\end{pmatrix}
=
\begin{pmatrix}
\frac{26}{5}+\frac95 \\
\frac{13}{5}+\frac{27}{5}
\end{pmatrix}
=
\begin{pmatrix}
7 \\
8
\end{pmatrix}
=b.
```

### 4. Comparing the Methods

Both methods give the same solution.

Counting the main stages, the inverse method has three: calculate the determinant, construct A⁻¹, and multiply A⁻¹ by b.

Gaussian elimination also has three main stages here: perform one row elimination, solve for x₂, and substitute to find x₁. These stages are not equal-cost arithmetic operations.

For this single right-hand side, Gaussian elimination is simpler because it finds the required solution directly without computing an entire inverse. If the inverse were already known, the inverse method would be convenient.
