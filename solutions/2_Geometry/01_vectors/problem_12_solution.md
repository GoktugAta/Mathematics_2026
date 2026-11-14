# Exercise 12. A Normal Vector to a Plane

## Question

Given

```math
A=(1,0,2),
\qquad
B=(2,1,0),
\qquad
C=(0,3,1),
```

construct two vectors lying in the plane, find a vector perpendicular to both, and check the perpendicularity using dot products.

## Solution

### 1. Constructing two vectors in the plane

Use two displacement vectors with the same starting point A:

```math
\overrightarrow{AB}=B-A
=(2-1,1-0,0-2)
=(1,1,-2),
```

```math
\overrightarrow{AC}=C-A
=(0-1,3-0,1-2)
=(-1,3,-1).
```

These vectors lie in the plane through A, B, and C.

### 2. Finding a perpendicular vector

The cross product gives a vector perpendicular to both:

```math
n=\overrightarrow{AB}\times\overrightarrow{AC}.
```

Using the component formula:

```math
n=
\left(
1(-1)-(-2)(3),
(-2)(-1)-1(-1),
1(3)-1(-1)
\right).
```

Therefore,

```math
n=(-1+6,2+1,3+1)
=\boxed{(5,3,4)}.
```

Since the cross product is nonzero, the two plane vectors are not parallel. Consequently, A, B, and C determine a unique plane, and n is a normal vector to that plane.

### 3. Checking perpendicularity to AB

```math
n\cdot\overrightarrow{AB}
=(5,3,4)\cdot(1,1,-2)
=5+3-8
=0.
```

Thus, n is perpendicular to AB.

### 4. Checking perpendicularity to AC

```math
n\cdot\overrightarrow{AC}
=(5,3,4)\cdot(-1,3,-1)
=-5+9-4
=0.
```

Thus, n is also perpendicular to AC.

Since AB and AC span the directions of the plane, a vector perpendicular to both is perpendicular to every direction in the plane. Therefore, (5,3,4) is a valid normal vector.

Any nonzero scalar multiple of this vector is also a valid normal vector.
