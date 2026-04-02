# Physics: Momentum and Kinetic Energy

Welcome back! This problem is a fantastic way to understand how objects interact when they crash into or join each other. When the runner jumps onto the cart, we are looking at something physicists call an **inelastic collision**. 

Let's break down the basic definitions and formulas before we do any math.

## 1. Necessary Definitions

* **Momentum ($p$):** Think of this as "mass in motion." It is a measurement of how hard it is to stop a moving object. A heavy truck moving slowly has a lot of momentum, and a tiny bullet moving very fast also has a lot of momentum. 
* **Conservation of Momentum:** A fundamental rule of the universe. It states that in a closed system (ignoring outside friction like wind resistance), the total momentum *before* an event is exactly equal to the total momentum *after* the event.
* **Perfectly Inelastic Collision:** A specific type of event where two separate objects collide, stick together, and continue moving as one single combined mass.
* **Kinetic Energy ($KE$):** The energy of actual motion. If something is moving, it has kinetic energy. If it is sitting perfectly still, its kinetic energy is zero.

## 2. The Master Formulas

**1. Momentum ($p$):**
Momentum is simply an object's mass ($m$) multiplied by its velocity or speed ($v$).

$$
p = m \cdot v
$$

**2. The Inelastic Collision Formula:**
Because momentum is conserved, the momentum of Object 1 plus the momentum of Object 2 before they meet must equal the momentum of their combined mass after they stick together.

$$
m_1v_1 + m_2v_2 = (m_1 + m_2)v_{final}
$$

**3. Kinetic Energy ($KE$):**
Depends on the mass ($m$) and the square of the velocity ($v^2$).

$$
KE = \frac{1}{2}mv^2
$$

---

## Part 1: Finding the Final Speed

**The Question:** A **70 kg** runner moving at **3 m/s** jumps onto a **140 kg** stationary cart. What is the final speed of the cart with the runner?

**Step 1: Write down what we know.**
* Mass of the runner ($m_1$) = **70 kg**
* Speed of the runner ($v_1$) = **3 m/s**
* Mass of the cart ($m_2$) = **140 kg**
* Speed of the cart ($v_2$) = **0 m/s** (because the problem says it is stationary)

**Step 2: Set up the Momentum Conservation equation.**
We use our inelastic collision formula from earlier:

$$
m_1v_1 + m_2v_2 = (m_1 + m_2)v_{final}
$$

**Step 3: Plug in our numbers.**

$$
(70 \cdot 3) + (140 \cdot 0) = (70 + 140) \cdot v_{final}
$$

**Step 4: Do the math step-by-step.**
First, let's calculate the left side of the equation (the momentum before the jump). The cart isn't moving, so its initial momentum is zero ($140 \cdot 0 = 0$). The runner's momentum is $70 \cdot 3 = 210$.

$$
210 + 0 = (70 + 140) \cdot v_{final}
$$

$$
210 = 210 \cdot v_{final}
$$

Now, we need to get $v_{final}$ completely by itself. We do this by dividing both sides by **210**.

$$
v_{final} = \frac{210}{210}
$$

$$
v_{final} = 1 \text{ m/s}
$$

**Answer 1:** The final speed of the cart with the runner on it is **1 m/s**. (Notice how adding the mass of the cart slowed the runner's forward speed down significantly!)

---

## Part 2: Is Kinetic Energy Conserved?

**The Question:** Is kinetic energy conserved in this collision? Explain.

To find out if kinetic energy is conserved (meaning the total energy stayed exactly the same), we have to calculate the total Kinetic Energy *before* the jump and compare it to the total Kinetic Energy *after* the jump.

**Step 1: Calculate the Kinetic Energy BEFORE the jump.**
Only the runner is moving, so only the runner has kinetic energy. 

$$
KE_{before} = \frac{1}{2}m_1v_1^2
$$

$$
KE_{before} = \frac{1}{2} \cdot 70 \cdot 3^2
$$

First, square the velocity ($3 \cdot 3 = 9$).

$$
KE_{before} = \frac{1}{2} \cdot 70 \cdot 9
$$

Half of 70 is 35, and $35 \cdot 9 = 315$.

$$
KE_{before} = 315 \text{ Joules}
$$

**Step 2: Calculate the Kinetic Energy AFTER the jump.**
Now, the runner and the cart are moving together as one big object. 
* Combined mass = $70 + 140 = 210 \text{ kg}$
* Final speed = **1 m/s**

$$
KE_{after} = \frac{1}{2}m_{total}v_{final}^2
$$

$$
KE_{after} = \frac{1}{2} \cdot 210 \cdot 1^2
$$

Since $1^2$ is just 1:

$$
KE_{after} = \frac{1}{2} \cdot 210 \cdot 1
$$

$$
KE_{after} = 105 \text{ Joules}
$$

**Step 3: Compare and Explain.**
* Energy Before: **315 Joules**
* Energy After: **105 Joules**

**Answer 2:** **No, kinetic energy is NOT conserved.** **Explanation:** We started with 315 Joules of kinetic energy and ended up with only 105 Joules. **210 Joules** of kinetic energy "disappeared" from the motion of the system. 

Where did it go? The Conservation of Energy says energy can't be destroyed, only transformed. In all inelastic collisions (like a runner landing on a cart, or two cars crashing), the "lost" kinetic energy is transformed into other forms of energy. In this case, it was transformed into the sound of the runner's shoes hitting the cart, vibrations traveling through the wheels, a tiny bit of heat generated by the impact, and the friction of the runner sliding slightly to a halt on the surface of the cart.
