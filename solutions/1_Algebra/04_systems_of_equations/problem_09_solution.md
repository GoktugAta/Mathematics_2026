# Exercise 9. A System from a Sum Condition

## Question

Find numbers x and y satisfying

```math
x+y=10,
\qquad
2x+5y=32.
```

Solve the system and explain geometrically why the solution is unique.

## Solution

### 1. Solving the system

We write the augmented matrix:

```math
\left(
\begin{array}{cc|c}
1 & 1 & 10\\
2 & 5 & 32
\end{array}
\right).
```

To eliminate x from the second equation, subtract twice the first row from the second row:

```math
R_2 \leftarrow R_2-2R_1.
```

This gives

```math
\left(
\begin{array}{cc|c}
1 & 1 & 10\\
0 & 3 & 12
\end{array}
\right).
```

The second row represents

```math
3y=12.
```

Therefore,

```math
y=4.
```

Substituting into the first equation gives

```math
x+4=10,
```

so

```math
x=6.
```

The solution is

```math
\boxed{x=6,\qquad y=4}.
```

### 2. Checking the solution

For the first equation:

```math
6+4=10.
```

For the second equation:

```math
2(6)+5(4)=12+20=32.
```

Both conditions are satisfied.

### 3. Geometric explanation of uniqueness

Each equation describes a straight line in the xy-plane.

Writing the first equation in slope-intercept form gives

```math
y=10-x.
```

Its slope is -1.

Writing the second equation in slope-intercept form gives

```math
y=\frac{32}{5}-\frac{2}{5}x.
```

Its slope is -2/5.

Since the slopes are different, the two lines intersect at exactly one point. That point is

```math
(6,4).
```

Therefore, the system has exactly one solution.
