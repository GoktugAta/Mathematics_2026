# Exercise 15. Classifying Three Systems

## Question

For each of the following systems, perform only as much elimination as necessary to recognize its type:

### System 1

```math
\begin{cases}
x+y=2,\\
x-y=0.
\end{cases}
```

### System 2

```math
\begin{cases}
x+y=2,\\
2x+2y=4.
\end{cases}
```

### System 3

```math
\begin{cases}
x+y=2,\\
2x+2y=5.
\end{cases}
```

For each, justify the classification: one solution, infinitely many solutions, or no solution.

## Solution

### 1. System 1: One solution

The augmented matrix is

```math
\left(
\begin{array}{cc|c}
1 & 1 & 2\\
1 & -1 & 0
\end{array}
\right).
```

Subtract the first row from the second row:

```math
R_2 \leftarrow R_2-R_1.
```

We obtain

```math
\left(
\begin{array}{cc|c}
1 & 1 & 2\\
0 & -2 & -2
\end{array}
\right).
```

There is a pivot in each variable column and no contradictory row. Therefore, both variables are determined uniquely.

The system has exactly one solution. No further elimination is needed to classify it.

### 2. System 2: Infinitely many solutions

The augmented matrix is

```math
\left(
\begin{array}{cc|c}
1 & 1 & 2\\
2 & 2 & 4
\end{array}
\right).
```

Subtract twice the first row from the second row:

```math
R_2 \leftarrow R_2-2R_1.
```

We obtain

```math
\left(
\begin{array}{cc|c}
1 & 1 & 2\\
0 & 0 & 0
\end{array}
\right).
```

The second row represents 0=0, so it imposes no additional condition.

The system is consistent and has only one pivot for two unknowns. Therefore, one variable is free, giving infinitely many solutions.

The second original equation is exactly twice the first, so both equations describe the same line.

### 3. System 3: No solution

The augmented matrix is

```math
\left(
\begin{array}{cc|c}
1 & 1 & 2\\
2 & 2 & 5
\end{array}
\right).
```

Subtract twice the first row from the second row:

```math
R_2 \leftarrow R_2-2R_1.
```

We obtain

```math
\left(
\begin{array}{cc|c}
1 & 1 & 2\\
0 & 0 & 1
\end{array}
\right).
```

The second row represents

```math
0x+0y=1,
```

or 0=1, which is impossible.

Therefore, the system is inconsistent and has no solution. We stop as soon as this contradiction appears.

### 4. Classification summary

| System | Result after elimination | Classification |
|---|---|---|
| 1 | Two pivots, no contradiction | Exactly one solution |
| 2 | One pivot, one free variable, no contradiction | Infinitely many solutions |
| 3 | A row representing 0=1 | No solution |
