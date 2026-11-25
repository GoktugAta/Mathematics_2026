# Exercise 13. Intersection of a Sphere and a Plane

## Question

Given the sphere

```math
x^2+y^2+z^2=25
```

and the plane z=3, find the equation of the intersection curve and its radius.

Then describe what happens for z=c depending on c.

## Solution

### 1. Finding the intersection with z=3

Substitute z=3 into the sphere equation:

```math
x^2+y^2+3^2=25.
```

Therefore,

```math
x^2+y^2=16.
```

The intersection curve is described in three-dimensional space by

```math
\boxed{
\begin{cases}
x^2+y^2=16,\\
z=3.
\end{cases}
}
```

It is a circle centered at (0,0,3), with radius

```math
\boxed{r=4}.
```

The condition z=3 must be included to specify the circle's position in space.

### 2. Checking a point on the circle

For example, the point (4,0,3) satisfies the plane equation and the sphere equation:

```math
4^2+0^2+3^2=16+9=25.
```

Thus, it belongs to both objects.

### 3. General horizontal plane z=c

Substituting z=c gives

```math
x^2+y^2=25-c^2.
```

The type of intersection depends on the sign of the right-hand side.

### 4. Case |c|<5

The right-hand side is positive, so the intersection is a circle centered at (0,0,c), with radius

```math
\boxed{r(c)=\sqrt{25-c^2}}.
```

The largest circle occurs at c=0 and has radius 5. The radius decreases as |c| increases toward 5.

### 5. Case |c|=5

The equation becomes

```math
x^2+y^2=0.
```

Thus, x=y=0, and the intersection is a single point:

```math
(0,0,5)\quad\text{or}\quad(0,0,-5).
```

The plane is tangent to the sphere.

### 6. Case |c|>5

Here,

```math
25-c^2<0.
```

Since x²+y² cannot be negative for real coordinates, there is no intersection.

### 7. Geometric interpretation

The sphere has center (0,0,0) and radius 5. The distance from its center to the plane z=c is |c|.

Therefore, the plane cuts a circle when this distance is less than 5, touches the sphere when it equals 5, and misses the sphere when it exceeds 5.
