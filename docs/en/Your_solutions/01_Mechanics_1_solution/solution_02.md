# Proof: Maximum Range of a Projectile

## 1. Initial Formulas
The horizontal and vertical components of the initial velocity $v_0$ are:

$$
v_x = v_0 \cos(\theta)
$$

$$
v_y = v_0 \sin(\theta)
$$

## 2. Deriving the Range Formula
The time of flight $t$ is determined by the vertical motion:

$$
t = \frac{2 v_0 \sin\theta}{g}
$$

The range $R$ is the horizontal distance traveled:

$$
R = v_x \cdot t = (v_0 \cos\theta) \left( \frac{2 v_0 \sin\theta}{g} \right)
$$

Using the double-angle identity $2 \sin\theta \cos\theta = \sin(2\theta)$:

$$
R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}
$$

## 3. Finding the Maximum Angle
To maximize $R(\theta)$, we must maximize $\sin(2\theta)$. 
The maximum value of the sine function is $1$, which occurs at $90^\circ$.

$$
\sin(2\theta) = 1 \implies 2\theta = 90^\circ
$$

$$
\theta = 45^\circ
$$

**Conclusion:** For any given initial velocity, the maximum horizontal range is achieved at a launch angle of $45^\circ$.
