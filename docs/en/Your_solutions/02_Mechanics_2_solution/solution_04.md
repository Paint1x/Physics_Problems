# Physics: Energy and Collisions

Welcome to a classic physics problem! This scenario combines two major physics concepts into one seamless event: first, a block sliding down a hill (Energy), and second, that block crashing into another block (Momentum). 

Because you are starting from scratch, we will break this down into two distinct parts and introduce all the definitions and formulas you need.

## 1. Necessary Definitions

* **Potential Energy ($PE$):** Energy stored by an object based on its height. The higher the block is, the more potential energy it has.
* **Kinetic Energy ($KE$):** The energy of motion. As the block slides down the track, it loses height (losing $PE$) and gains speed (gaining $KE$).
* **Conservation of Energy:** In a frictionless system, energy cannot be lost. All the stored height energy at the top of the track turns exactly into motion energy at the bottom.
* **Momentum ($p$):** A measurement of how hard it is to stop a moving object. It depends on how heavy the object is and how fast it is moving.
* **Conservation of Momentum:** When two objects collide, the total momentum before the crash is exactly equal to the total momentum after the crash. 
* **Perfectly Inelastic Collision:** A specific type of crash where two objects hit each other and stick together, moving as one combined mass afterwards.

## 2. The Master Formulas

**1. Potential Energy ($PE$):**
Depends on mass ($m$), gravitational acceleration ($g \approx 9.81 \text{ m/s}^2$), and height ($h$).

$$
PE = mgh
$$

**2. Kinetic Energy ($KE$):**
Depends on mass ($m$) and velocity/speed ($v$).

$$
KE = \frac{1}{2}mv^2
$$

**3. Momentum ($p$):**
Just mass multiplied by velocity.

$$
p = mv
$$

**4. Inelastic Collision Formula:**
Since momentum is conserved, the momentum of Block 1 plus the momentum of Block 2 before the crash equals the momentum of their combined mass after the crash.

$$
m_1v_1 + m_2v_2 = (m_1 + m_2)v_{final}
$$

---

## The Problem

A 0.5 kg block slides down a frictionless track from a height of 3.0 m. At the bottom, it collides and sticks to a 1.5 kg block, which is initially at rest. What is the speed of the combined mass just after the collision?

### Part 1: Sliding Down the Track

Before we can look at the crash, we need to know how fast the first block is moving when it reaches the bottom of the track. We use **Conservation of Energy** for this.

**Step 1: Write down what we know for Block 1.**
* Mass ($m_1$) = $0.5 \text{ kg}$
* Starting height ($h$) = $3.0 \text{ m}$
* Gravity ($g$) $\approx 9.81 \text{ m/s}^2$

**Step 2: Set up the Energy Conservation equation.**
At the very top, the block has only Potential Energy. At the very bottom, it has completely turned into Kinetic Energy.

$$
PE_{\text{top}} = KE_{\text{bottom}}
$$

Let's plug in the formulas for those:

$$
m_1gh = \frac{1}{2}m_1v_1^2
$$

**Step 3: Simplify the equation.**
Notice that mass ($m_1$) is on both sides of the equals sign. Just like in pendulum problems, if we divide both sides by mass, it cancels out! The speed at the bottom doesn't depend on how heavy the sliding block is.

$$
gh = \frac{1}{2}v_1^2
$$

Multiply both sides by 2 to get the $v_1^2$ by itself:

$$
2gh = v_1^2
$$

Take the square root to solve for velocity ($v_1$):

$$
v_1 = \sqrt{2gh}
$$

**Step 4: Plug in the numbers to find the speed at the bottom.**

$$
v_1 = \sqrt{2 \cdot 9.81 \cdot 3.0}
$$

$$
v_1 = \sqrt{58.86}
$$

$$
v_1 \approx 7.67 \text{ m/s}
$$

So, right before the crash, Block 1 is speeding along at about 7.67 meters per second.

---

### Part 2: The Collision

Now, Block 1 slams into Block 2 and they stick together. We use **Conservation of Momentum** to find out what happens next.

**Step 1: Write down what we know for the crash.**
* Mass of Block 1 ($m_1$) = $0.5 \text{ kg}$
* Speed of Block 1 before crash ($v_1$) = $7.67 \text{ m/s}$
* Mass of Block 2 ($m_2$) = $1.5 \text{ kg}$
* Speed of Block 2 before crash ($v_2$) = $0 \text{ m/s}$ (because it is at rest)

**Step 2: Set up the Momentum Conservation equation.**

$$
m_1v_1 + m_2v_2 = (m_1 + m_2)v_{final}
$$

**Step 3: Plug in our numbers.**

$$
(0.5 \cdot 7.67) + (1.5 \cdot 0) = (0.5 + 1.5) \cdot v_{final}
$$

**Step 4: Do the math to solve for $v_{final}$.**
Since Block 2 was sitting still, its initial momentum is zero ($1.5 \cdot 0 = 0$).

$$
3.835 + 0 = 2.0 \cdot v_{final}
$$

$$
3.835 = 2.0 \cdot v_{final}
$$

Now, divide both sides by the combined mass (2.0) to get the final speed by itself:

$$
v_{final} = \frac{3.835}{2.0}
$$

$$
v_{final} \approx 1.918 \text{ m/s}
$$

**Answer:** Just after the collision, the combined mass of the two blocks will slide together at a speed of approximately **1.92 meters per second**.
