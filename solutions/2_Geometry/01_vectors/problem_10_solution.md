# Exercise 10. Triangle Area from Vectors

## Question

The points

```math
A=(0,0,0),
\qquad
B=(2,1,0),
\qquad
C=(1,3,2)
```

form a triangle.

Construct the vectors AB and AC, compute the area of the parallelogram using the cross product, and then find the area of the triangle. Explain the factor 1/2.

## Solution

### 1. Constructing the side vectors

Subtract the coordinates of A from the coordinates of each endpoint:

```math
\overrightarrow{AB}=B-A
=(2-0,1-0,0-0)
=(2,1,0),
```

```math
\overrightarrow{AC}=C-A
=(1-0,3-0,2-0)
=(1,3,2).
```

Both vectors start at A and form two adjacent sides of a parallelogram.

### 2. Computing the cross product

Using the component formula gives

```math
\overrightarrow{AB}\times\overrightarrow{AC}
=
(1(2)-0(3),\;
0(1)-2(2),\;
2(3)-1(1)).
```

Therefore,

```math
\overrightarrow{AB}\times\overrightarrow{AC}
=(2,-4,5).
```

### 3. Finding the parallelogram area

The area of a parallelogram formed by two vectors is the length of their cross product:

```math
S_{\mathrm{parallelogram}}
=
\left\|
\overrightarrow{AB}\times\overrightarrow{AC}
\right\|.
```

Thus,

```math
S_{\mathrm{parallelogram}}
=\sqrt{2^2+(-4)^2+5^2}
=\sqrt{4+16+25}
=\sqrt{45}.
```

Therefore,

```math
\boxed{S_{\mathrm{parallelogram}}=3\sqrt5}.
```

This formula agrees with base times height because the cross-product magnitude is the product of the side lengths and the sine of their included angle.

### 4. Finding the triangle area

The triangle occupies half of this parallelogram, so

```math
S_{\mathrm{triangle}}
=\frac12
\left\|
\overrightarrow{AB}\times\overrightarrow{AC}
\right\|.
```

Therefore,

```math
\boxed{S_{\mathrm{triangle}}=\frac{3\sqrt5}{2}}.
```

### 5. Explaining the factor 1/2

A diagonal divides a parallelogram into two congruent triangles. The triangle ABC is one of these two triangles.

Equivalently, the triangle and the parallelogram have the same base and height. The parallelogram has area base times height, while the triangle has half that area. This explains the factor 1/2.
