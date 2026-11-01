# Problem 15 Solution

We are given:

```math
\det(A)=-2,
\qquad
\det(B)=3.
```

### 1. Apply the Product Property

The determinant of a product equals the product of its determinants:

```math
\det(B^{-1}A^TB)
=
\det(B^{-1})\det(A^T)\det(B).
```

### 2. Apply the Inverse and Transpose Properties

For an invertible matrix B:

```math
\det(B^{-1})=\frac{1}{\det(B)}.
```

Transposition does not change the determinant:

```math
\det(A^T)=\det(A).
```

Therefore:

```math
\det(B^{-1}A^TB)
=
\frac{1}{\det(B)}\det(A)\det(B)
=
\frac{1}{3}(-2)(3)
=
\boxed{-2}.
```

### 3. Why the B Factors Cancel

The determinant factors involving B are reciprocal nonzero scalars:

```math
\det(B^{-1})\det(B)
=
\frac{1}{\det(B)}\det(B)
=
1.
```

Since scalar multiplication is commutative, these factors cancel, leaving only det(Aᵀ), which equals det(A).
