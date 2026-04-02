# Physics: Forces and Friction on Stacked Blocks

Welcome! This is a fantastic problem because it involves analyzing multiple forces happening at the same time. Since you are just starting out, we are going to take this slow and look at exactly how things push and rub against each other.

Imagine a heavy box sitting on a rug. If you pull the rug out from under the box, the rug rubs against the floor, but it *also* rubs against the bottom of the box. We are dealing with exactly that situation here!

## 1. Necessary Definitions

* **Mass ($m$):** How much "stuff" makes up an object. Measured in kilograms (kg).
* **Gravity ($g$):** The constant pull of the Earth downwards. On Earth, this is always approximately $9.81 \text{ m/s}^2$.
* **Weight / Force of Gravity ($W$):** The actual downward force an object pushes with because of gravity. (Mass and Weight are different! Mass is the stuff, Weight is the physical downward push).
* **Normal Force ($N$):** The upward push from a surface. If a 10 kg block sits on the floor, gravity pulls it down, but the floor pushes back up to keep it from falling through the ground. That upward push is the Normal Force.
* **Kinetic Friction ($f_k$):** The rubbing force that slows things down when they slide past each other. "Kinetic" simply means "moving." 
* **Coefficient of Kinetic Friction ($\mu_k$):** A decimal number that tells you how rough or sticky a surface is. The symbol is the Greek letter "mu" ($\mu$). A higher number means more friction. Here, it is $0.2$.
* **Net Force ($F_{\text{net}}$):** The total leftover force after you subtract all the forces fighting against you (like friction) from the force you are pulling with.
* **Acceleration ($a$):** How quickly an object speeds up. Measured in meters per second squared ($\text{m/s}^2$).

## 2. The Master Formulas

**1. Weight ($W$):**
Mass multiplied by gravity.

$$
W = m \cdot g
$$

**2. Kinetic Friction ($f_k$):**
Friction depends on how rough the surfaces are ($\mu_k$) multiplied by how hard they are being squeezed together (the Normal Force, $N$).

$$
f_k = \mu_k \cdot N
$$

**3. Newton's Second Law of Motion:**
The most famous equation in mechanics. The total Net Force on an object equals its mass times its acceleration. 

$$
F_{\text{net}} = m \cdot a
$$

---

## The Problem

A **5 kg** block is placed on a **10 kg** block. A horizontal force of **45 N** is applied to the 10 kg block, and the 5 kg block is tied to the wall. The coefficient of kinetic friction between all moving surfaces is **0.2**. Find the acceleration of the 10 kg block.

### Step-by-Step Solution:

**Step 1: Understand the setup.**
* **Top Block (5 kg):** It is tied to a wall. It cannot move forward.
* **Bottom Block (10 kg):** It is being pulled forward with **45 N** of force. As it slides forward, it scrapes against the floor beneath it, AND it scrapes against the 5 kg block sitting on top of it.
* This means the bottom block has to fight **two** different friction forces! We need to calculate both.

**Step 2: Calculate the friction between the two blocks (Top Friction).**
To find friction, we need the Normal Force ($N_1$)—how hard the top block pushes down on the bottom block.
The top block is 5 kg. Its downward weight is:

$$
W_1 = m_1 \cdot g = 5 \cdot 9.81 = 49.05 \text{ Newtons}
$$

So, the top block squeezes against the bottom block with $49.05 \text{ N}$ of force. Now, let's find the friction rubbing between them using our friction formula ($\mu_k = 0.2$):

$$
f_{k1} = \mu_k \cdot N_1
$$

$$
f_{k1} = 0.2 \cdot 49.05 = 9.81 \text{ Newtons}
$$

*Top Friction = 9.81 N fighting against our pull.*

**Step 3: Calculate the friction between the bottom block and the floor (Bottom Friction).**
How hard is the floor being pushed down on? The floor has to support the bottom block (10 kg) **AND** the top block (5 kg) sitting on it. 
Total mass pressing on the floor = $10 + 5 = 15 \text{ kg}$.

Let's find that total downward weight ($N_2$):

$$
W_2 = m_{\text{total}} \cdot g = 15 \cdot 9.81 = 147.15 \text{ Newtons}
$$

Now, calculate the friction from the floor using the same coefficient ($\mu_k = 0.2$):

$$
f_{k2} = \mu_k \cdot N_2
$$

$$
f_{k2} = 0.2 \cdot 147.15 = 29.43 \text{ Newtons}
$$

*Bottom Friction = 29.43 N fighting against our pull.*

**Step 4: Calculate the Net Force ($F_{\text{net}}$).**
The Net Force is the total pulling force minus all the friction fighting it.
* Pulling Force = **45 N** (forward)
* Top Friction ($f_{k1}$) = **9.81 N** (backward)
* Bottom Friction ($f_{k2}$) = **29.43 N** (backward)

$$
F_{\text{net}} = 45 - 9.81 - 29.43
$$

$$
F_{\text{net}} = 45 - 39.24 = 5.76 \text{ Newtons}
$$

So, out of the 45 N you pulled with, only **5.76 N** is actually left over to make the 10 kg block speed up. The rest of your effort was completely wasted fighting friction!

**Step 5: Calculate the acceleration ($a$).**
Now we use Newton's Second Law. We only care about the **10 kg** block because that is the one moving. 

$$
F_{\text{net}} = m_2 \cdot a
$$

Plug in our Net Force (5.76) and the mass of the moving block (10):

$$
5.76 = 10 \cdot a
$$

To get acceleration ($a$) by itself, divide both sides by 10:

$$
a = \frac{5.76}{10}
$$

$$
a = 0.576 \text{ m/s}^2
$$

**Answer:** The acceleration of the 10 kg block is **$0.576 \text{ meters per second squared}$**.
