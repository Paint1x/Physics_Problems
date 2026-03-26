# Projectile Motion Physics Problem

## Problem Statement
A projectile is fired with $v_0 = 100 \text{ m/s}$ at $\theta = 37^\circ$. 
Assume $g = 9.8 \text{ m/s}^2$ and ignore air resistance.

---

## 1. Differential Equations of Motion
Using Newton's Second Law ($F = ma$), where the only force is gravity acting vertically downward:

**Horizontal Direction:**

$$
\frac{d^2x}{dt^2} = 0
$$

**Vertical Direction:**

$$
\frac{d^2y}{dt^2} = -g
$$

---

## 2. Time of Flight ($t$)
The projectile hits the ground when vertical displacement $y = 0$.

$$
y(t) = (v_0 \sin\theta)t - \frac{1}{2}gt^2 = 0
$$

Solving for $t$:

$$
t = \frac{2 v_0 \sin\theta}{g} = \frac{2(100)(0.6)}{9.8} \approx 12.24 \text{ s}
$$

---

## 3. Maximum Height ($H$)
Occurs when vertical velocity $v_y = 0$.

$$
H = \frac{(v_0 \sin\theta)^2}{2g} = \frac{60^2}{2(9.8)} \approx 183.67 \text{ m}
$$

---

## 4. Range ($R$)
Total horizontal distance covered during the time of flight.

$$
R = (v_0 \cos\theta) \times t = 80 \times 12.24 \approx 979.2 \text{ m}
$$
