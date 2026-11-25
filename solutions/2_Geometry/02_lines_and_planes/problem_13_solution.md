# Exercise 13. Closest Point on a Plane

## Question

Find the point on the plane

```math
x+2y+2z=4
```

closest to P=(3,0,0).

Give the distance and check that the segment joining the two points is perpendicular to the plane.

## Solution

### 1. Constructing the perpendicular displacement

The plane has normal vector

```math
n=(1,2,2).
```

The closest point H is reached by moving from P along the normal direction. Write

```math
H=P+\lambda n
=(3+\lambda,2\lambda,2\lambda).
```

### 2. Requiring H to lie in the plane

Substitute these coordinates into the plane equation:

```math
(3+\lambda)+2(2\lambda)+2(2\lambda)=4.
```

Therefore,

```math
3+9\lambda=4,
\qquad
\lambda=\frac19.
```

The closest point is

```math
\boxed{H=\left(\frac{28}{9},\frac29,\frac29\right)}.
```

### 3. Checking that H lies in the plane

Substitution gives

```math
\frac{28}{9}
+2\left(\frac29\right)
+2\left(\frac29\right)
=\frac{28+4+4}{9}
=4.
```

Thus, H belongs to the plane.

### 4. Checking perpendicularity

The displacement from P to H is

```math
H-P
=\left(\frac19,\frac29,\frac29\right)
=\frac19(1,2,2)
=\frac19n.
```

Since this displacement is parallel to the normal vector, the segment PH is perpendicular to the plane.

### 5. Computing the distance

The distance is the length of H-P:

```math
d=\|H-P\|
=\sqrt{\left(\frac19\right)^2+
\left(\frac29\right)^2+
\left(\frac29\right)^2}.
```

Hence,

```math
d=\sqrt{\frac9{81}}
=\boxed{\frac13}.
```

The point-to-plane distance formula confirms this:

```math
d=\frac{|3+2(0)+2(0)-4|}
{\sqrt{1^2+2^2+2^2}}
=\frac13.
```

### 6. Why H is the closest point

For any point R in the plane, H-R lies along the plane and is perpendicular to P-H. Therefore,

```math
\|P-R\|^2=\|P-H\|^2+\|H-R\|^2.
```

The second term is nonnegative and equals zero only when R=H. Consequently, H is the unique closest point to P on the plane.
