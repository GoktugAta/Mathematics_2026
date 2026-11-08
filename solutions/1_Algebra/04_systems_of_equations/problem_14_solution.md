# Exercise 14. A Small Change in the Right-Hand Side

## Question

Compare the systems

```math
\begin{cases}
x+y=2,\\
2x-y=1,\\
3x=3
\end{cases}
```

and

```math
\begin{cases}
x+y=2,\\
2x-y=1,\\
3x=3.1.
\end{cases}
```

Check the consistency of each system and explain why a small change in one number can change the type of the system.

## Solution

### 1. Solving the two equations shared by both systems

The first two equations are

```math
\begin{cases}
x+y=2,\\
2x-y=1.
\end{cases}
```

Adding them eliminates y:

```math
(x+y)+(2x-y)=2+1.
```

Therefore,

```math
3x=3,
\qquad
x=1.
```

Substituting into the first equation gives

```math
1+y=2,
\qquad
y=1.
```

Thus, any solution of either full system must be

```math
(x,y)=(1,1).
```

### 2. Checking the first system

The third equation of the first system is

```math
3x=3.
```

Substituting x=1 gives

```math
3(1)=3.
```

Therefore, (1,1) satisfies all three equations.

The first system is consistent and has exactly one solution:

```math
\boxed{x=1,\qquad y=1}.
```

The third equation is the sum of the first two equations, so it adds no new restriction.

### 3. Checking the second system

The third equation of the second system is

```math
3x=3.1.
```

However, the first two equations require x=1. Substituting this value into the third equation gives

```math
3=3.1,
```

which is false.

Therefore, the second system is inconsistent:

```math
\boxed{\text{No solution}}.
```

### 4. Showing the difference in the augmented matrices

The coefficient row of the third equation is the sum of the first two coefficient rows:

```math
(3,0)=(1,1)+(2,-1).
```

We can therefore use the row operation

```math
R_3 \leftarrow R_3-R_1-R_2.
```

For the first system, this gives

```math
\left(
\begin{array}{cc|c}
1 & 1 & 2\\
2 & -1 & 1\\
0 & 0 & 0
\end{array}
\right).
```

The last row represents 0=0, so it creates no contradiction.

For the second system, the same operation gives

```math
\left(
\begin{array}{cc|c}
1 & 1 & 2\\
2 & -1 & 1\\
0 & 0 & 0.1
\end{array}
\right).
```

The last row represents

```math
0=0.1,
```

which is a contradiction.

### 5. Why the small change matters

The first two equations already determine a unique point, (1,1).

For the full system to be consistent, the third equation must also hold at this point. Its left-hand side is the sum of the first two left-hand sides, so its right-hand side must equal

```math
2+1=3.
```

Changing that number to 3.1 breaks this required equality. Although the numerical change is small, the equations require exact equality.

Therefore, the first system has one solution, while the second system has no solution.
