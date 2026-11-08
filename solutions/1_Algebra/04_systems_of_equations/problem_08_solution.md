# Exercise 8. Two Systems with the Same Coefficient Matrix

## Question

Solve by elimination the two systems

```math
\begin{cases}
2x+y=5,\\
x-y=1,
\end{cases}
```

and

```math
\begin{cases}
2x+y=1,\\
x-y=4.
\end{cases}
```

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

## Solution

### 1. Solving the first system

The augmented matrix is

```math
\left(
\begin{array}{cc|c}
2 & 1 & 5\\
1 & -1 & 1
\end{array}
\right).
```

We first interchange the rows to obtain a leading coefficient of 1:

```math
R_1 \leftrightarrow R_2.
```

This gives

```math
\left(
\begin{array}{cc|c}
1 & -1 & 1\\
2 & 1 & 5
\end{array}
\right).
```

To eliminate x from the second equation, subtract twice the first row from the second row:

```math
R_2 \leftarrow R_2-2R_1.
```

We obtain

```math
\left(
\begin{array}{cc|c}
1 & -1 & 1\\
0 & 3 & 3
\end{array}
\right).
```

The second row gives

```math
3y=3,
\qquad
y=1.
```

Substituting into the first equation gives

```math
x-y=1,
\qquad
x=1+y=2.
```

Therefore, the first system has the solution

```math
\boxed{x=2,\qquad y=1}.
```

Checking both original equations:

```math
2(2)+1=5,
```

```math
2-1=1.
```

Both equations are satisfied.

### 2. Solving the second system

The augmented matrix is

```math
\left(
\begin{array}{cc|c}
2 & 1 & 1\\
1 & -1 & 4
\end{array}
\right).
```

We use exactly the same row operations. First, interchange the rows:

```math
R_1 \leftrightarrow R_2.
```

This gives

```math
\left(
\begin{array}{cc|c}
1 & -1 & 4\\
2 & 1 & 1
\end{array}
\right).
```

Next, eliminate x from the second row:

```math
R_2 \leftarrow R_2-2R_1.
```

We obtain

```math
\left(
\begin{array}{cc|c}
1 & -1 & 4\\
0 & 3 & -7
\end{array}
\right).
```

The second row gives

```math
3y=-7,
\qquad
y=-\frac{7}{3}.
```

Substituting into the first equation gives

```math
x-y=4,
```

```math
x=4+y
=4-\frac{7}{3}
=\frac{5}{3}.
```

Therefore, the second system has the solution

```math
\boxed{x=\frac{5}{3},\qquad y=-\frac{7}{3}}.
```

Checking both original equations:

```math
2\left(\frac{5}{3}\right)-\frac{7}{3}
=\frac{10-7}{3}
=1,
```

```math
\frac{5}{3}-\left(-\frac{7}{3}\right)
=\frac{12}{3}
=4.
```

Both equations are satisfied.

### 3. Comparing the elimination steps

Both systems have the same coefficient matrix:

```math
A=
\begin{pmatrix}
2 & 1\\
1 & -1
\end{pmatrix}.
```

Therefore, the same row operations eliminate the same coefficient:

```math
R_1 \leftrightarrow R_2,
\qquad
R_2 \leftarrow R_2-2R_1.
```

In both cases, the coefficient matrix becomes

```math
\begin{pmatrix}
1 & -1\\
0 & 3
\end{pmatrix}.
```

The row operations and elimination multiplier are identical because they depend on the coefficients of x and y.

Only the right-hand-side calculations differ:

```math
5-2(1)=3
```

for the first system, and

```math
1-2(4)=-7
```

for the second system.

Thus, the elimination operations can be reused for different right-hand-side vectors, but the resulting solutions may be different.
