# Understanding Spring Oscillations and Energy

Welcome back! This problem dives into something called **Simple Harmonic Motion (SHM)**. Whenever you see a spring bouncing back and forth or a pendulum swinging, you are looking at SHM. Let's break down the definitions and formulas you need to solve this.

## 1. Necessary Definitions

* **Mass ($m$):** The weight of the object attached to the spring. Measured in kilograms (kg). 
* **Amplitude ($A$):** The maximum distance the mass stretches or compresses the spring from its normal, resting position. Measured in meters (m).
* **Angular Frequency ($\omega$):** This represents how fast the object is cycling back and forth. The symbol is the lowercase Greek letter omega ($\omega$). It is measured in radians per second (rad/s).
* **Spring Constant ($k$):** A number that tells us exactly how stiff the spring is. A high $k$ means a very stiff spring (like a car suspension), and a low $k$ means a very loose spring (like a slinky). Measured in Newtons per meter (N/m).
* **Total Mechanical Energy ($E$):** The total amount of energy in the system. As the spring bounces, energy switches between movement (kinetic) and stored spring energy (potential), but the *total* energy stays exactly the same. Measured in Joules (J).

## 2. The Master Formulas

**Equation of Motion:**
The position of a bouncing mass at any given time ($t$) is often written like this:

$$
x(t) = A \cos(\omega t)
$$

**Finding the Spring Constant:**
The stiffness of a spring ($k$), the mass ($m$), and how fast it bounces ($\omega$) are perfectly linked by this formula:

$$
\omega = \sqrt{\frac{k}{m}}
$$

**Finding Total Energy:**
The total energy in the system depends only on how stiff the spring is ($k$) and how far you pulled it back ($A$):

$$
E = \frac{1}{2} k A^2
$$

---

## The Problem

A 10 kg mass is attached to a spring and oscillates according to the equation $x(t) = 0.2 \cos(10\pi t)$ (in meters). What is the spring constant $k$? What is the total mechanical energy of the system?

### Part 1: Finding the Spring Constant ($k$)

**Step 1: Compare our equation to the standard formula.**
The problem gives us the equation: $x(t) = 0.2 \cos(10\pi t)$
The standard formula is: $x(t) = A \cos(\omega t)$

By just looking at the two equations side-by-side, we can easily steal two pieces of vital information!
* The Amplitude ($A$) is $0.2 \text{ m}$.
* The Angular Frequency ($\omega$) is $10\pi \text{ rad/s}$.

We also know the mass ($m$) is $10 \text{ kg}$.

**Step 2: Use the frequency formula to solve for $k$.**
Let's take our formula linking frequency, mass, and the spring constant:

$$
\omega = \sqrt{\frac{k}{m}}
$$

**Step 3: Rearrange the formula to isolate $k$.**
First, we need to get rid of the square root. We do this by squaring both sides of the equation:

$$
\omega^2 = \frac{k}{m}
$$

Next, we multiply both sides by $m$ to get $k$ all by itself:

$$
k = m \cdot \omega^2
$$

**Step 4: Plug in the numbers!**
Remember, $m = 10$ and $\omega = 10\pi$. 

$$
k = 10 \cdot (10\pi)^2
$$

When you square $(10\pi)$, you have to square both the 10 and the $\pi$. So, $(10\pi)^2$ becomes $100\pi^2$.

$$
k = 10 \cdot 100\pi^2
$$

$$
k = 1000\pi^2 \text{ N/m}
$$

*(If you want that as a regular decimal number, $\pi^2$ is roughly 9.87, so $k \approx 9869.6 \text{ N/m}$. But leaving it as $1000\pi^2$ is usually preferred in physics classes because it's exactly precise!)*

**Answer 1:** The spring constant $k$ is **$1000\pi^2 \text{ N/m}$**.

---

### Part 2: Finding the Total Mechanical Energy ($E$)

Now that we have the spring constant ($k$), finding the total energy is incredibly straightforward.

**Step 1: Write down our knowns and the energy formula.**
* $k = 1000\pi^2 \text{ N/m}$
* $A = 0.2 \text{ m}$ (We grabbed this from the original equation in Part 1)

Our formula is:

$$
E = \frac{1}{2} k A^2
$$

**Step 2: Plug in the numbers.**

$$
E = \frac{1}{2} \cdot (1000\pi^2) \cdot (0.2)^2
$$

**Step 3: Calculate the math step-by-step.**
First, let's square the amplitude ($0.2 \cdot 0.2 = 0.04$).

$$
E = \frac{1}{2} \cdot (1000\pi^2) \cdot 0.04
$$

Next, let's multiply the numbers: $\frac{1}{2} \cdot 1000 = 500$.

$$
E = 500\pi^2 \cdot 0.04
$$

Finally, $500 \cdot 0.04 = 20$. 

$$
E = 20\pi^2 \text{ Joules}
$$

*(Again, as a decimal, this is roughly 197.4 Joules).*

**Answer 2:** The total mechanical energy of the system is **$20\pi^2 \text{ J}$**.
