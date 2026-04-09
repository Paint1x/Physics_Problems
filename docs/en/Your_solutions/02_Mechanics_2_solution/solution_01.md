#  pendulum-physics-problems

A simple pendulum has a period of 4 seconds on Earth. What would its period be on the Moon, where the gravitational acceleration is about 1/6th of Earth's?

What is the required length of a simple pendulum to have a period of exactly 1 second on Earth?

## 📚 Necessary Definitions

Before we solve the problems, let's understand the basic terms:

* **Simple Pendulum:** Imagine a weight (called a "bob") hanging from a string that swings back and forth. A playground swing is a great real-life example.
* **Period ($T$):** The time it takes for the pendulum to make one *complete* swing (starting at one side, swinging to the other, and returning to the exact starting point). We measure this in seconds.
* **Length ($L$):** The length of the string from the pivot point at the top down to the center of the weight. We measure this in meters.
* **Gravitational Acceleration ($g$):** The invisible force that pulls things down. On Earth, this force pulls at a constant rate of roughly **9.8 meters per second squared** (written as $9.8 \text{ m/s}^2$). 
* **Pi ($\pi$):** A mathematical constant representing the ratio of a circle's circumference to its diameter. It's approximately **3.14159**.

### The Golden Rule of Pendulums
The most important thing to know is that the time it takes for a pendulum to swing back and forth (the Period) depends on **only two things**:
1.  How long the string is ($L$).
2.  How strong gravity is pulling on it ($g$).

*It does not matter how heavy the weight is!* ## 🧮 The Core Formula

Here is the formula we use to find the period of a pendulum. 

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

**How to read this formula:** The Period ($T$) equals 2 times Pi ($2\pi$), multiplied by the square root of the Length ($L$) divided by Gravity ($g$).

---

## 🚀 Problem 1: The Pendulum on the Moon

**The Question:** A simple pendulum has a period of 4 seconds on Earth. What would its period be on the Moon, where the gravitational acceleration is about 1/6th of Earth's?

### Step-by-Step Solution:

**Step 1: Understand what we know.**
* The Period on Earth ($T_{Earth}$) is **4 seconds**.
* Gravity on the Moon ($g_{Moon}$) is **1/6** of the Gravity on Earth ($g_{Earth}$).

**Step 2: Set up the equation for the Moon.**
We take our core formula but use the Moon's gravity instead of Earth's.

$$
T_{Moon} = 2\pi \sqrt{\frac{L}{g_{Moon}}}
$$

**Step 3: Swap in the Earth gravity fraction.**
Since the Moon's gravity is just Earth's gravity divided by 6, we replace $g_{Moon}$ with $\frac{g_{Earth}}{6}$.

$$
T_{Moon} = 2\pi \sqrt{\frac{L}{\frac{g_{Earth}}{6}}}
$$

**Step 4: Use a math trick to clean up the fraction.**
In math, dividing by a fraction is the same as multiplying by its flipped version. So, bringing the 6 to the top gives us:

$$
T_{Moon} = 2\pi \sqrt{6 \cdot \frac{L}{g_{Earth}}}
$$

**Step 5: Separate the numbers.**
We can pull that number 6 out of the main fraction, as long as we keep it under its own square root.

$$
T_{Moon} = \sqrt{6} \cdot \left( 2\pi \sqrt{\frac{L}{g_{Earth}}} \right)
$$

**Step 6: Notice the hidden Earth formula!**
Look closely at the part inside the parentheses: $2\pi \sqrt{\frac{L}{g_{Earth}}}$. That is the exact formula for the period of the pendulum on Earth! And the problem already told us that the period on Earth is **4 seconds**. So, we can replace that entire chunk of math with the number 4.

$$
T_{Moon} = \sqrt{6} \cdot 4
$$

**Step 7: Calculate the final answer.**
The square root of 6 is about **2.45**. 

$$
T_{Moon} = 2.45 \cdot 4
$$

$$
T_{Moon} = 9.8 \text{ seconds}
$$

**Answer:** On the Moon, because gravity is weaker, the pendulum swings much slower. It would take about **9.8 seconds** to complete one swing.

---

## 📏 Problem 2: Finding the Exact Length

**The Question:** What is the required length of a simple pendulum to have a period of exactly 1 second on Earth?

### Step-by-Step Solution:

**Step 1: Understand what we know.**
* The target Period ($T$) is **1 second**.
* Gravity on Earth ($g$) is **9.8 m/s²**.

**Step 2: Start with the core formula.**

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

**Step 3: Isolate the Length ($L$).**
Because we want to find the length, we need to shuffle the math around to get $L$ by itself. First, divide both sides by $2\pi$ to move it away from the $L$.

$$
\frac{T}{2\pi} = \sqrt{\frac{L}{g}}
$$

**Step 4: Get rid of the square root.**
To undo a square root, we multiply everything by itself (we square both sides).

$$
\frac{T^2}{4\pi^2} = \frac{L}{g}
$$

**Step 5: Move gravity ($g$) to the other side.**
Multiply both sides by $g$. Now we have our custom formula to find the length!

$$
L = \frac{g \cdot T^2}{4\pi^2}
$$

**Step 6: Plug in our numbers.**
We know $T = 1$ and $g = 9.8$.

$$
L = \frac{9.8 \cdot 1^2}{4 \cdot 3.14159^2}
$$

**Step 7: Do the final math.**
* $1^2$ is just 1. So the top part is just **9.8**.
* $3.14159^2$ is about **9.8696**.
* Multiply that by 4 to get the bottom part: **39.478**.

$$
L = \frac{9.8}{39.478}
$$

$$
L \approx 0.248 \text{ meters}
$$

**Answer:** To make a pendulum that takes exactly 1 second to swing back and forth on Earth, the string needs to be roughly **0.248 meters** long (which is **24.8 centimeters**).
