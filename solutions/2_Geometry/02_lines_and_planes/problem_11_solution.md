# Exercise 11. Plane Containing a Line and a Point

## Question

Find the equation of the plane containing the line

```math
(x,y,z)=(1,0,2)+t(1,1,-1),
\qquad t\in\mathbb{R},
```

and the point P=(0,2,1).

Check that both the entire line and the point lie in the plane you obtain.

## Solution

### 1. Constructing two directions in the plane

A point on the line is A=(1,0,2), and its direction vector is

```math
d=(1,1,-1).
```

A second vector in the required plane joins A to P:

```math
w=P-A=(0-1,2-0,1-2)=(-1,2,-1).
```

The vectors d and w are not scalar multiples. Therefore, they provide two independent directions and determine a unique plane through A.

### 2. Finding a normal vector

The cross product is perpendicular to both directions:

```math
n=d\times w.
```

Computing the components gives

```math
n=
(1(-1)-(-1)(2),\;
(-1)(-1)-1(-1),\;
1(2)-1(-1)).
```

Thus,

```math
n=(1,2,3).
```

### 3. Constructing the plane equation

Using A and the normal vector:

```math
n\cdot((x,y,z)-A)=0.
```

Therefore,

```math
(x-1)+2y+3(z-2)=0.
```

Simplifying gives

```math
\boxed{x+2y+3z-7=0}.
```

### 4. Checking the entire line

The coordinates of a general point on the line are

```math
x=1+t,\qquad y=t,\qquad z=2-t.
```

Substitution into the plane equation gives

```math
(1+t)+2t+3(2-t)-7
=1+t+2t+6-3t-7
=0.
```

This holds for every real t, so the entire line lies in the plane.

### 5. Checking the point P

Substituting P=(0,2,1) gives

```math
0+2(2)+3(1)-7=0.
```

Therefore, P also lies in the plane, as required.
