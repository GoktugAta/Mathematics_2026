# Exercise 14. Contrast: Intersection and Parallelism

## Question

From the point P=(0,0,1), two lines are drawn with direction vectors

```math
v_1=(2,1,-1),
\qquad
v_2=(2,1,0).
```

For each line, analyze its position relative to the plane z=0.

For the line that intersects the plane, find the intersection point. For the other line, explain how you can recognize parallelism without solving an equation.

## Solution

### 1. Identifying the plane's normal vector

The plane z=0 has normal vector

```math
n=(0,0,1).
```

The dot product of a line's direction vector with n determines whether the line moves toward or away from the plane, or stays at a constant height.

### 2. Analyzing the first line

The first line has equation

```math
L_1:\ (x,y,z)=(0,0,1)+t(2,1,-1).
```

Its direction satisfies

```math
n\cdot v_1=(0,0,1)\cdot(2,1,-1)=-1.
```

Since this is nonzero, the line intersects the plane at exactly one point.

The coordinate equations are

```math
x=2t,\qquad y=t,\qquad z=1-t.
```

At the intersection, z=0, so

```math
1-t=0,
\qquad t=1.
```

Substituting gives

```math
\boxed{I=(2,1,0)}.
```

This point lies on L_1 at t=1 and satisfies z=0, confirming the intersection.

### 3. Analyzing the second line

The second line has equation

```math
L_2:\ (x,y,z)=(0,0,1)+s(2,1,0).
```

Its direction satisfies

```math
n\cdot v_2=(0,0,1)\cdot(2,1,0)=0.
```

Thus, its direction is parallel to the plane.

The starting point P has z=1, so it does not belong to the plane. Therefore, L_2 is parallel to the plane and has no common points with it.

No equation needs to be solved: the zero third component of v_2 means that movement along the line never changes the z-coordinate. Every point on L_2 remains at height z=1, while the plane has z=0.

### 4. Comparing the two cases

Both lines start at the same point, but their vertical direction components differ.

The first line has vertical component -1, allowing it to reach z=0. The second has vertical component zero, so it remains at a constant height and never reaches the plane.
