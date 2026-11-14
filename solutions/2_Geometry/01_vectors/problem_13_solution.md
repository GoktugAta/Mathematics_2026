# Exercise 13. Do Four Points Lie in One Plane?

## Question

Given

```math
A=(0,0,0),
\qquad
B=(1,2,0),
\qquad
C=(0,1,1),
\qquad
D=(2,5,1),
```

1. Construct the vectors AB and AC.
2. Find their cross product n.
3. Construct AD and check whether its dot product with n is zero.
4. Decide whether D lies in the plane determined by A, B, and C, and justify the criterion.

## Solution

### 1. Constructing AB and AC

Subtract the coordinates of A from the endpoint coordinates:

```math
\overrightarrow{AB}=B-A=(1,2,0),
```

```math
\overrightarrow{AC}=C-A=(0,1,1).
```

### 2. Finding a normal vector

Compute the cross product:

```math
n=\overrightarrow{AB}\times\overrightarrow{AC}.
```

Using the component formula gives

```math
n=
(2(1)-0(1),\;
0(0)-1(1),\;
1(1)-2(0)).
```

Therefore,

```math
\boxed{n=(2,-1,1)}.
```

This vector is nonzero, so AB and AC are not parallel. Hence, A, B, and C determine a unique plane with normal vector n.

### 3. Constructing AD and computing the dot product

The displacement from A to D is

```math
\overrightarrow{AD}=D-A=(2,5,1).
```

Its dot product with the normal vector is

```math
\overrightarrow{AD}\cdot n
=(2,5,1)\cdot(2,-1,1)
=4-5+1
=0.
```

Therefore, AD is perpendicular to the plane's normal vector.

### 4. Deciding whether D lies in the plane

A point P lies in the plane through A with normal vector n exactly when

```math
(P-A)\cdot n=0.
```

This condition means that the displacement from A to P has no component in the normal direction, so it lies along the plane.

Since

```math
(D-A)\cdot n=0,
```

D lies in the plane determined by A, B, and C. Therefore, all four points are coplanar.

### 5. Additional verification

We can also express AD as a combination of the two plane vectors:

```math
2\overrightarrow{AB}+\overrightarrow{AC}
=2(1,2,0)+(0,1,1)
=(2,5,1)
=\overrightarrow{AD}.
```

This directly confirms that AD lies in the span of AB and AC, so D belongs to the same plane.
