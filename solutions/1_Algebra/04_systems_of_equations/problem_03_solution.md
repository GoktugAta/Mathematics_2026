# Exercise 3. Inconsistent System

## Question

Solve or show that the system is inconsistent:

```math
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
```

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

## Solution

### 1. Forming the Augmented Matrix

Using the variable order x, y:

```math
\left(
\begin{array}{cc|c}
1 & 2 & 3 \\
2 & 4 & 7
\end{array}
\right).
```

### 2. Performing Elimination

Subtract twice the first row from the second:

```math
R_2\leftarrow R_2-2R_1.
```

This gives:

```math
\left(
\begin{array}{cc|c}
1 & 2 & 3 \\
0 & 0 & 1
\end{array}
\right).
```

### 3. Interpreting the Contradiction

The second row represents:

```math
0x+0y=1,
```

which means:

```math
0=1.
```

This is impossible for any values of x and y. Therefore, the system is inconsistent and has no solution.

The same contradiction follows directly from the equations: doubling the first equation gives 2x + 4y = 6, while the second equation requires 2x + 4y = 7. Both cannot hold simultaneously.
