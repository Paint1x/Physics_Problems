# Motion Analysis: Parametric Path Solution

## 1. Path Equations
The object's position is given by:

$$
x(t) = 2t^2, \qquad y(t) = 3t^3
$$

## 2. Eliminating the Parameter $t$
Solving for $t$ in terms of $x$:

$$
t = \sqrt{\frac{x}{2}}
$$

Substituting into the $y$ equation:

$$
y = 3\left(\frac{x}{2}\right)^{3/2}
$$

## 3. Velocity Analysis
Velocity is the derivative of position: $\vec{v}(t) = (\frac{dx}{dt}, \frac{dy}{dt})$.

$$
\vec{v}(t) = (4t)\hat{i} + (9t^2)\hat{j}
$$

Magnitude (Speed):

$$
|\vec{v}(t)| = \sqrt{16t^2 + 81t^4}
$$

## 4. Acceleration Analysis
Acceleration is the derivative of velocity: $\vec{a}(t) = (\frac{dv_x}{dt}, \frac{dv_y}{dt})$.

$$
\vec{a}(t) = 4\hat{i} + (18t)\hat{j}
$$

Magnitude:

$$
|\vec{a}(t)| = \sqrt{16 + 324t^2}
$$

## 5. Conclusion
The acceleration is **not constant** because the vertical component $18t$ changes as time $t$ progresses.
