# Exercise 10. Projection of a Point onto a Plane

## Question

Find the orthogonal projection of P=(2,1,3) onto the plane

```math
x+y+z=3,
```

and then find the reflection of P across this plane.

Check that the midpoint of the segment joining the point and its reflection lies on the plane.

## Solution

### 1. Finding the orthogonal projection

The plane has normal vector

```math
n=(1,1,1).
```

The orthogonal projection H is obtained by moving from P in the normal direction:

```math
H=P-\lambda n.
```

Therefore,

```math
H=(2-\lambda,1-\lambda,3-\lambda).
```

For H to lie in the plane, its coordinates must satisfy

```math
(2-\lambda)+(1-\lambda)+(3-\lambda)=3.
```

Thus,

```math
6-3\lambda=3,
\qquad
\lambda=1.
```

The projection is

```math
\boxed{H=(1,0,2)}.
```

### 2. Checking the projection

First, H satisfies the plane equation:

```math
1+0+2=3.
```

Also, the displacement from H to P is

```math
P-H=(2,1,3)-(1,0,2)=(1,1,1)=n.
```

Therefore, the segment from P to H is perpendicular to the plane. Together, these checks confirm that H is the orthogonal projection.

### 3. Finding the reflection

For reflection across the plane, H is the midpoint between P and its reflection P'.

Therefore,

```math
P'=2H-P.
```

Substituting gives

```math
P'=2(1,0,2)-(2,1,3)
=(2,0,4)-(2,1,3).
```

Hence,

```math
\boxed{P'=(0,-1,1)}.
```

The vectors from H to the two points are opposites:

```math
P-H=(1,1,1),
```

```math
P'-H=(-1,-1,-1)=-(P-H).
```

Thus, P and P' are equally far from the plane on opposite sides along the normal direction.

### 4. Checking the midpoint

The midpoint of P and P' is

```math
M=\frac{P+P'}2
=\left(
\frac{2+0}{2},
\frac{1-1}{2},
\frac{3+1}{2}
\right)
=(1,0,2).
```

This is exactly H. Substitution into the plane equation gives

```math
1+0+2=3.
```

Therefore, the midpoint lies on the plane, as required.
