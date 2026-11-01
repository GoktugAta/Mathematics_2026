# Problem 9 Solution

### 1. Computing the Area

Place the vectors as columns of a matrix:

```math
M =
\begin{pmatrix}
3 & 1 \\
1 & 4
\end{pmatrix}
```

The area of the parallelogram is the absolute value of the determinant:

```math
\det(M)=3\cdot4-1\cdot1=12-1=11.
```

```math
\text{Area}=|\det(M)|=|11|=\boxed{11}
```

The area is 11 square units.

### 2. Reversing the Order of the Vectors

Swapping the columns gives:

```math
N =
\begin{pmatrix}
1 & 3 \\
4 & 1
\end{pmatrix}
```

```math
\det(N)=1\cdot1-3\cdot4=1-12=-11.
```

Swapping two columns reverses the sign of the determinant, reflecting a reversal of orientation. However, its absolute value remains unchanged:

```math
\text{Area}=|\det(N)|=|-11|=\boxed{11}.
```

Thus, the determinant changes sign, but the parallelogram and its area remain unchanged.
