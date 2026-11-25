# Exercise 12. Intersection Line of Two Planes

## Question

Find a parametric equation of the line that is the intersection of

```math
x+y+z=3,
\qquad
x-y+z=1.
```

Find its direction vector in two ways: from the system of equations and from the cross product of the normal vectors. Compare the results.

## Solution

### 1. Solving the plane equations simultaneously

Subtract the second equation from the first:

```math
(x+y+z)-(x-y+z)=3-1.
```

This gives

```math
2y=2,
\qquad y=1.
```

Substituting into either plane equation gives

```math
x+z=2.
```

Let z=t. Then

```math
x=2-t,\qquad y=1,\qquad z=t.
```

Therefore, the intersection line is

```math
\boxed{
(x,y,z)=(2,1,0)+t(-1,0,1),
\qquad t\in\mathbb{R}
}.
```

Every common point must satisfy y=1 and x+z=2, so this parametrization includes all points of the intersection.

### 2. Finding the direction from the system

The coefficients of t in the coordinate expressions give the direction vector:

```math
\boxed{d=(-1,0,1)}.
```

As z increases by one, x decreases by one and y remains unchanged.

### 3. Finding the direction using the normals

The normal vectors are

```math
n_1=(1,1,1),
\qquad n_2=(1,-1,1).
```

The intersection direction must be perpendicular to both normals. Therefore, we compute their cross product:

```math
n_1\times n_2
=
(1(1)-1(-1),\;
1(1)-1(1),\;
1(-1)-1(1)).
```

Thus,

```math
n_1\times n_2=(2,0,-2).
```

This nonzero vector also gives the direction of the intersection line.

### 4. Comparing the results

The two direction vectors satisfy

```math
(2,0,-2)=-2(-1,0,1).
```

They are nonzero scalar multiples, so they describe the same line direction. The negative factor reverses orientation, while the factor two changes the vector length.

Neither change affects the line when the parameter ranges over all real numbers.

### 5. Checking both plane equations

For a general point (2-t,1,t), the first equation gives

```math
(2-t)+1+t=3.
```

The second gives

```math
(2-t)-1+t=1.
```

Both equations hold for every real t, confirming the intersection line.
