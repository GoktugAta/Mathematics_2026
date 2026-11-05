# Exercise 3. Swapping Two Rows

## Question

For

```math
A =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix},
```

compute det(A). Then form a matrix B by swapping the first and second rows of A.

First predict det(B) using a determinant property, and then verify your prediction by calculation.

## Solution

### 1. Computing det(A)

Expanding along the first row:

```math
\det(A)=
1\begin{vmatrix}
3 & 1 \\
1 & 1
\end{vmatrix}
-
2\begin{vmatrix}
0 & 1 \\
2 & 1
\end{vmatrix}
=1(3-1)-2(0-2)=6.
```

### 2. Forming B and Predicting Its Determinant

Swapping the first two rows gives:

```math
B =
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1
\end{pmatrix}.
```

A single row swap reverses the sign of the determinant. Therefore:

```math
\det(B)=-\det(A)=-6.
```

### 3. Verification by Calculation

Expanding B along its first row:

```math
\det(B)=
-3\begin{vmatrix}
1 & 0 \\
2 & 1
\end{vmatrix}
+
\begin{vmatrix}
1 & 2 \\
2 & 1
\end{vmatrix}
=-3(1-0)+(1-4)=-6.
```

The calculation confirms the predicted sign change.
