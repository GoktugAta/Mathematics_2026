# Exercise 3. Plane Through a Point with a Given Normal Vector

## Question

Find the equation of the plane through P=(1,-2,3) and perpendicular to n=(2,1,-1).

Check the result by substituting the point P and explain the role of the normal vector.

## Solution

### 1. Using the normal-vector condition

For any point X=(x,y,z) in the plane, the displacement X-P lies along the plane. Therefore, it must be perpendicular to n:

```math
n\cdot(X-P)=0.
```

Substituting the given point and normal vector gives

```math
(2,1,-1)\cdot(x-1,y+2,z-3)=0.
```

Thus,

```math
2(x-1)+(y+2)-(z-3)=0.
```

### 2. Simplifying the equation

Expanding gives

```math
2x-2+y+2-z+3=0.
```

Therefore, the plane equation is

```math
\boxed{2x+y-z+3=0}.
```

### 3. Checking the given point

Substitute P=(1,-2,3):

```math
2(1)+(-2)-3+3=0.
```

Thus, P lies in the plane.

### 4. Explaining the normal vector

The vector n=(2,1,-1) is perpendicular to every direction lying in the plane. Its components are the coefficients of x, y, and z in the plane equation.

The normal vector determines the orientation of the plane, while the point P fixes its position.

Any nonzero scalar multiple of n describes the same normal direction and can be used to obtain an equivalent plane equation.
