# Exercise 7. A Line Relative to a Plane

## Question

For

```math
L:\ (x,y,z)=(1,1,0)+t(1,-1,0),
\qquad t\in\mathbb{R},
```

and

```math
\Pi:\ x+y+z=2,
```

determine whether the line intersects the plane at one point, is parallel to it, or lies in it.

Explain the role of the dot product of the direction vector and the normal vector.

## Solution

### 1. Identifying the relevant vectors

A point on the line is

```math
P_0=(1,1,0).
```

The line's direction vector and the plane's normal vector are

```math
d=(1,-1,0),
\qquad
n=(1,1,1).
```

### 2. Computing the dot product

```math
d\cdot n
=1(1)+(-1)(1)+0(1)
=0.
```

Thus, the line's direction is perpendicular to the normal vector and parallel to the plane.

This alone does not distinguish between a line lying in the plane and a line parallel to it without meeting it. We must also check a point.

### 3. Checking a point on the line

Substitute P_0=(1,1,0) into the plane equation:

```math
1+1+0=2.
```

Therefore, P_0 lies in the plane.

Since the line starts in the plane and its direction is parallel to the plane, the entire line lies in the plane.

### 4. Verifying all points on the line

The coordinate equations of L are

```math
x=1+t,
\qquad
y=1-t,
\qquad
z=0.
```

Substituting into the plane equation gives

```math
x+y+z=(1+t)+(1-t)+0=2.
```

This holds for every real t. Hence,

```math
\boxed{L\subset\Pi}.
```

The line and plane share every point of L, so there are infinitely many common points.

### 5. Explaining the general dot-product test

For a line X=P_0+td and a plane with equation n·X=c, substitution gives

```math
n\cdot P_0+t(n\cdot d)=c.
```

If the dot product n·d is nonzero, this equation determines exactly one parameter value, giving one intersection point.

If the dot product is zero, the left-hand side is constant along the line. There are then two possibilities:

- If P_0 satisfies the plane equation, the entire line lies in the plane.
- If P_0 does not satisfy it, the line is parallel to the plane and has no intersection.

In this problem, the dot product is zero and P_0 satisfies the plane equation, so the line lies in the plane.
