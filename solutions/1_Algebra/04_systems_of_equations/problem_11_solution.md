# Exercise 11. A Parameter in a System of Three Equations

## Question

Analyze the number of solutions depending on t:

```math
\begin{cases}
x+y+z=1,\\
x+ty+z=2,\\
x+y+tz=3.
\end{cases}
```

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

## Solution

### 1. Performing elimination

The augmented matrix is

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 1\\
1 & t & 1 & 2\\
1 & 1 & t & 3
\end{array}
\right).
```

Subtract the first row from the second and third rows:

```math
R_2 \leftarrow R_2-R_1,
\qquad
R_3 \leftarrow R_3-R_1.
```

This gives

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 1\\
0 & t-1 & 0 & 1\\
0 & 0 & t-1 & 2
\end{array}
\right).
```

The corresponding equations are

```math
\begin{cases}
x+y+z=1,\\
(t-1)y=1,\\
(t-1)z=2.
\end{cases}
```

These row operations are valid for every t. However, division by t-1 is valid only when t is not 1, so we must consider two cases.

### 2. Case t is not 1

Since t-1 is nonzero, the last two equations give

```math
y=\frac{1}{t-1},
\qquad
z=\frac{2}{t-1}.
```

Using the first equation:

```math
x=1-y-z.
```

Therefore,

```math
x
=1-\frac{1}{t-1}-\frac{2}{t-1}
=1-\frac{3}{t-1}
=\frac{t-4}{t-1}.
```

Thus, for every t different from 1, the unique solution is

```math
\boxed{
(x,y,z)=
\left(
\frac{t-4}{t-1},
\frac{1}{t-1},
\frac{2}{t-1}
\right)
}.
```

There are three pivots and no free variables, so exactly one solution exists.

### 3. Checking the solution for t different from 1

For the first equation:

```math
x+y+z
=\frac{t-4+1+2}{t-1}
=\frac{t-1}{t-1}
=1.
```

For the second equation:

```math
x+ty+z
=\frac{t-4+t+2}{t-1}
=\frac{2t-2}{t-1}
=2.
```

For the third equation:

```math
x+y+tz
=\frac{t-4+1+2t}{t-1}
=\frac{3t-3}{t-1}
=3.
```

All three equations are satisfied.

### 4. Case t equals 1

We must analyze this value without dividing by t-1.

Substituting t=1 into the eliminated matrix gives

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 1\\
0 & 0 & 0 & 1\\
0 & 0 & 0 & 2
\end{array}
\right).
```

The second and third rows represent

```math
0=1,
\qquad
0=2.
```

These are contradictions. Therefore, the system has no solution when t=1.

This is also visible in the original system: the same expression x+y+z would have to equal 1, 2, and 3 simultaneously.

### 5. Classification

| Parameter value | Number of solutions |
|---|---|
| t different from 1 | Exactly one solution |
| t = 1 | No solution |

There is no parameter value giving infinitely many solutions. When the last two pivots vanish, the right-hand sides remain nonzero, producing contradictions rather than free variables.
