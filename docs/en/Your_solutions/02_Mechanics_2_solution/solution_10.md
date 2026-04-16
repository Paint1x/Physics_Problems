## 10. Force field and power

In a certain force field, the equations of motion of a particle with mass $m=0.5$ kg are as follows:

$$
x = 5t^2 - t, \quad y = 2t^3, \quad z = -3t + 2
$$

Find the time dependence of: the particle's velocity, the particle's momentum, the particle's acceleration, the force acting on the particle, and the power transferred by the field to the particle.

## 1. The Calculus Crash Course: The "Power Rule"

To solve this, you need a tiny bit of calculus. Specifically, you need to know how to take a **derivative**. A derivative is just a mathematical tool that finds the "rate of change." For example, how fast your position changes is your velocity.

Here is the only rule you need to know to take a derivative, called the **Power Rule**:
If you have a term with time ($t$) and an exponent ($n$), like this: $A t^n$
The derivative is found by multiplying the main number by the exponent, and then subtracting 1 from the exponent: $n \cdot A t^{n-1}$

**Examples:**
* The derivative of $5t^2$ is $(2 \cdot 5)t^1 = 10t$
* The derivative of $2t^3$ is $(3 \cdot 2)t^2 = 6t^2$
* The derivative of a plain $t$ (which is $1t^1$) is just $1$.
* The derivative of a plain number with no $t$ (like $2$) is always $0$, because a constant number never changes!

## 2. Necessary Definitions & Formulas

* **Position ($x, y, z$):** Where the particle is located in space.
* **Velocity ($v$):** How fast position is changing. It is the derivative of position. 
* **Momentum ($p$):** How hard it is to stop the moving particle. 

$$
p = m \cdot v
$$

* **Acceleration ($a$):** How fast the velocity is changing (speeding up or slowing down). It is the derivative of velocity.
* **Force ($F$):** A push or pull. According to Newton's Second Law, Force is mass times acceleration.

$$
F = m \cdot a
$$

* **Power ($P$):** How much energy the force is pumping into the particle every second. It is calculated using a "Dot Product" (multiplying the Force and Velocity of each direction together and adding them up).

$$
P = (F_x \cdot v_x) + (F_y \cdot v_y) + (F_z \cdot v_z)
$$

---

## Step-by-Step Solution

**The Setup:**
We are given the mass ($m = 0.5 \text{ kg}$) and the position equations for $x$, $y$, and $z$:
* $x(t) = 5t^2 - t$
* $y(t) = 2t^3$
* $z(t) = -3t + 2$

### Step 1: Find the Velocity ($v$)
Velocity is the derivative of position. We will use the power rule on our position equations to find the velocity in all three directions.

* **X-Velocity ($v_x$):** The derivative of $5t^2 - t$

$$
v_x = 10t - 1
$$

* **Y-Velocity ($v_y$):** The derivative of $2t^3$

$$
v_y = 6t^2
$$

* **Z-Velocity ($v_z$):** The derivative of $-3t + 2$ (the $t$ becomes $1$, and the $2$ disappears)

$$
v_z = -3
$$

**Answer 1 (Velocity):** The velocity equations are $v_x = 10t - 1$, $v_y = 6t^2$, and $v_z = -3$.

---

### Step 2: Find the Momentum ($p$)
Momentum is simply mass multiplied by velocity. Our mass is $0.5$ kg. We just multiply each of our velocity answers by $0.5$.

* **X-Momentum ($p_x$):** $0.5 \cdot (10t - 1)$

$$
p_x = 5t - 0.5
$$

* **Y-Momentum ($p_y$):** $0.5 \cdot (6t^2)$

$$
p_y = 3t^2
$$

* **Z-Momentum ($p_z$):** $0.5 \cdot (-3)$

$$
p_z = -1.5
$$

**Answer 2 (Momentum):** The momentum equations are $p_x = 5t - 0.5$, $p_y = 3t^2$, and $p_z = -1.5$.

---

### Step 3: Find the Acceleration ($a$)
Acceleration is the derivative of velocity. We look back at our answers from Step 1 and use the Power Rule on them.

* **X-Acceleration ($a_x$):** The derivative of $10t - 1$

$$
a_x = 10
$$

* **Y-Acceleration ($a_y$):** The derivative of $6t^2$

$$
a_y = 12t
$$

* **Z-Acceleration ($a_z$):** The derivative of $-3$. (Since there is no $t$, it is a constant, so the derivative is zero!)

$$
a_z = 0
$$

**Answer 3 (Acceleration):** The acceleration equations are $a_x = 10$, $a_y = 12t$, and $a_z = 0$.

---

### Step 4: Find the Force ($F$)
Newton's Second Law says Force is mass multiplied by acceleration ($F = m \cdot a$). Just like we did with momentum, we multiply our acceleration answers by our mass ($0.5$).

* **X-Force ($F_x$):** $0.5 \cdot 10$

$$
F_x = 5
$$

* **Y-Force ($F_y$):** $0.5 \cdot 12t$

$$
F_y = 6t
$$

* **Z-Force ($F_z$):** $0.5 \cdot 0$

$$
F_z = 0
$$

**Answer 4 (Force):** The force equations are $F_x = 5$, $F_y = 6t$, and $F_z = 0$.

---

### Step 5: Find the Power ($P$)
Power is the Force multiplied by the Velocity. Since these are in 3D space, we multiply the $X$'s together, the $Y$'s together, and the $Z$'s together, and then add the whole thing up into one single equation.

$$
P = (F_x \cdot v_x) + (F_y \cdot v_y) + (F_z \cdot v_z)
$$

Let's plug in the answers we found in Step 4 and Step 1:

$$
P = \left(5 \cdot (10t - 1)\right) + \left(6t \cdot 6t^2\right) + \left(0 \cdot -3\right)
$$

Now, let's do the algebra to simplify:
* The $X$ part: $5 \cdot 10t = 50t$, and $5 \cdot -1 = -5$. So, $50t - 5$.
* The $Y$ part: $6 \cdot 6 = 36$, and $t \cdot t^2 = t^3$. So, $36t^3$.
* The $Z$ part: $0 \cdot -3 = 0$.

Add them all together:

$$
P = 50t - 5 + 36t^3
$$

*(We usually write formulas with the biggest exponents first to make them look neat)*

$$
P = 36t^3 + 50t - 5
$$

**Answer 5 (Power):** The power transferred by the field to the particle is **$36t^3 + 50t - 5$**.
