# Exercise 15. Combining Determinant Properties

## Question

Let A and B be invertible 2 × 2 matrices with:

```math
\det(A)=-2,
\qquad
\det(B)=3.
```

Without finding the entries of the matrices, compute:

```math
\det(B^{-1}A^TB).
```

State the determinant properties you use in order and explain why the factors involving B eventually cancel.

## Solution

### 1. Product Property

The determinant of a product equals the product of the determinants:

```math
\det(B^{-1}A^TB)
=\det(B^{-1})\det(A^T)\det(B).
```

### 2. Inverse Property

Since B is invertible:

```math
\det(B^{-1})=\frac{1}{\det(B)}=\frac13.
```

### 3. Transpose Property

Transposition does not change the determinant:

```math
\det(A^T)=\det(A)=-2.
```

### 4. Substitution and Cancellation

Substituting gives:

```math
\det(B^{-1}A^TB)
=\frac13(-2)(3)=-2.
```

The factors involving B are reciprocal nonzero scalars:

```math
\det(B^{-1})\det(B)
=\frac{1}{\det(B)}\det(B)=1.
```

Scalar multiplication is commutative, so these factors cancel, leaving det(Aᵀ) = det(A). Therefore, the answer is −2.
