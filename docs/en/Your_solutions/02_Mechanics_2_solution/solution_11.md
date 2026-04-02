# Physics: Motion from a Changing Force in 3D Space

In this problem, we have an object moving in 3D space, meaning it moves in three directions at once: $x$ (left/right), $y$ (up/down), and $z$ (forward/backward). The force pushing it changes as time passes, which means its acceleration, velocity, and position are all changing constantly.

We will break this down into three separate dimensions and use a little bit of calculus (integration) to go from Force to Velocity, and then from Velocity to Position.

## 1. Necessary Definitions & The Calculus "Integral"

* **Vector $(x, y, z)$:** A way of organizing 3D numbers. Instead of writing three long sentences, physicists group the three directions into brackets. For example, a position of $(5, 2, -3)$ means $5$ meters in the $x$ direction, $2$ meters in the $y$ direction, and $-3$ meters in the $z$ direction.
* **Mass ($m$):** How heavy the object is.
* **Force ($F$):** A push or a pull.
* **Acceleration ($a$):** How fast your speed is changing.
* **Velocity ($v$):** How fast your position is changing.
* **Position ($r$):** Where you are located in space.
* **Initial Conditions ($r_0$ and $v_0$):** Exactly where the object is and how fast it is moving at the moment the stopwatch starts (time $t = 0$).

### The Calculus Crash Course: Integrals
Because the force is constantly changing, we have to use an **integral** ($\int$) to add up those changes over time. Taking an integral is the exact opposite of taking a derivative. 

**The Reverse Power Rule:**
If you have a term with time ($t$) and an exponent ($n$), like $A t^n$, to find the integral you:
1. **Add 1** to the exponent.
2. **Divide** the big number in front by the new exponent.

*Example:* The integral of $15t$ (which is $15t^1$) becomes $\frac{15}{2}t^2 = 7.5t^2$. 

*Important Note:* Whenever you take an integral, you must add a "Constant" ($C$) at the end. This is where our Initial Conditions come in to help us figure out exactly what $C$ is!

## 2. The Master Formulas

**1. Newton's Second Law:**
Force equals mass times acceleration. We can rearrange this to find acceleration by dividing Force by mass.

$$
a = \frac{F}{m}
$$

**2. From Acceleration to Velocity:**
Velocity is the integral of acceleration over time ($t$).

$$
v(t) = \int a(t) \, dt
$$

**3. From Velocity to Position:**
Position is the integral of velocity over time ($t$).

$$
r(t) = \int v(t) \, dt
$$

---

## Step-by-Step Solution

**What we know:**
* Mass: $m = 3 \text{ kg}$
* Force in 3D: $F = (15t, 3t - 12, -6t^2)$
* Starting position ($t=0$): $r_0 = (5, 2, -3)$
* Starting velocity ($t=0$): $v_0 = (2, 0, 1)$

### Step 1: Find the Acceleration ($a$)

To find acceleration, we divide the force by the mass. Since the mass is $3$, we divide every single piece of the force vector by $3$.

* **X-Acceleration ($a_x$):** $\frac{15t}{3}$
* **Y-Acceleration ($a_y$):** $\frac{3t - 12}{3}$
* **Z-Acceleration ($a_z$):** $\frac{-6t^2}{3}$

Simplifying these gives us our acceleration vector:

$$
a(t) = (5t, \, t - 4, \, -2t^2)
$$

---

### Step 2: Find the Velocity ($v$)

Velocity is the integral of acceleration. We will use the reverse power rule on each piece of our acceleration vector.

* **X-Velocity ($v_x$):** The integral of $5t$.
  * Exponent goes from $1$ to $2$. Divide $5$ by $2$.
  * $v_x = 2.5t^2 + C_x$
  * *Find $C_x$:* At $t=0$, the initial x-velocity ($v_{0x}$) is $2$. If we plug $0$ in for $t$, we get $v_x = 0 + C_x = 2$. So, $C_x = 2$.

$$
v_x(t) = 2.5t^2 + 2
$$

* **Y-Velocity ($v_y$):** The integral of $t - 4$.
  * For $t$: exponent goes from $1$ to $2$. Divide $1$ by $2$.
  * For $-4$: just attach a $t$ to it (it becomes $-4t$).
  * $v_y = 0.5t^2 - 4t + C_y$
  * *Find $C_y$:* At $t=0$, the initial y-velocity ($v_{0y}$) is $0$. Plugging in $0$ gives $C_y = 0$.

$$
v_y(t) = 0.5t^2 - 4t
$$

* **Z-Velocity ($v_z$):** The integral of $-2t^2$.
  * Exponent goes from $2$ to $3$. Divide $-2$ by $3$.
  * $v_z = -\frac{2}{3}t^3 + C_z$
  * *Find $C_z$:* At $t=0$, the initial z-velocity ($v_{0z}$) is $1$. Plugging in $0$ gives $C_z = 1$.

$$
v_z(t) = -\frac{2}{3}t^3 + 1
$$

**Answer 1 (Velocity Dependence):**
Grouping them back into a vector, the velocity of the particle is:

$$
v(t) = \left( 2.5t^2 + 2, \,\, 0.5t^2 - 4t, \,\, -\frac{2}{3}t^3 + 1 \right) \text{ m/s}
$$

---

### Step 3: Find the Position ($r$)

Position is the integral of velocity. We do the exact same process again, integrating the velocity formulas we just found.

* **X-Position ($r_x$):** The integral of $2.5t^2 + 2$.
  * For $2.5t^2$: exponent becomes $3$. Divide $2.5$ by $3$ (which is $\frac{2.5}{3}$ or $\frac{5}{6}$).
  * For $2$: attach a $t$.
  * $r_x = \frac{5}{6}t^3 + 2t + C_x$
  * *Find $C_x$:* At $t=0$, initial x-position is $5$. So, $C_x = 5$.

$$
r_x(t) = \frac{5}{6}t^3 + 2t + 5
$$

* **Y-Position ($r_y$):** The integral of $0.5t^2 - 4t$.
  * For $0.5t^2$: exponent becomes $3$. Divide $0.5$ by $3$ (which is $\frac{0.5}{3}$ or $\frac{1}{6}$).
  * For $-4t$: exponent becomes $2$. Divide $-4$ by $2$ to get $-2$. 
  * $r_y = \frac{1}{6}t^3 - 2t^2 + C_y$
  * *Find $C_y$:* At $t=0$, initial y-position is $2$. So, $C_y = 2$.

$$
r_y(t) = \frac{1}{6}t^3 - 2t^2 + 2
$$

* **Z-Position ($r_z$):** The integral of $-\frac{2}{3}t^3 + 1$.
  * For $-\frac{2}{3}t^3$: exponent becomes $4$. Divide $-\frac{2}{3}$ by $4$ (which is $-\frac{2}{12}$ or $-\frac{1}{6}$).
  * For $1$: attach a $t$.
  * $r_z = -\frac{1}{6}t^4 + t + C_z$
  * *Find $C_z$:* At $t=0$, initial z-position is $-3$. So, $C_z = -3$.

$$
r_z(t) = -\frac{1}{6}t^4 + t - 3
$$

**Answer 2 (Position Dependence):**
Grouping them back into a vector, the exact position of the particle at any time $t$ is:

$$
r(t) = \left( \frac{5}{6}t^3 + 2t + 5, \,\, \frac{1}{6}t^3 - 2t^2 + 2, \,\, -\frac{1}{6}t^4 + t - 3 \right) \text{ meters}
$$
