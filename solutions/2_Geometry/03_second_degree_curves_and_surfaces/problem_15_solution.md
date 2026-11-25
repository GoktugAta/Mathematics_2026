# Exercise 15. Recognition and Sketch Without a Given Name

## Question

Consider the two equations:

```math
4x^2+9y^2-8x+36y+4=0,
```

```math
4x^2+y^2=z^2.
```

For the first equation, reduce it to canonical form, recognize the curve, give its most important features, and make a sketch.

For the second equation, do not begin by using a ready-made name for the surface. First describe the cross-sections z=c and the cross-sections by the planes x=0 and y=0, paying attention to the different scales along the axes. Only then identify the surface and make a sketch.

## Solution

### 1. Reducing the first equation to canonical form

Group the terms and complete the squares:

```math
4(x^2-2x)+9(y^2+4y)+4=0.
```

Using

```math
x^2-2x=(x-1)^2-1,
```

```math
y^2+4y=(y+2)^2-4,
```

we obtain

```math
4(x-1)^2-4+9(y+2)^2-36+4=0.
```

Therefore,

```math
4(x-1)^2+9(y+2)^2=36.
```

Dividing by 36 gives

```math
\boxed{\frac{(x-1)^2}{9}+\frac{(y+2)^2}{4}=1}.
```

### 2. Recognizing the curve and its features

The canonical form describes an ellipse with center

```math
\boxed{C=(1,-2)}.
```

Its semiaxis lengths are

```math
\boxed{a=3\text{ horizontally},\qquad b=2\text{ vertically}}.
```

The major axis is horizontal and has length 6. The minor axis has length 4.

The vertices are

```math
(1\pm3,-2),
```

that is,

```math
\boxed{(-2,-2),\qquad (4,-2)}.
```

The co-vertices are

```math
(1,-2\pm2),
```

that is,

```math
\boxed{(1,-4),\qquad (1,0)}.
```

The focal distance is

```math
\sqrt{a^2-b^2}=\sqrt{9-4}=\sqrt5,
```

so the foci are

```math
(1-\sqrt5,-2),\qquad (1+\sqrt5,-2).
```

### 3. Sketching the ellipse

Mark the center, the two vertices, and the two co-vertices. Draw a smooth closed oval through these four boundary points.

The ellipse is symmetric about x=1 and y=-2. It extends horizontally from x=-2 to x=4 and vertically from y=-4 to y=0.

A parametrization for plotting is

```math
x=1+3\cos t,
\qquad
y=-2+2\sin t,
\qquad
0\leq t<2\pi.
```

### 4. Horizontal sections of the second surface

Now consider

```math
4x^2+y^2=z^2.
```

At z=c, the equation becomes

```math
4x^2+y^2=c^2.
```

For c≠0, divide by c²:

```math
\frac{x^2}{c^2/4}+\frac{y^2}{c^2}=1.
```

Thus, the section is an ellipse centered at (0,0,c), with semiaxis lengths

```math
\boxed{\frac{|c|}{2}\text{ along }x,\qquad |c|\text{ along }y}.
```

Each ellipse is twice as wide in the y-direction as in the x-direction.

For example:

| Height | x semiaxis | y semiaxis |
|---|---|---|
| z=±1 | 1/2 | 1 |
| z=±2 | 1 | 2 |
| z=±4 | 2 | 4 |

At c=0, the equation requires x=y=0, so the section is the origin.

### 5. Vertical section x=0

Setting x=0 gives

```math
y^2=z^2.
```

Therefore,

```math
\boxed{y=z\qquad\text{or}\qquad y=-z}.
```

The section consists of two intersecting lines in the yz-plane. At height z=c, they give y=±c.

### 6. Vertical section y=0

Setting y=0 gives

```math
4x^2=z^2.
```

Therefore,

```math
\boxed{z=2x\qquad\text{or}\qquad z=-2x}.
```

The section consists of two intersecting lines in the xz-plane. At height z=c, they give x=±c/2.

This confirms that the surface is narrower in the x-direction than in the y-direction.

### 7. Identifying and sketching the surface

The horizontal sections are ellipses that shrink to a point at z=0 and expand linearly with |z|. The vertical coordinate sections are pairs of straight lines through the origin.

Therefore, the surface is an elliptic double cone with vertex at the origin and axis along the z-axis.

For the sketch, draw the horizontal ellipses from the table above and below the origin. Connect corresponding points with straight generators through the vertex.

The two parts meet at the origin, and each horizontal ellipse is twice as wide along y as along x.

A parametrization for plotting is

```math
(x,y,z)=
\left(\frac{|s|}{2}\cos t,\;|s|\sin t,\;s\right),
\qquad
s\in\mathbb{R},\quad 0\leq t<2\pi.
```
