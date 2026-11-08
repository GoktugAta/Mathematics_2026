# Exercise 5. Row Echelon Form and Number of Solutions

## Question

For the augmented matrix

```math
\left(
\begin{array}{ccc|c}
1 & 2 & -1 & 3 \\
0 & 1 & 2 & 1 \\
0 & 0 & 0 & 0
\end{array}
\right),
```

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

## Solution

### 1. Reading the Equations

Using the variable order x, y, z, the rows represent:

```math
\begin{cases}
x+2y-z=3, \\
y+2z=1, \\
0=0.
\end{cases}
```

The last row is always true and imposes no additional condition. There is no contradictory equation, so the system is consistent.

### 2. Identifying the Free Variable

There are pivots in the x and y columns, but no pivot in the z column.

Since there are three variables and two pivots, there is one free variable. Choose:

```math
z=t,\qquad t\in\mathbb{R}.
```

### 3. Finding the Other Variables

From the second equation:

```math
y+2z=1
\quad\Longrightarrow\quad
y=1-2t.
```

Substitute into the first equation:

```math
x+2(1-2t)-t=3.
```

Simplifying gives:

```math
x+2-5t=3
\quad\Longrightarrow\quad
x=1+5t.
```

### 4. Parametric Form and Number of Solutions

All solutions are:

```math
\begin{cases}
x=1+5t, \\
y=1-2t, \\
z=t,
\end{cases}
\qquad t\in\mathbb{R}.
```

Equivalently, in vector form:

```math
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
=
\begin{pmatrix}
1 \\
1 \\
0
\end{pmatrix}
+
t\begin{pmatrix}
5 \\
-2 \\
1
\end{pmatrix},
\qquad t\in\mathbb{R}.
```

The system has infinitely many solutions because the free parameter t can take any real value.

### 5. Verification

Substituting the parametric expressions gives:

```math
x+2y-z
=(1+5t)+2(1-2t)-t
=3,
```

```math
y+2z=(1-2t)+2t=1.
```

Both equations hold for every real t, confirming the solution set.
