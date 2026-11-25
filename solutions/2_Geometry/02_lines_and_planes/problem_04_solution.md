# Exercise 4. Plane Through Three Points

## Question

Find the equation of the plane through

```math
A=(1,0,0),
\qquad
B=(0,1,0),
\qquad
C=(0,0,1).
```

First construct two vectors lying in the plane, and then use the cross product. Check the resulting equation on all three points.

## Solution

### 1. Constructing two vectors in the plane

Using A as the common starting point gives

```math
\overrightarrow{AB}=B-A=(-1,1,0),
```

```math
\overrightarrow{AC}=C-A=(-1,0,1).
```

### 2. Finding a normal vector

The cross product is perpendicular to both plane vectors:

```math
n=\overrightarrow{AB}\times\overrightarrow{AC}.
```

Using the component formula:

```math
n=
(1(1)-0(0),\;
0(-1)-(-1)(1),\;
(-1)(0)-1(-1)).
```

Therefore,

```math
n=(1,1,1).
```

Since the cross product is nonzero, the two vectors are not parallel. Thus, the three points determine a unique plane.

As a check,

```math
n\cdot\overrightarrow{AB}=-1+1+0=0,
```

```math
n\cdot\overrightarrow{AC}=-1+0+1=0.
```

### 3. Constructing the plane equation

Using the normal vector n and the point A:

```math
n\cdot((x,y,z)-A)=0.
```

This gives

```math
(1,1,1)\cdot(x-1,y,z)=0.
```

Therefore,

```math
\boxed{x+y+z-1=0}.
```

### 4. Checking all three points

For A=(1,0,0):

```math
1+0+0-1=0.
```

For B=(0,1,0):

```math
0+1+0-1=0.
```

For C=(0,0,1):

```math
0+0+1-1=0.
```

All three points satisfy the equation, confirming that it is the required plane.
