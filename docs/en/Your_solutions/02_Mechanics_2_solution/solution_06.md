# The Physics of a Bouncing Ball: Energy Loss

Welcome back! This is a really fun problem because it describes something we've all seen in real life: a bouncing ball that doesn't bounce quite as high as where it started. 

In the real world, "Conservation of Energy" still applies, but the energy doesn't all stay inside the ball. When the ball hits the ground, some of its energy escapes as the "smack" sound you hear, and some turns into a tiny bit of heat from the friction of the rubber squishing against the floor. 

Let's break down the definitions and formulas you need to solve this.

## 1. Necessary Definitions

* **Mechanical Energy ($E$):** This is the total amount of "useful" energy the ball has. For a falling ball, it is a combination of its height (Potential Energy) and its movement (Kinetic Energy).
* **Potential Energy ($PE$):** Energy based on height. At the very top of its bounce, right before it starts falling back down, the ball stops moving for a split second. At this exact moment, 100% of its Mechanical Energy is just Potential Energy.
* **Energy Loss:** The problem says the ball *loses* 30% of its energy on each bounce. This means we have to focus on what it *keeps*. If it loses 30%, it keeps exactly 70% of its energy for the next bounce.

## 2. The Master Formulas

**1. Potential Energy ($PE$):**
Depends on mass ($m$), gravitational acceleration ($g$), and height ($h$). 

$$
PE = mgh
$$

**2. Calculating Energy After a Bounce:**
If $E_{old}$ is the energy before the bounce, the new energy ($E_{new}$) is just 70% of that (which we write as 0.70 in math).

$$
E_{new} = 0.70 \cdot E_{old}
$$

---

## The Problem

A tennis ball is dropped from a height of 2.0 m. After each bounce, it loses 30% of its mechanical energy. To what height does it rise after the second bounce?

### Step-by-Step Solution:

**Step 1: Write down what we know.**
* Initial height ($h_0$) = 2.0 meters
* Energy retained per bounce = 70% (or 0.70)
* Mass of the ball ($m$) = ? *(Don't worry, just like in previous problems, we will see this magically cancel out!)*
* Gravity ($g$) $\approx 9.81 \text{ m/s}^2$

**Step 2: Understand the Initial Energy.**
Before the ball is dropped, it is being held perfectly still at 2.0 meters high. That means all of its initial mechanical energy ($E_0$) is Potential Energy.

$$
E_0 = m \cdot g \cdot h_0
$$

**Step 3: Calculate the energy after the FIRST bounce.**
The ball hits the floor and loses 30%. It keeps 70%. So, the energy it has to climb back up into the air ($E_1$) is:

$$
E_1 = 0.70 \cdot E_0
$$

**Step 4: Calculate the energy after the SECOND bounce.**
The ball falls again, hits the floor a second time, and loses *another* 30% of whatever energy it had left. It keeps 70% of $E_1$. Let's call this energy after the second bounce $E_2$:

$$
E_2 = 0.70 \cdot E_1
$$

Since we know $E_1$ is actually $0.70 \cdot E_0$, we can put that inside:

$$
E_2 = 0.70 \cdot (0.70 \cdot E_0)
$$

Multiply $0.70 \cdot 0.70$ and you get $0.49$. This means after two bounces, the ball only has 49% of the total energy it started with!

$$
E_2 = 0.49 \cdot E_0
$$

**Step 5: Translate that remaining energy back into height.**
At the top of the second bounce, all of that $E_2$ energy is pure Potential Energy again. Let's call this new peak height $h_2$. Let's write out the full equations using the $PE$ formula:

The energy at the top of bounce 2:
$$
E_2 = m \cdot g \cdot h_2
$$

The very first energy it started with:
$$
E_0 = m \cdot g \cdot h_0
$$

Now, plug both of those into our equation from Step 4 ($E_2 = 0.49 \cdot E_0$):

$$
m \cdot g \cdot h_2 = 0.49 \cdot (m \cdot g \cdot h_0)
$$

**Step 6: Simplify and Solve!**
Look at the equation above. We have mass ($m$) and gravity ($g$) on the left side, and mass ($m$) and gravity ($g$) on the right side. If we divide both sides by $(m \cdot g)$, they completely cancel out! 

This tells us something amazing: *the height a ball bounces back to doesn't depend on how heavy it is, or even what planet it is bouncing on!* It only depends on the dropping height and the energy loss.

$$
h_2 = 0.49 \cdot h_0
$$

Finally, we plug in our starting height of 2.0 meters:

$$
h_2 = 0.49 \cdot 2.0
$$

$$
h_2 = 0.98 \text{ meters}
$$

**Answer:** After the second bounce, the tennis ball will rise to a height of **0.98 meters** (or 98 centimeters).
