# Exercise 1. From a System to a Matrix

## Question

Write the system

```math
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7
\end{cases}
```

in the form Ax = b. Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

## Solution

### 1. The Coefficient Matrix

We use the variable order x, y, z. Each row contains the coefficients of these variables in the corresponding equation.

Therefore, the coefficient matrix is:

```math
A =
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{pmatrix}.
```

### 2. The Vector of Unknowns

The unknowns are written as a column vector in the same order:

```math
\mathbf{x} =
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}.
```

Here, the bold symbol represents the whole vector, while x is its first component.

### 3. The Right-Hand Side Vector

The constants on the right-hand sides form another column vector:

```math
b =
\begin{pmatrix}
4 \\
1 \\
7
\end{pmatrix}.
```

### 4. Writing the Matrix Equation

The system becomes:

```math
A\mathbf{x}=b,
```

or explicitly:

```math
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
=
\begin{pmatrix}
4 \\
1 \\
7
\end{pmatrix}.
```

### 5. How the Rows Represent the Equations

Multiplying each row of A by the vector of unknowns gives:

```math
A\mathbf{x} =
\begin{pmatrix}
2x-y+z \\
x+3y-2z \\
3x+y+z
\end{pmatrix}.
```

The first row produces the first equation, the second row produces the second equation, and the third row produces the third equation.

Equating the entries of this column vector to those of b reproduces the original system.
