# Exercise 13. Does Every Equation Add New Information?

## Question

Consider the system

```math
\begin{cases}
x_1+x_2=10,\\
x_2+x_3=8,\\
x_1-x_3=2.
\end{cases}
```

Solve it and check whether all three equations are independently necessary to describe the solution set. If one follows from the others, show this by calculation.

## Solution

### 1. Identifying a redundant equation

Subtract the second equation from the first equation:

```math
(x_1+x_2)-(x_2+x_3)=10-8.
```

After simplifying, we obtain

```math
x_1-x_3=2.
```

This is exactly the third equation. Therefore, the third equation follows from the first two and adds no new restriction.

The first two equations are independent because neither is a scalar multiple of the other.

### 2. Confirming this by elimination

The augmented matrix is

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 0 & 10\\
0 & 1 & 1 & 8\\
1 & 0 & -1 & 2
\end{array}
\right).
```

Subtract the first row from the third row:

```math
R_3 \leftarrow R_3-R_1.
```

This gives

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 0 & 10\\
0 & 1 & 1 & 8\\
0 & -1 & -1 & -8
\end{array}
\right).
```

Now add the second row to the third row:

```math
R_3 \leftarrow R_3+R_2.
```

We obtain

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 0 & 10\\
0 & 1 & 1 & 8\\
0 & 0 & 0 & 0
\end{array}
\right).
```

The last row represents 0=0, confirming that the third equation is redundant.

### 3. Finding all solutions

There are two pivots and three unknowns, so there is one free variable.

Let

```math
x_3=t,
\qquad
t\in\mathbb{R}.
```

From the second equation,

```math
x_2+x_3=8,
```

we obtain

```math
x_2=8-t.
```

Using the first equation,

```math
x_1+x_2=10,
```

gives

```math
x_1=10-(8-t)=2+t.
```

Therefore, all solutions are

```math
\boxed{
(x_1,x_2,x_3)=(2+t,8-t,t),
\qquad t\in\mathbb{R}
}.
```

Equivalently,

```math
\begin{pmatrix}
x_1\\
x_2\\
x_3
\end{pmatrix}
=
\begin{pmatrix}
2\\
8\\
0
\end{pmatrix}
+
t
\begin{pmatrix}
1\\
-1\\
1
\end{pmatrix},
\qquad t\in\mathbb{R}.
```

### 4. Checking the solution

For the first equation:

```math
(2+t)+(8-t)=10.
```

For the second equation:

```math
(8-t)+t=8.
```

For the third equation:

```math
(2+t)-t=2.
```

All three equations hold for every real t. Thus, the system has infinitely many solutions, and only two independent equations are needed to describe its solution set.
