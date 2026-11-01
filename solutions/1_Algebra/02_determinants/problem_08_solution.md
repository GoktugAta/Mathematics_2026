# Problem 8 Solution

We are given:

```math
\det(A)=3,
\qquad
\det(B)=-5.
```

### 1. Computing det(AB)

Using the product property:

```math
\det(AB)=\det(A)\det(B)=3(-5)=\boxed{-15}.
```

### 2. Computing det(BA)

Similarly:

```math
\det(BA)=\det(B)\det(A)=(-5)3=\boxed{-15}.
```

### 3. Computing det(A⁻¹B)

Since det(A) = 3 is nonzero, A is invertible. The determinant of its inverse is:

```math
\det(A^{-1})=\frac{1}{\det(A)}=\frac{1}{3}.
```

Therefore:

```math
\det(A^{-1}B)
=
\det(A^{-1})\det(B)
=
\frac{1}{3}(-5)
=
\boxed{-\frac{5}{3}}.
```

### 4. Why det(AB) = det(BA)

Although matrix multiplication is generally noncommutative, determinants are scalars, and scalar multiplication is commutative:

```math
\det(AB)
=
\det(A)\det(B)
=
\det(B)\det(A)
=
\det(BA).
```

Thus, AB and BA have equal determinants even when the matrices themselves are different.
