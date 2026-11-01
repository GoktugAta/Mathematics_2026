# Problem 14 Solution

### 1. Condition for Exactly One Solution

The system Ax = b has exactly one solution for every b if and only if A is invertible.

```math
A =
\begin{pmatrix}
1 & 2 \\
k & 4
\end{pmatrix},
\qquad
\det(A)=4-2k.
```

Therefore:

```math
4-2k \neq 0
\quad\Longleftrightarrow\quad
\boxed{k \neq 2}.
```

### 2. The Exceptional Case: k = 2

When k = 2:

```math
A =
\begin{pmatrix}
1 & 2 \\
2 & 4
\end{pmatrix}.
```

The second row is twice the first. Writing the system explicitly:

```math
\begin{cases}
x_1+2x_2=b_1, \\
2x_1+4x_2=b_2.
\end{cases}
```

The equations are consistent exactly when:

```math
b_2=2b_1.
```

### 3. Example with Infinitely Many Solutions

Choose:

```math
b =
\begin{pmatrix}
1 \\
2
\end{pmatrix}.
```

The second equation is twice the first, so both reduce to:

```math
x_1+2x_2=1.
```

Letting x₂ = s gives infinitely many solutions:

```math
x =
\begin{pmatrix}
1-2s \\
s
\end{pmatrix},
\qquad s \in \mathbb{R}.
```

### 4. Example with No Solution

Choose:

```math
b =
\begin{pmatrix}
1 \\
3
\end{pmatrix}.
```

The system becomes:

```math
\begin{cases}
x_1+2x_2=1, \\
2x_1+4x_2=3.
\end{cases}
```

Twice the first equation gives a right-hand side of 2, but the second equation requires 3. Subtracting twice the first equation from the second gives:

```math
0=1.
```

Therefore, this system has no solution.
