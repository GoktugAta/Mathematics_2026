# Exercise 14. A System of Equations and the Determinant

## Question

Consider the system Ax = b, where:

```math
A =
\begin{pmatrix}
1 & 2 \\
k & 4
\end{pmatrix}.
```

For which values of k does the system have exactly one solution for every b? For the remaining value, give an example of a right-hand side b for which the system has infinitely many solutions, and an example for which it has no solution.

## Solution

### 1. Condition for a Unique Solution

The system has exactly one solution for every b if and only if A is invertible.

```math
\det(A)=1\cdot4-2k=4-2k.
```

Thus:

```math
\det(A)\neq0
\quad\Longleftrightarrow\quad
k\neq2.
```

### 2. The Exceptional Value

When k = 2, the system is:

```math
\begin{cases}
x_1+2x_2=b_1, \\
2x_1+4x_2=b_2.
\end{cases}
```

The left side of the second equation is twice the left side of the first. Therefore, consistency requires b₂ = 2b₁.

### 3. Infinitely Many Solutions

Choose:

```math
b =
\begin{pmatrix}
1 \\
2
\end{pmatrix}.
```

Both equations reduce to x₁ + 2x₂ = 1. Setting x₂ = s gives:

```math
x =
\begin{pmatrix}
1-2s \\
s
\end{pmatrix},
\qquad s\in\mathbb{R}.
```

Hence, there are infinitely many solutions.

### 4. No Solution

Choose:

```math
b =
\begin{pmatrix}
1 \\
3
\end{pmatrix}.
```

The equations become:

```math
\begin{cases}
x_1+2x_2=1, \\
2x_1+4x_2=3.
\end{cases}
```

Subtracting twice the first equation from the second gives 0 = 1, a contradiction. Therefore, this system has no solution.
