# Exercise 12. Homogeneous System

## Question

Solve

```math
\begin{cases}
x+2y-z=0,\\
2x+4y-2z=0,\\
x-y+2z=0.
\end{cases}
```

Give all solutions in parametric form and explain why (0,0,0) always satisfies a homogeneous system.

## Solution

### 1. Writing the augmented matrix

The augmented matrix is

```math
\left(
\begin{array}{ccc|c}
1 & 2 & -1 & 0\\
2 & 4 & -2 & 0\\
1 & -1 & 2 & 0
\end{array}
\right).
```

The second equation is twice the first equation, so it does not provide an additional independent condition.

### 2. Performing elimination

Eliminate x from the second and third rows:

```math
R_2 \leftarrow R_2-2R_1,
\qquad
R_3 \leftarrow R_3-R_1.
```

This gives

```math
\left(
\begin{array}{ccc|c}
1 & 2 & -1 & 0\\
0 & 0 & 0 & 0\\
0 & -3 & 3 & 0
\end{array}
\right).
```

Move the zero row to the bottom:

```math
R_2 \leftrightarrow R_3.
```

We obtain

```math
\left(
\begin{array}{ccc|c}
1 & 2 & -1 & 0\\
0 & -3 & 3 & 0\\
0 & 0 & 0 & 0
\end{array}
\right).
```

Divide the second row by -3:

```math
R_2 \leftarrow -\frac{1}{3}R_2.
```

The matrix becomes

```math
\left(
\begin{array}{ccc|c}
1 & 2 & -1 & 0\\
0 & 1 & -1 & 0\\
0 & 0 & 0 & 0
\end{array}
\right).
```

Finally, eliminate y from the first row:

```math
R_1 \leftarrow R_1-2R_2.
```

This gives

```math
\left(
\begin{array}{ccc|c}
1 & 0 & 1 & 0\\
0 & 1 & -1 & 0\\
0 & 0 & 0 & 0
\end{array}
\right).
```

### 3. Writing all solutions in parametric form

The nonzero rows represent

```math
x+z=0,
\qquad
y-z=0.
```

There are two pivot variables, x and y, and one free variable, z.

Let

```math
z=s,
\qquad
s\in\mathbb{R}.
```

Then

```math
x=-s,
\qquad
y=s.
```

Therefore, all solutions are

```math
\boxed{(x,y,z)=(-s,s,s),\qquad s\in\mathbb{R}}.
```

Equivalently, in vector form:

```math
\begin{pmatrix}
x\\
y\\
z
\end{pmatrix}
=
s
\begin{pmatrix}
-1\\
1\\
1
\end{pmatrix},
\qquad
s\in\mathbb{R}.
```

Since s may be any real number, the system has infinitely many solutions.

### 4. Checking the parametric solution

Substituting x=-s, y=s, and z=s into the first equation gives

```math
-s+2s-s=0.
```

For the second equation:

```math
2(-s)+4s-2s=0.
```

For the third equation:

```math
-s-s+2s=0.
```

Thus, every value of s gives a solution.

### 5. Why the zero vector always satisfies a homogeneous system

A homogeneous linear system has zero on the right-hand side of every equation.

When all unknowns are zero, every term on the left-hand side is also zero. Therefore, every equation becomes 0=0.

In matrix notation:

```math
A\mathbf{0}=\mathbf{0}.
```

Hence, the zero vector always satisfies a homogeneous system. In our parametric solution, it corresponds to s=0.
