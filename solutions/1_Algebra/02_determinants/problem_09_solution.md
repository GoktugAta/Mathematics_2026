# Exercise 9. Area and the Determinant

## Question

The vectors

```math
u =
\begin{pmatrix}
3 \\
1
\end{pmatrix},
\qquad
v =
\begin{pmatrix}
1 \\
4
\end{pmatrix}
```

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

## Solution

### 1. Computing the Area

Place u and v as the columns of a matrix:

```math
M =
\begin{pmatrix}
3 & 1 \\
1 & 4
\end{pmatrix}.
```

Its determinant is:

```math
\det(M)=3\cdot4-1\cdot1=11.
```

The area is the absolute value of this determinant:

```math
\text{Area}=|\det(M)|=11.
```

Thus, the parallelogram has area 11 square units.

### 2. Reversing the Vector Order

Reversing the order swaps the columns:

```math
N =
\begin{pmatrix}
1 & 3 \\
4 & 1
\end{pmatrix}.
```

Then:

```math
\det(N)=1\cdot1-3\cdot4=-11.
```

Swapping the columns reverses orientation and changes the sign of the determinant. However:

```math
|\det(N)|=|-11|=11.
```

The parallelogram and its area remain unchanged.
