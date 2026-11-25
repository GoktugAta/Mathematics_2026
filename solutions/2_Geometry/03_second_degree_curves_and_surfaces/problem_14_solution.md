# Exercise 14. Cone and Cylinder

## Question

Compare

```math
x^2+y^2=z^2
```

and

```math
x^2+y^2=4.
```

For each surface, describe the cross-sections z=c, x=0, and y=0, make a sketch, and explain why the radius of the cross-section depends on z in the first case but is constant in the second.

## Solution

### 1. The surface x²+y²=z²

#### Horizontal cross-sections z=c

Substituting z=c gives

```math
x^2+y^2=c^2.
```

For c≠0, this is a circle centered at (0,0,c) with radius

```math
\boxed{r=|c|}.
```

For c=0, the cross-section is the single point (0,0,0).

The circles grow linearly with the distance from the xy-plane. Sections at heights c and -c have the same radius.

#### Cross-section x=0

Setting x=0 gives

```math
y^2=z^2,
```

so

```math
y=z\qquad\text{or}\qquad y=-z.
```

The section consists of two intersecting lines in the yz-plane.

#### Cross-section y=0

Setting y=0 gives

```math
x^2=z^2,
```

so

```math
x=z\qquad\text{or}\qquad x=-z.
```

The section consists of two intersecting lines in the xz-plane.

#### Shape and sketch

The surface is a circular double cone with vertex at the origin and axis along the z-axis.

To construct the sketch, mark the vertex and draw horizontal circles of radius 1 at z=±1 and radius 2 at z=±2. Connect them along straight generators through the vertex.

There are two parts opening upward and downward, meeting at the origin.

A parametrization for plotting the surface is

```math
(x,y,z)=(|s|\cos t,|s|\sin t,s),
\qquad s\in\mathbb{R},\quad 0\leq t<2\pi.
```

### 2. The surface x²+y²=4

#### Horizontal cross-sections z=c

The equation does not contain z, so for every real c the section is

```math
x^2+y^2=4,
\qquad z=c.
```

This is a circle centered at (0,0,c) with constant radius

```math
\boxed{r=2}.
```

#### Cross-section x=0

Setting x=0 gives

```math
y^2=4,
\qquad y=\pm2.
```

Since z is unrestricted, the section consists of two lines parallel to the z-axis:

```math
(0,2,z),\qquad (0,-2,z).
```

#### Cross-section y=0

Setting y=0 gives

```math
x^2=4,
\qquad x=\pm2.
```

The section consists of two lines parallel to the z-axis:

```math
(2,0,z),\qquad (-2,0,z).
```

#### Shape and sketch

The surface is a circular cylinder of radius 2 with axis along the z-axis.

For the sketch, draw equal horizontal circles at several heights and connect their outlines with vertical lines. The cylinder extends indefinitely in both z-directions and has no caps.

A parametrization is

```math
(x,y,z)=(2\cos t,2\sin t,s),
\qquad s\in\mathbb{R},\quad 0\leq t<2\pi.
```

### 3. Why the radii behave differently

For the cone, the squared distance from the z-axis is

```math
r^2=x^2+y^2=z^2,
```

so r=|z|. Changing the height changes the radius.

For the cylinder,

```math
r^2=x^2+y^2=4,
```

so r=2 at every height. Since z does not appear in the equation, changing z does not change the allowed x and y coordinates.
