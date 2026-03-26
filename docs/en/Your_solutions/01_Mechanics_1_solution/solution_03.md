# Alice and Bob: Motion Analysis

## 1. Problem Setup
The positions of Alice and Bob are given by:

$$
A(t) = (2+t, 8-3t)
$$

$$
B(t) = (2t-1, 2t+2)
$$

## 2. Collision Test
For a collision to occur, $x_A(t) = x_B(t)$ and $y_A(t) = y_B(t)$ for the same $t$.

1. $2+t = 2t-1 \implies t = 3$
2. At $t=3$: $y_A = -1$ and $y_B = 8$.

**Result:** No collision occurs.

## 3. Minimum Distance Calculation
The distance $D$ between them satisfies:

$$
D^2 = [(2t-1) - (2+t)]^2 + [(2t+2) - (8-3t)]^2
$$

Simplifying:

$$
D^2 = 26t^2 - 66t + 45
$$

To find the minimum, we find the vertex of the parabola:

$$
t_{min} = \frac{-(-66)}{2(26)} = \frac{33}{26} \approx 1.27 \text{ s}
$$

The minimum distance is:

$$
D_{min} = \sqrt{26(\frac{33}{26})^2 - 66(\frac{33}{26}) + 45} \approx 1.74 \text{ units}
$$
