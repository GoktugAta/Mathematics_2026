# Exercise 6. A System with a Parameter — Which Cases Actually Occur?

## Question

Analyze, depending on the parameter a, the system:

```math
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
```

Among the three possibilities — exactly one solution, infinitely many solutions, no solution — determine which actually occur and for which values of a. If one type cannot occur, explain why.

## Solution

### 1. Elimination with the Parameter

The augmented matrix is:

```math
\left(
\begin{array}{cc|c}
1 & 1 & 2 \\
a & a & 4
\end{array}
\right).
```

Apply:

```math
R_2\leftarrow R_2-aR_1.
```

This operation is valid for every a and gives:

```math
\left(
\begin{array}{cc|c}
1 & 1 & 2 \\
0 & 0 & 4-2a
\end{array}
\right).
```

The second row represents:

```math
0=4-2a.
```

### 2. Infinitely Many Solutions

If a = 2, the last row becomes 0 = 0. The second equation is twice the first, so only one independent equation remains:

```math
x+y=2.
```

Choose y = t freely. Then:

```math
x=2-t.
```

Thus, all solutions are:

```math
\begin{pmatrix}
x \\
y
\end{pmatrix}
=
\begin{pmatrix}
2-t \\
t
\end{pmatrix},
\qquad t\in\mathbb{R}.
```

Therefore, there are infinitely many solutions when a = 2.

### 3. No Solution

If a ≠ 2, then 4 − 2a is nonzero. The last row states that zero equals a nonzero number, which is impossible.

Therefore, the system has no solution when a ≠ 2.

### 4. Why Exactly One Solution Cannot Occur

The second coefficient row is always a multiple of the first. Consequently, elimination never produces a second pivot.

If the system is consistent, one variable remains free. If it is inconsistent, there is no solution. A unique solution cannot occur for any value of a.

| Parameter | Number of solutions |
|---|---|
| a = 2 | Infinitely many |
| a ≠ 2 | None |
| No value of a | Exactly one |
