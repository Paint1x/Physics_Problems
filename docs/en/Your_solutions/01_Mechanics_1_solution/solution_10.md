# Analysis of 3D Point Motion (Elliptical Helix)

## 1. Trajectory Equation
The position is given by:

$$
\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)
$$

By eliminating $t$ using the trigonometric identity $\cos^2 \theta + \sin^2 \theta = 1$, we find the projection on the $xy$-plane:

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1
$$

Since $z$ increases linearly with $t$, the trajectory is an **elliptical helix**.

## 2. Path Length Calculation
The velocity vector is:

$$
\vec{v}(t) = (-a\omega \sin(\omega t), b\omega \cos(\omega t), b)
$$

The path length $s$ from $t=0$ to $t=t_0$ is:

$$
s = \int_{0}^{t_0} \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2} dt
$$

In the special case where $a = b$, the speed is constant, and the length is:

$$
s = t_0 \cdot b\sqrt{\omega^2 + 1}
$$

## 3. Special Cases
- **Circular Helix:** $a = b$
- **Planar Ellipse:** $b = 0$ (no vertical motion)
