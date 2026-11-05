# Exercise 7. Using Properties Instead of Recomputing

## Question

Suppose that for a 3 × 3 matrix A:

```math
\det(A)=-4.
```

Compute:

```math
\det(2A),\qquad
\det(A^T),\qquad
\det(A^2),\qquad
\det(-A).
```

Justify each answer using the appropriate property.

## Solution

### 1. Computing det(2A)

For an n × n matrix, scaling the entire matrix by k multiplies its determinant by kⁿ. Since A is 3 × 3:

```math
\det(2A)=2^3\det(A)=8(-4)=-32.
```

### 2. Computing det(Aᵀ)

Transposing a matrix leaves its determinant unchanged:

```math
\det(A^T)=\det(A)=-4.
```

### 3. Computing det(A²)

The determinant of a product is the product of the determinants:

```math
\det(A^2)=\det(A)\det(A)=(-4)^2=16.
```

### 4. Computing det(−A)

Applying the scaling property with k = −1 gives:

```math
\det(-A)=(-1)^3\det(A)=(-1)(-4)=4.
```
