# Exercise 5. Hyperbola and Asymptotes

## Question

For

```math
\frac{x^2}{16}-\frac{y^2}{9}=1,
```

find the intercepts with the x-axis, the asymptotes, and make a sketch.

Explain why the asymptotes describe the behavior of the curve far from the center.

## Solution

### 1. Identifying the hyperbola

The squared terms have opposite signs, so the curve is a hyperbola centered at (0,0).

Comparing with

```math
\frac{x^2}{a^2}-\frac{y^2}{b^2}=1
```

gives

```math
a=4,\qquad b=3.
```

Since the x^2 term is positive, the two branches open left and right.

### 2. Finding the x-axis intercepts

Set y=0:

```math
\frac{x^2}{16}=1.
```

Thus,

```math
x=\pm4.
```

The x-axis intercepts, which are also the vertices, are

```math
\boxed{(-4,0),\qquad (4,0)}.
```

There are no y-axis intercepts because setting x=0 gives

```math
-\frac{y^2}{9}=1,
```

which has no real solution.

### 3. Finding the asymptotes

The asymptotes of this standard hyperbola are

```math
y=\pm\frac{b}{a}x.
```

Therefore,

```math
\boxed{y=\frac34x,\qquad y=-\frac34x}.
```

These lines can also be obtained by setting the quadratic part equal to zero:

```math
\frac{x^2}{16}-\frac{y^2}{9}=0.
```

This gives

```math
y^2=\frac9{16}x^2,
```

and hence the same two lines.

### 4. Sketch

Draw the asymptotes as dashed lines through the origin. A guide rectangle with corners (±4,±3) helps determine their slopes.

Mark the vertices (-4,0) and (4,0). Draw one branch opening right from (4,0) and another opening left from (-4,0), both approaching the asymptotes.

The curve is symmetric about both coordinate axes and has points only where

```math
|x|\geq4.
```

For additional plotting points, setting x=±5 gives

```math
y^2=9\left(\frac{25}{16}-1\right)=\frac{81}{16}.
```

Thus, the four points

```math
\left(\pm5,\pm\frac94\right)
```

lie on the hyperbola.

### 5. Explaining the behavior far from the center

Rearrange the equation:

```math
y^2=\frac9{16}(x^2-16).
```

Therefore,

```math
|y|=\frac34\sqrt{x^2-16}.
```

Compare this with the absolute height of the asymptote at the same x-coordinate:

```math
\frac34|x|.
```

Their difference is

```math
\frac34|x|-|y|
=\frac34\left(|x|-\sqrt{x^2-16}\right).
```

Rationalizing gives

```math
\frac34|x|-|y|
=\frac{12}{|x|+\sqrt{x^2-16}}.
```

As |x| increases without bound, this difference tends to zero. Therefore, the branches approach the lines y=±3x/4, explaining why these asymptotes describe the curve far from its center.
