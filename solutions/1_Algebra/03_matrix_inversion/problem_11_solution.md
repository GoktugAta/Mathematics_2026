# Exercise 11. Parameter and Invertibility

## Question

For

```math
A(t) =
\begin{pmatrix}
1 & t \\
t & 1
\end{pmatrix},
```

find all t for which the matrix is invertible, and then give a formula for A(t)⁻¹. Explain what happens to this formula at the excluded values.

## Solution

### 1. Finding the Invertible Cases

The determinant is:

```math
\det(A(t))=1\cdot1-t\cdot t=1-t^2.
```

The matrix is invertible exactly when this determinant is nonzero:

```math
1-t^2\neq0
\quad\Longleftrightarrow\quad
t\neq1\ \text{and}\ t\neq-1.
```

### 2. Formula for the Inverse

Applying the 2 × 2 inverse formula gives:

```math
A(t)^{-1} =
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix},
\qquad t\neq\pm1.
```

Indeed:

```math
A(t)A(t)^{-1} =
\frac{1}{1-t^2}
\begin{pmatrix}
1 & t \\
t & 1
\end{pmatrix}
\begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix}
=
\frac{1}{1-t^2}
\begin{pmatrix}
1-t^2 & 0 \\
0 & 1-t^2
\end{pmatrix}
=I.
```

### 3. What Happens at the Excluded Values?

At t = 1 or t = −1, the denominator 1 − t² is zero, so the inverse formula is undefined.

At t = 1:

```math
A(1) =
\begin{pmatrix}
1 & 1 \\
1 & 1
\end{pmatrix}.
```

The rows are equal.

At t = −1:

```math
A(-1) =
\begin{pmatrix}
1 & -1 \\
-1 & 1
\end{pmatrix}.
```

The second row is the negative of the first.

In both cases, the rows are linearly dependent and the determinant is zero. Therefore, no inverse exists at these values.
