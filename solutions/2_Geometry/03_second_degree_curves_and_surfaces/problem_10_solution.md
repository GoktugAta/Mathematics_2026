# Exercise 10. Paraboloids

## Question

Compare

```math
z=x^2+y^2
```

and

```math
z=x^2-y^2.
```

For each surface, describe the cross-sections x=0, y=0, and z=c, then make a qualitative sketch.

## Solution

### 1. The surface z=x^2+y^2

This is an elliptic paraboloid. Since the coefficients of x^2 and y^2 are equal, it is also a circular paraboloid.

#### Cross-section x=0

Setting x=0 gives

```math
z=y^2.
```

This is a parabola in the yz-plane, opening upward with vertex at the origin.

#### Cross-section y=0

Setting y=0 gives

```math
z=x^2.
```

This is a parabola in the xz-plane, also opening upward with vertex at the origin.

#### Cross-section z=c

Setting z=c gives

```math
x^2+y^2=c.
```

There are three cases:

- For c>0, the section is a circle of radius √c centered at (0,0,c).
- For c=0, the section is the single point (0,0,0).
- For c<0, there are no real points.

#### Qualitative sketch

The surface has a bowl shape opening in the positive z-direction. Its lowest point is the origin.

Draw upward-opening parabolas in the two vertical coordinate planes and horizontal circles that become larger as z increases.

A parametrization for plotting is

```math
(x,y,z)=(r\cos t,r\sin t,r^2),
\qquad r\geq0,\quad 0\leq t<2\pi.
```

### 2. The surface z=x^2-y^2

This is a hyperbolic paraboloid, commonly called a saddle surface.

#### Cross-section x=0

Setting x=0 gives

```math
z=-y^2.
```

This is a parabola in the yz-plane, opening downward with vertex at the origin.

#### Cross-section y=0

Setting y=0 gives

```math
z=x^2.
```

This is a parabola in the xz-plane, opening upward with vertex at the origin.

Thus, the surface bends in opposite directions in the two vertical coordinate planes.

#### Cross-section z=c

Setting z=c gives

```math
x^2-y^2=c.
```

For c>0, divide by c:

```math
\frac{x^2}{c}-\frac{y^2}{c}=1.
```

This is a hyperbola opening in the positive and negative x-directions.

For c<0, rewrite the equation as

```math
y^2-x^2=-c.
```

Therefore,

```math
\frac{y^2}{-c}-\frac{x^2}{-c}=1.
```

This is a hyperbola opening in the positive and negative y-directions.

For c=0:

```math
x^2-y^2=(x-y)(x+y)=0.
```

The section consists of two intersecting lines:

```math
\boxed{y=x,\qquad y=-x,\qquad z=0}.
```

#### Qualitative sketch

Draw an upward-opening parabola along the x-direction and a downward-opening parabola along the y-direction.

The resulting surface resembles a saddle. The origin is a saddle point, not a maximum or minimum: nearby points have positive z-values along the x-axis and negative z-values along the y-axis.

A parametrization for plotting is

```math
(x,y,z)=(s,t,s^2-t^2),
\qquad s,t\in\mathbb{R}.
```

### 3. Comparison

| Feature | z=x²+y² | z=x²−y² |
|---|---|---|
| Surface type | Elliptic paraboloid | Hyperbolic paraboloid |
| Section x=0 | Upward parabola | Downward parabola |
| Section y=0 | Upward parabola | Upward parabola |
| Section z=c, c>0 | Circle | Hyperbola opening along x |
| Section z=0 | One point | Two intersecting lines |
| Section z=c, c<0 | No real points | Hyperbola opening along y |
| Overall shape | Upward-opening bowl | Saddle |

The key difference is the sign between the squared terms. A sum produces the bowl, while a difference produces opposite bending directions and the saddle.
