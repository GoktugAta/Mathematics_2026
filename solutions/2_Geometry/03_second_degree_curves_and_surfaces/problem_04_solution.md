# Exercise 4. Parabola

## Question

For

```math
y^2=12x,
```

identify the vertex, axis of symmetry, and opening direction.

Find points on the parabola for x=3 and use them to make a sketch.

## Solution

### 1. Identifying the vertex

The equation has the standard form

```math
y^2=4px.
```

There are no coordinate shifts, so the vertex is

```math
\boxed{V=(0,0)}.
```

### 2. Finding the axis of symmetry

Replacing y by -y leaves the equation unchanged because

```math
(-y)^2=y^2.
```

Therefore, the curve is symmetric about the x-axis. Its axis of symmetry is

```math
\boxed{y=0}.
```

### 3. Determining the opening direction

Since y^2 is nonnegative,

```math
x=\frac{y^2}{12}\geq0.
```

Thus, the parabola opens to the right, in the positive x-direction.

### 4. Finding the points for x=3

Substituting x=3 gives

```math
y^2=12(3)=36.
```

Therefore,

```math
y=\pm6.
```

The required points are

```math
\boxed{(3,6),\qquad (3,-6)}.
```

Checking either point gives

```math
(\pm6)^2=36=12(3).
```

### 5. Sketch

Mark the vertex (0,0) and the points (3,6) and (3,-6). Draw a smooth curve through them opening to the right.

The upper and lower parts are mirror images across the x-axis, and no part of the curve lies where x<0.

An exact parametrization for plotting is

```math
(x,y)=\left(\frac{t^2}{12},t\right),
\qquad t\in\mathbb{R}.
```

The parameter values t=0, t=6, and t=-6 give the vertex and the two calculated points.
