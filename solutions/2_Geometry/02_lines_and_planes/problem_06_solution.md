# Exercise 6. Angle Between Planes

## Question

Given

```math
\Pi_1:\ x+y+z=1,
\qquad
\Pi_2:\ x-y=2,
```

first use the normal vectors to decide whether the planes are parallel.

If not, compute the angle between them and explain why the normal vectors alone are enough for this calculation.

## Solution

### 1. Identifying the normal vectors

The coefficients of x, y, and z give a normal vector to each plane:

```math
n_1=(1,1,1),
\qquad
n_2=(1,-1,0).
```

The zero in n_2 corresponds to the missing z term.

### 2. Checking whether the planes are parallel

Two planes are parallel when their normal vectors are scalar multiples.

Here, n_1 and n_2 are not scalar multiples. Every scalar multiple of n_2 has third component zero, whereas n_1 has third component one.

Therefore, the planes are not parallel.

### 3. Computing the angle

The smaller angle between two planes is found from their normal vectors:

```math
\cos\theta
=\frac{|n_1\cdot n_2|}{\|n_1\|\|n_2\|}.
```

The absolute value makes the result independent of which orientation is chosen for each normal vector.

Compute the dot product:

```math
n_1\cdot n_2
=1(1)+1(-1)+1(0)
=0.
```

The lengths are

```math
\|n_1\|=\sqrt3,
\qquad
\|n_2\|=\sqrt2.
```

Therefore,

```math
\cos\theta=\frac{0}{\sqrt3\sqrt2}=0.
```

Thus,

```math
\boxed{\theta=90^\circ=\frac{\pi}{2}}.
```

The planes are perpendicular.

### 4. Why the normal vectors are sufficient

A normal vector determines a plane's orientation. The angle between planes depends on their orientations, so it can be calculated from their normal vectors.

The constants on the right-hand sides determine the positions of the planes but do not affect their orientations. Therefore, no points or intersection line are needed to calculate the angle.
