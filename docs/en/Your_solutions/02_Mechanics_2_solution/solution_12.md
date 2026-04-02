# Physics: 2D Motion, Work, and Energy

Welcome to 2D physics! This problem is a fantastic step up because it takes the concepts you've been learning (force, velocity, position, work, and energy) and applies them to two dimensions at the same time: the **X-direction** (left/right) and the **Y-direction** (up/down). 

Don't worry about the extra dimension; the secret to 2D physics is that **the X and Y directions are completely independent**. What happens horizontally doesn't affect what happens vertically. We just solve the problem twice side-by-side!

Here are all the concepts and formulas you need to know before we begin.

## 1. Necessary Definitions & Math Tools

* **Vectors (written with an arrow, like $\vec{v}$ or in brackets $[x, y]$):** A vector is just a package of two numbers. It tells you "how much horizontal" and "how much vertical." For example, a force vector $\vec{F} = [6, 2]$ means the force pushes with **6 N** to the right and **2 N** upward.
* **Vector Math:** To add or subtract vectors, you just do the math on the X's together, and the Y's together. To multiply a vector by a normal number, multiply both parts by that number.
* **Dot Product ($\cdot$):** A special way to multiply two vectors together to get a single normal number. You multiply their X parts, multiply their Y parts, and add the results together: 
    $A \cdot B = (A_x \cdot B_x) + (A_y \cdot B_y)$
* **Acceleration ($\vec{a}$):** How fast your velocity is changing.
* **Velocity ($\vec{v}$):** How fast your position is changing.
* **Position ($\vec{r}$):** Your exact coordinates on a graph.
* **Work ($W$):** The total energy pushed into the object by a force. It is the dot product of Force and Displacement (change in position). Measured in Joules (J).
* **Kinetic Energy ($KE$):** The energy of motion. Measured in Joules (J).
* **Work-Energy Theorem:** A fundamental rule of the universe. It states that the total Work done on an object is exactly equal to its change in Kinetic Energy. If you do **50 J** of work on an object, its kinetic energy increases by exactly **50 J**.

## 2. The Master Formulas

**1. Newton's Second Law:**
Force equals mass times acceleration.

$$
\vec{a} = \frac{\vec{F}}{m}
$$

**2. Kinematics (Since acceleration is constant):**
To get velocity, we multiply acceleration by time ($t$) and add the starting velocity ($\vec{v}_0$).

$$
\vec{v}(t) = \vec{a} \cdot t + \vec{v}_0
$$

To get position, we integrate velocity over time. 

$$
\vec{r}(t) = \frac{1}{2}\vec{a}t^2 + \vec{v}_0 t + \vec{r}_0
$$

**3. Work ($W$):**
Force dotted with the change in position ($\Delta \vec{r}$).

$$
W = \vec{F} \cdot \Delta \vec{r}
$$

**4. Kinetic Energy ($KE$):**
Depends on mass ($m$) and the actual speed squared. For a vector, speed squared ($|\vec{v}|^2$) is just $v_x^2 + v_y^2$.

$$
KE = \frac{1}{2}m(v_x^2 + v_y^2)
$$

---

## Step-by-Step Solution

**The Setup:**
* Mass: **2 kg**
* Force: $\vec{F} = [6, 2]$ N
* Initial Velocity ($t=0$): $\vec{v}(0) = [1, -1]$ m/s
* Initial Position ($t=0$): $\vec{r}(0) = [0, 0]$ m

### Part 1: Determine $\vec{a}(t)$

To find the acceleration, we use Newton's Second Law. We just divide the Force vector by the mass.

$$
\vec{a} = \frac{[6, 2]}{2}
$$

Divide both the X and the Y parts by 2:

$$
\vec{a}(t) = [3, 1]\ \text{m/s}^2
$$

*Explanation: The acceleration is constant. Every second, the X-velocity increases by 3, and the Y-velocity increases by 1.*

---

### Part 2: Determine $\vec{v}(t)$

Now we use our velocity formula. We plug in our acceleration $[3, 1]$ and our initial velocity $[1, -1]$.

$$
\vec{v}(t) = [3, 1]t + [1, -1]
$$

Distribute the $t$ into the first bracket:

$$
\vec{v}(t) = [3t, 1t] + [1, -1]
$$

