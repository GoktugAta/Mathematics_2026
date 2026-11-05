# Exercise 2. Determinant of a 3 × 3 Matrix

## Question

For

```math
A =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5
\end{pmatrix},
```

compute det(A) using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

## Solution

### 1. Applying Sarrus' Rule

The sum of the downward diagonal products is:

```math
1\cdot3\cdot5+2\cdot4\cdot2+(-1)\cdot0\cdot1
=15+16+0=31.
```

The sum of the upward diagonal products is:

```math
(-1)\cdot3\cdot2+2\cdot0\cdot5+1\cdot4\cdot1
=-6+0+4=-2.
```

Subtracting the second sum from the first gives:

```math
\det(A)=31-(-2)=33.
```

### 2. Checking with Row Operations

Adding a multiple of one row to another preserves the determinant. Apply:

```math
R_3\leftarrow R_3-2R_1.
```

This gives:

```math
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7
\end{pmatrix}.
```

Then apply:

```math
R_3\leftarrow R_3+R_2.
```

The resulting matrix is upper triangular:

```math
U =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & 0 & 11
\end{pmatrix}.
```

Its determinant is the product of its diagonal entries:

```math
\det(A)=\det(U)=1\cdot3\cdot11=33.
```

This confirms the Sarrus calculation.
