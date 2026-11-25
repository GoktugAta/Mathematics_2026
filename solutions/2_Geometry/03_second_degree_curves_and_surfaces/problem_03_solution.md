# Exercise 3. Ellipse

## Question

For

```math
\frac{x^2}{25}+\frac{y^2}{9}=1,
```

find the semiaxis lengths, the intercepts with the coordinate axes, and make a sketch.

Explain along which axis the ellipse is more stretched and how this is visible in the equation.

## Solution

### 1. Finding the center and semiaxis lengths

Compare the equation with the standard form

```math
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1.
```

There are no coordinate shifts, so the center is (0,0).

The semiaxis lengths are the square roots of the denominators:

```math
\boxed{a=5,\qquad b=3}.
```

The horizontal semiaxis has length 5, while the vertical semiaxis has length 3. Therefore, the full axis lengths are 10 and 6.

### 2. Finding the x-axis intercepts

Set y=0:

```math
\frac{x^2}{25}=1.
```

Therefore,

```math
x^2=25,
\qquad x=\pm5.
```

The x-axis intercepts are

```math
\boxed{(-5,0),\qquad (5,0)}.
```

### 3. Finding the y-axis intercepts

Set x=0:

```math
\frac{y^2}{9}=1.
```

Thus,

```math
y^2=9,
\qquad y=\pm3.
```

The y-axis intercepts are

```math
\boxed{(0,-3),\qquad (0,3)}.
```

### 4. Sketch and orientation

Mark the center and the four intercepts, then draw a smooth closed oval through them, symmetric about both coordinate axes.

The ellipse extends from -5 to 5 horizontally and from -3 to 3 vertically. Thus, it is more stretched along the x-axis.

This is visible directly from the equation: the larger denominator, 25, is under x^2, giving the larger semiaxis in the horizontal direction.

An exact parametrization useful for plotting the sketch is

```math
x=5\cos t,
\qquad
y=3\sin t,
\qquad
0\leq t\leq2\pi.
```

It satisfies the equation because

```math
\frac{(5\cos t)^2}{25}
+\frac{(3\sin t)^2}{9}
=\cos^2t+\sin^2t
=1.
```
