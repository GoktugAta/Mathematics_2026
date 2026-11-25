# Exercise 1. Recognizing Curves from Canonical Form

## Question

Recognize the curves

```math
x^2+y^2=9,
```

```math
\frac{x^2}{16}+\frac{y^2}{9}=1,
```

```math
y^2=8x,
```

```math
\frac{x^2}{9}-\frac{y^2}{4}=1.
```

For each one, identify the most important features and make a sketch. Explain which parts of the equation let you recognize the type of curve.

## Solution

### 1. Circle

The canonical equation of a circle is

```math
(x-h)^2+(y-k)^2=r^2.
```

Comparing this with x^2+y^2=9 gives

```math
\boxed{\text{Center }(0,0),\qquad r=3}.
```

Both variables are squared, their coefficients are equal, and the squared terms are added. These features identify a circle.

Its intercepts are

```math
(3,0),\quad (-3,0),\quad (0,3),\quad (0,-3).
```

For the sketch, mark these four points and draw a circle centered at the origin through them. The curve is symmetric about both coordinate axes.

### 2. Ellipse

The equation

```math
\frac{x^2}{16}+\frac{y^2}{9}=1
```

has two positive squared terms with different denominators. Therefore, it represents an ellipse centered at the origin.

The semiaxis lengths are

```math
a=\sqrt{16}=4,
\qquad
b=\sqrt9=3.
```

The larger denominator is under x^2, so the major axis is horizontal.

The vertices and co-vertices are

```math
\boxed{(\pm4,0),\qquad (0,\pm3)}.
```

The focal distance satisfies

```math
c^2=a^2-b^2=16-9=7.
```

Thus, the foci are

```math
(\pm\sqrt7,0).
```

For the sketch, mark the four axis intercepts and draw a smooth closed oval through them. It extends farther horizontally than vertically and is symmetric about both axes.

### 3. Parabola

Compare

```math
y^2=8x
```

with the canonical form

```math
y^2=4px.
```

Since 4p=8, we obtain p=2.

Only y is squared, while x appears to the first power. This identifies a parabola with a horizontal axis. The positive coefficient of x means that it opens to the right.

Its main features are

```math
\boxed{\text{Vertex }(0,0),\qquad \text{Focus }(2,0)}.
```

The directrix and axis of symmetry are

```math
x=-2,
\qquad
y=0.
```

For the sketch, mark the vertex and the points

```math
(2,4),\qquad (2,-4),
```

which satisfy y^2=8x. Draw a smooth curve opening right through these points, symmetric about the x-axis. There are no points with x<0 because y^2 is nonnegative.

### 4. Hyperbola

The equation

```math
\frac{x^2}{9}-\frac{y^2}{4}=1
```

contains squared terms with opposite signs, identifying a hyperbola.

Its center is (0,0). Since the x^2 term is positive, the branches open left and right.

The parameters are

```math
a=3,\qquad b=2.
```

Therefore, its vertices are

```math
\boxed{(\pm3,0)}.
```

For a hyperbola, the focal distance satisfies

```math
c^2=a^2+b^2=9+4=13.
```

Thus, the foci are

```math
(\pm\sqrt{13},0).
```

Its asymptotes are

```math
\boxed{y=\pm\frac23x}.
```

For the sketch, first draw the asymptotes as dashed lines. Mark the vertices (-3,0) and (3,0), then draw two branches opening outward from them and approaching the asymptotes.

The branches are symmetric about both coordinate axes. There are no y-intercepts because x=0 would require

```math
-\frac{y^2}{4}=1,
```

which has no real solution.

### 5. Summary of the sketches

| Curve | Center or vertex | Points to mark | Shape |
|---|---|---|---|
| Circle | Center (0,0) | (±3,0), (0,±3) | Closed circle |
| Ellipse | Center (0,0) | (±4,0), (0,±3) | Closed horizontal oval |
| Parabola | Vertex (0,0) | (2,±4) | Opens right |
| Hyperbola | Center (0,0) | Vertices (±3,0) | Opens left and right; asymptotes y=±2x/3 |
