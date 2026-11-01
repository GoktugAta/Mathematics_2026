# Problem 6 Solution

### 1. Computing the Determinant

```math
A(t) =
\begin{pmatrix}
t & 1 \\
2 & t
\end{pmatrix}
```

```math
\det(A(t)) = t \cdot t - 1 \cdot 2 = t^2-2.
```

### 2. Finding When the Matrix Is Not Invertible

A square matrix is not invertible if and only if its determinant is zero:

```math
t^2-2=0
\quad\Longrightarrow\quad
t^2=2
\quad\Longrightarrow\quad
t=\pm\sqrt{2}.
```

Therefore, A(t) is not invertible exactly when:

```math
\boxed{t=\sqrt{2}\ \text{or}\ t=-\sqrt{2}}.
```

For all other real values of t, the determinant is nonzero, so A(t) is invertible.
