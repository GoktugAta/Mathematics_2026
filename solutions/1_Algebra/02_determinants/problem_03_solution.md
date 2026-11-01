# Problem 3 Solution

### 1. Computing det(A)

```math
A =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix}
```

Expanding along the first row:

```math
\det(A) =
1\begin{vmatrix}
3 & 1 \\
1 & 1
\end{vmatrix}
-
2\begin{vmatrix}
0 & 1 \\
2 & 1
\end{vmatrix}
```

```math
\det(A) = 1(3-1)-2(0-2)
= 2+4
= 6.
```

### 2. Forming B and Predicting det(B)

Swapping the first and second rows gives:

```math
B =
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1
\end{pmatrix}
```

Swapping two rows changes the sign of the determinant. Therefore, we predict:

```math
\det(B) = -\det(A) = -6.
```

### 3. Verification by Calculation

Expanding B along the first row:

```math
\det(B) =
-3\begin{vmatrix}
1 & 0 \\
2 & 1
\end{vmatrix}
+
1\begin{vmatrix}
1 & 2 \\
2 & 1
\end{vmatrix}
```

```math
\det(B) = -3(1-0)+(1-4)
= -3-3
= -6.
```

The calculation confirms the prediction:

```math
\det(B) = -6 = -\det(A).
```
