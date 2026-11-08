# Exercise 10. A Polynomial Through Three Points

## Question

Find a polynomial

```math
p(x)=ax^2+bx+c
```

whose graph passes through (0,1), (1,3), and (2,9). Reduce the problem to a system of equations and check the result by substituting all three points.

## Solution

### 1. Forming a system of equations

A point lies on the graph when its coordinates satisfy y=p(x).

Substituting the point (0,1) gives

```math
a(0)^2+b(0)+c=1,
```

so c=1.

Substituting the point (1,3) gives

```math
a+b+c=3.
```

Substituting the point (2,9) gives

```math
4a+2b+c=9.
```

Therefore, the coefficients must satisfy the linear system

```math
\begin{cases}
c=1,\\
a+b+c=3,\\
4a+2b+c=9.
\end{cases}
```

The unknowns are a, b, and c. The system is linear in these unknown coefficients.

### 2. Solving for the coefficients

Using c=1 in the last two equations gives

```math
\begin{cases}
a+b=2,\\
4a+2b=8.
\end{cases}
```

Subtract twice the first equation from the second equation:

```math
(4a+2b)-2(a+b)=8-2(2).
```

Thus,

```math
2a=4,
\qquad
a=2.
```

Substituting into a+b=2 gives

```math
2+b=2,
\qquad
b=0.
```

Since c=1, the required polynomial is

```math
\boxed{p(x)=2x^2+1}.
```

### 3. Checking all three points

For (0,1):

```math
p(0)=2(0)^2+1=1.
```

For (1,3):

```math
p(1)=2(1)^2+1=3.
```

For (2,9):

```math
p(2)=2(2)^2+1=8+1=9.
```

Therefore, the graph passes through all three given points.
