# Exercise 9. Distances

## Question

Compute:

1. The distance from P=(2,3) to the line

```math
3x+4y-10=0.
```

2. The distance from Q=(2,-1,3) to the plane

```math
2x-2y+z-4=0.
```

Compare the two formulas and explain their common connection with the normal direction.

## Solution

### 1. Distance from the point to the line

For a line with equation ax+by+c=0, the distance from a point (x_0,y_0) is

```math
d=\frac{|ax_0+by_0+c|}{\sqrt{a^2+b^2}}.
```

The line has normal vector n=(3,4), whose length is

```math
\|n\|=\sqrt{3^2+4^2}=5.
```

Substituting P=(2,3) gives

```math
d(P,L)
=\frac{|3(2)+4(3)-10|}{5}
=\frac{|6+12-10|}{5}.
```

Therefore,

```math
\boxed{d(P,L)=\frac85}.
```

### 2. Distance from the point to the plane

For a plane with equation ax+by+cz+d=0, the distance from a point (x_0,y_0,z_0) is

```math
D=\frac{|ax_0+by_0+cz_0+d|}
{\sqrt{a^2+b^2+c^2}}.
```

The normal vector of the given plane is n=(2,-2,1), with length

```math
\|n\|=\sqrt{2^2+(-2)^2+1^2}=3.
```

Substituting Q=(2,-1,3) gives

```math
d(Q,\Pi)
=\frac{|2(2)-2(-1)+3-4|}{3}
=\frac{|4+2+3-4|}{3}.
```

Thus,

```math
\boxed{d(Q,\Pi)=\frac53}.
```

### 3. Comparing the formulas

Both formulas calculate the length of a displacement in the normal direction, which is perpendicular to the line or plane.

To see this, write either equation as

```math
n\cdot X+c=0,
```

and choose a point X_0 on the line or plane. Since

```math
n\cdot X_0+c=0,
```

we have

```math
n\cdot P+c=n\cdot(P-X_0).
```

Dividing by the normal-vector length gives the scalar component of P-X_0 along a unit normal:

```math
\frac{n\cdot(P-X_0)}{\|n\|}.
```

Taking its absolute value gives the nonnegative perpendicular distance:

```math
\boxed{d=\frac{|n\cdot P+c|}{\|n\|}}.
```

The two formulas therefore express the same geometric idea in two and three dimensions.