Now, add the X's together and the Y's together to get one single equation:

$$
\vec{v}(t) = [3t + 1, t - 1]\ \text{m/s}
$$

---

### Part 3: Determine $\vec{r}(t)$

We use our position formula. We plug in acceleration $[3, 1]$, initial velocity $[1, -1]$, and since the initial position is just $[0, 0]$, we can ignore it!

$$
\vec{r}(t) = \frac{1}{2}[3, 1]t^2 + [1, -1]t + [0, 0]
$$

Distribute the $\frac{1}{2}t^2$ into the first bracket, and the $t$ into the second bracket:

$$
\vec{r}(t) = [1.5t^2, 0.5t^2] + [t, -t]
$$

Add the X's together and the Y's together:

$$
\vec{r}(t) = [1.5t^2 + t, 0.5t^2 - t]\ \text{m}
$$

---

### Part 4: Draw the trajectory of the motion



If you were to draw this on graph paper:
1.  Draw a standard X and Y axis.
2.  Start your line at the origin $(0,0)$.
3.  Notice that at $t=1$, the position is $X = 2.5$, $Y = -0.5$. The particle initially dips down a little bit because of that negative starting Y-velocity!
4.  At $t=2$, $X = 8$, $Y = 0$. It crosses back up through the X-axis.
5.  At $t=3$, $X = 16.5$, $Y = 1.5$. It is now climbing upward and far to the right.
6.  **The Shape:** Because both $X$ and $Y$ have a $t^2$ in their equations, the path is a smooth, curving **parabola** that sweeps out to the right and eventually curls upwards.

---

### Part 5: Calculate the work done by the force at time $t = 3\ \text{s}$

To find the Work done, we first need to know exactly how far the particle travelled. We need its position at exactly **3 seconds**.

Let's plug $t=3$ into the position formula from Part 3:
* $X(3) = 1.5(3^2) + 3 = 1.5(9) + 3 = 13.5 + 3 = 16.5$
* $Y(3) = 0.5(3^2) - 3 = 0.5(9) - 3 = 4.5 - 3 = 1.5$

So, the displacement $\Delta \vec{r}$ is $[16.5, 1.5]$ meters.

Now, we calculate Work using the Dot Product formula ($W = \vec{F} \cdot \Delta \vec{r}$).
Our force is $[6, 2]$ and our displacement is $[16.5, 1.5]$.

$$
W = (F_x \cdot X) + (F_y \cdot Y)
$$

$$
W = (6 \cdot 16.5) + (2 \cdot 1.5)
$$

$$
W = 99 + 3
$$

$$
W = 102\ \text{Joules}
$$

---

### Part 6: Check the consistency with the work-energy theorem

The theorem states that the Work done (**102 J**) must exactly equal the change in Kinetic Energy. Let's calculate the Kinetic Energy at the very beginning and at $t=3$ to see if this is true!

**Step A: Initial Kinetic Energy (at $t=0$)**
* Initial velocity: $\vec{v}(0) = [1, -1]$
* Velocity squared: $v_x^2 + v_y^2 = (1^2) + (-1^2) = 1 + 1 = 2$

$$
KE_{start} = \frac{1}{2}m(v^2) = \frac{1}{2}(2)(2) = 2\ \text{Joules}
$$

**Step B: Final Kinetic Energy (at $t=3$)**
First, we need the velocity at 3 seconds. Let's plug $t=3$ into our velocity formula from Part 2:
* $\vec{v}(3) = [3(3) + 1, 3 - 1] = [10, 2]$
* Velocity squared: $v_x^2 + v_y^2 = (10^2) + (2^2) = 100 + 4 = 104$

$$
KE_{final} = \frac{1}{2}m(v^2) = \frac{1}{2}(2)(104) = 104\ \text{Joules}
$$

**Step C: The Comparison**
The change in kinetic energy ($\Delta KE$) is the Final minus the Start:

$$
\Delta KE = 104 - 2 = 102\ \text{Joules}
$$

**Conclusion:**
The calculated Work is **102 J**, and the change in Kinetic Energy is exactly **102 J**. 

$$
102\ \text{J} = 102\ \text{J}
$$

The results are perfectly consistent with the Work-Energy theorem!
