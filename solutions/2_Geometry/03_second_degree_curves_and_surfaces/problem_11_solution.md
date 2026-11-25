# Exercise 11. Two Similar Surfaces

## Question

Compare

```math
x^2+y^2-z^2=1
```

and

```math
x^2+y^2-z^2=-1.
```

For several values z=c, check whether the cross-section exists and what its radius is. Based on this, describe qualitatively the difference between the surfaces and make sketches.

## Solution

### 1. Cross-sections of the first surface

For

```math
x^2+y^2-z^2=1,
```

substituting z=c gives

```math
x^2+y^2=1+c^2.
```

Since 1+c^2 is always positive, every horizontal plane intersects the surface in a circle centered at (0,0,c), with radius

```math
\boxed{r_1(c)=\sqrt{1+c^2}}.
```

The smallest radius is 1, occurring at c=0. The circles grow as |c| increases.

### 2. Cross-sections of the second surface

For

```math
x^2+y^2-z^2=-1,
```

substituting z=c gives

```math
x^2+y^2=c^2-1.
```

Therefore:

- If |c|>1, the section is a circle with radius √(c²−1).
- If |c|=1, the section is a single point.
- If |c|<1, there are no real points.

For the circular sections,

```math
\boxed{r_2(c)=\sqrt{c^2-1}}.
```

### 3. Comparing several heights

| Height c | First surface | Second surface |
|---|---|---|
| -2 | Circle, radius √5 | Circle, radius √3 |
| -1 | Circle, radius √2 | Point (0,0,-1) |
| 0 | Circle, radius 1 | No real points |
| 1 | Circle, radius √2 | Point (0,0,1) |
| 2 | Circle, radius √5 | Circle, radius √3 |

### 4. Qualitative shapes and sketch construction

The first surface is a hyperboloid of one sheet. It is connected and has a circular waist of radius 1 at z=0.

To sketch it, draw the horizontal circles from the table and connect them smoothly. The surface narrows toward z=0 and widens above and below it.

The second surface is a hyperboloid of two sheets. It has two separate parts: one with z≥1 and one with z≤-1.

To sketch it, mark the tips (0,0,1) and (0,0,-1). Draw expanding horizontal circles above the upper tip and below the lower tip. Leave the region -1<z<1 empty.

Both surfaces are symmetric about the xy-plane and rotationally symmetric about the z-axis.

### 5. Equations for plotting the sketches

Let r be the distance from the z-axis:

```math
r=\sqrt{x^2+y^2}.
```

For the first surface:

```math
r=\sqrt{1+z^2}.
```

For the second surface:

```math
z=\pm\sqrt{1+r^2}.
```

These profiles, rotated about the z-axis, give the two surfaces and show the difference between a connected waist and two separated sheets.
