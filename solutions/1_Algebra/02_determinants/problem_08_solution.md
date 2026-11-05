# Exercise 8. Determinant of a Product

## Question

Let A and B be square matrices such that:

```math
\det(A)=3,
\qquad
\det(B)=-5.
```

Compute det(AB), det(BA), and, if it exists, det(A⁻¹B). Explain why the first two results are equal even though usually AB ≠ BA.

## Solution

### 1. Computing det(AB)

Using the product property:

```math
\det(AB)=\det(A)\det(B)=3(-5)=-15.
```

### 2. Computing det(BA)

Similarly:

```math
\det(BA)=\det(B)\det(A)=(-5)3=-15.
```

### 3. Computing det(A⁻¹B)

Since det(A) = 3 is nonzero, A⁻¹ exists. The determinant of the inverse is the reciprocal of the original determinant:

```math
\det(A^{-1})=\frac{1}{\det(A)}=\frac13.
```

Therefore:

```math
\det(A^{-1}B)
=\det(A^{-1})\det(B)
=\frac13(-5)
=-\frac53.
```

### 4. Explaining the Equal Determinants

Although matrix multiplication is generally noncommutative, determinants are scalars and scalar multiplication is commutative:

```math
\det(AB)
=\det(A)\det(B)
=\det(B)\det(A)
=\det(BA).
```

Equal determinants do not imply that AB and BA are equal matrices.
