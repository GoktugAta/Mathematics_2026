# Exercise 2. Gaussian Elimination — One Solution

## Question

Solve using Gaussian elimination:

```math
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
```

After solving, substitute the result into all equations and check consistency.

## Solution

### 1. Forming the Augmented Matrix

Using the variable order x, y, z:

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
2 & -1 & 1 & 3 \\
1 & 2 & -1 & 2
\end{array}
\right).
```

### 2. Eliminating x from Rows 2 and 3

Apply:

```math
R_2\leftarrow R_2-2R_1,
\qquad
R_3\leftarrow R_3-R_1.
```

These operations preserve the solution set and give:

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & -3 & -1 & -9 \\
0 & 1 & -2 & -4
\end{array}
\right).
```

### 3. Choosing a Simpler Second Pivot

Swap the second and third rows to use the pivot 1:

```math
R_2\leftrightarrow R_3.
```

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & -3 & -1 & -9
\end{array}
\right).
```

### 4. Eliminating y from Row 3

Apply:

```math
R_3\leftarrow R_3+3R_2.
```

This gives the upper triangular system:

```math
\left(
\begin{array}{ccc|c}
1 & 1 & 1 & 6 \\
0 & 1 & -2 & -4 \\
0 & 0 & -7 & -21
\end{array}
\right).
```

### 5. Back Substitution

The third row gives:

```math
-7z=-21
\quad\Longrightarrow\quad
z=3.
```

The second row gives:

```math
y-2z=-4
\quad\Longrightarrow\quad
y-6=-4
\quad\Longrightarrow\quad
y=2.
```

The first row gives:

```math
x+y+z=6
\quad\Longrightarrow\quad
x+2+3=6
\quad\Longrightarrow\quad
x=1.
```

Therefore:

```math
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
=
\begin{pmatrix}
1 \\
2 \\
3
\end{pmatrix}.
```

There is a pivot for every variable and no free variable, so the solution is unique.

### 6. Checking All Original Equations

Substitute x = 1, y = 2, and z = 3.

First equation:

```math
x+y+z=1+2+3=6.
```

Second equation:

```math
2x-y+z=2(1)-2+3=3.
```

Third equation:

```math
x+2y-z=1+2(2)-3=2.
```

All three equations are satisfied, confirming that the system is consistent and the solution is correct.
