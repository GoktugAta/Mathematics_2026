# Exercise 6. Projection and Perpendicular Component

## Question

Find the projection of u=(4,2) onto the direction v=(1,1).

Then compute

```math
r=u-\mathrm{proj}_v u
```

and verify that

```math
r\cdot v=0.
```

Explain this result geometrically.

## Solution

### 1. Finding the projection

For a nonzero vector v, the vector projection of u onto its direction is

```math
\mathrm{proj}_v u
=\frac{u\cdot v}{v\cdot v}v.
```

We compute the two dot products:

```math
u\cdot v=4(1)+2(1)=6,
```

```math
v\cdot v=1^2+1^2=2.
```

Therefore,

```math
\mathrm{proj}_v u
=\frac62(1,1)
=3(1,1)
=\boxed{(3,3)}.
```

This is a scalar multiple of v, so it is parallel to v.

### 2. Computing the perpendicular component

Subtract the projection from the original vector:

```math
r=u-\mathrm{proj}_v u
=(4,2)-(3,3).
```

Thus,

```math
\boxed{r=(1,-1)}.
```

### 3. Verifying perpendicularity

Compute the dot product of r with v:

```math
r\cdot v=(1,-1)\cdot(1,1)
=1(1)+(-1)(1)
=0.
```

Since both vectors are nonzero and their dot product is zero, r is perpendicular to v.

### 4. Geometric explanation

The projection decomposes u into a component parallel to v and a component perpendicular to v:

```math
u=\mathrm{proj}_v u+r.
```

In this example,

```math
(4,2)=(3,3)+(1,-1).
```

The vector (3,3) lies on the line through the origin in the direction (1,1), which is the line y=x.

The vector r=(1,-1) runs from the projection point (3,3) to the endpoint (4,2) of u. It is perpendicular to that line.

Therefore, the projection point is the closest point on the line y=x to the endpoint of u.
