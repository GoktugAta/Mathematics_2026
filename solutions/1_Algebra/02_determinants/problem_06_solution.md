# Exercise 6. Parameter and Invertibility

## Question

For

```math
A(t) =
\begin{pmatrix}
t & 1 \\
2 & t
\end{pmatrix},
```

find all values of t for which the matrix is not invertible. Explain how your answer is related to the determinant being zero.

## Solution

The determinant is:

```math
\det(A(t))=t\cdot t-1\cdot2=t^2-2.
```

A square matrix is not invertible exactly when its determinant is zero. Therefore, solve:

```math
t^2-2=0
\quad\Longrightarrow\quad
t^2=2
\quad\Longrightarrow\quad
t=\pm\sqrt2.
```

Thus, A(t) is not invertible for:

```math
t=\sqrt2
\qquad\text{or}\qquad
t=-\sqrt2.
```

For every other real value of t, the determinant is nonzero and the matrix is invertible.
