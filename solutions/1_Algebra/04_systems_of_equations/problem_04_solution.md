# Exercise 4. Infinitely Many Solutions

## Question

Solve

```math
\begin{cases}
x+y+z=2,\\
2x+2y+2z=4,\\
x-y+z=0.
\end{cases}
```

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

## Solution

### 1. Writing the augmented matrix

The augmented matrix is

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 2\\
2 & 2 & 2 & 4\\
1 & -1 & 1 & 0
\end{array}
\right).
```

The second equation is twice the first equation, so it provides no additional restriction.

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
1 & 1 & 1 & 2\\
0 & 0 & 0 & 0\\
0 & -2 & 0 & -2
\end{array}
\right).
```

Interchange the second and third rows:

```math
R_2 \leftrightarrow R_3.
```

We obtain

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 2\\
0 & -2 & 0 & -2\\
0 & 0 & 0 & 0
\end{array}
\right).
```

Divide the second row by -2:

```math
R_2 \leftarrow -\frac{1}{2}R_2.
```

Then subtract the second row from the first row:

```math
R_1 \leftarrow R_1-R_2.
```

The resulting matrix is

```math
\left(
\begin{array}{ccc|c}
1 & 0 & 1 & 1\\
0 & 1 & 0 & 1\\
0 & 0 & 0 & 0
\end{array}
\right).
```

Therefore, the original system is equivalent to

```math
\begin{cases}
x+z=1,\\
y=1.
\end{cases}
```

The zero row represents 0=0, so there is no contradiction.

### 3. Identifying the free variable

The pivot columns correspond to x and y. The column corresponding to z has no pivot, so z is a free variable.

Let

```math
z=t,
\qquad
t\in\mathbb{R}.
```

Then x+z=1 gives

```math
x=1-t.
```

Also, y=1. Hence, all solutions are

```math
\boxed{
(x,y,z)=(1-t,1,t),
\qquad t\in\mathbb{R}
}.
```

Equivalently, in vector form:

```math
\begin{pmatrix}
x\\
y\\
z
\end{pmatrix}
=
\begin{pmatrix}
1\\
1\\
0
\end{pmatrix}
+
t
\begin{pmatrix}
-1\\
0\\
1
\end{pmatrix},
\qquad t\in\mathbb{R}.
```

The system is consistent and has one free variable. Therefore, it has infinitely many solutions.

### 4. Checking one chosen parameter value

Choose t=2. The corresponding point is

```math
(x,y,z)=(-1,1,2).
```

Substitute this point into each original equation.

First equation:

```math
x+y+z=-1+1+2=2.
```

Second equation:

```math
2x+2y+2z=2(-1)+2(1)+2(2)=-2+2+4=4.
```

Third equation:

```math
x-y+z=-1-1+2=0.
```

All three equations are satisfied, so the chosen point is a solution of the original system.
