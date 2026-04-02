# The Physics of a Swinging Pendulum: Conservation of Energy

Welcome back! To solve this problem, we are going to use one of the most powerful and beautiful "shortcuts" in all of physics: **Conservation of Energy**. 

When a pendulum swings, trying to calculate the exact forces at every single millimeter of the swing is incredibly difficult because the angle is constantly changing. Instead, physicists just look at the energy at the very beginning and the energy at the very end. 

## 1. Necessary Definitions

* **Potential Energy ($PE$):** The energy of "position" or "height." When you pull the pendulum up to the starting angle, you are working against gravity. The higher you pull it, the more "stored" energy it has. 
* **Kinetic Energy ($KE$):** The energy of "motion." When you let the pendulum go, it speeds up. Its stored Potential Energy turns into Kinetic Energy. At the very bottom of the swing, it has no height left, meaning *all* of its energy is now Kinetic Energy (motion).
* **Conservation of Energy:** A rule stating that energy cannot be created or destroyed, only transformed. This means the total stored energy at the top of the swing is exactly equal to the total motion energy at the bottom of the swing.
* **Height ($h$):** The vertical distance the pendulum bob drops from its starting point to its lowest point. Measured in meters (m).

## 2. The Master Formulas

**1. Potential Energy ($PE$):**
Depends on mass ($m$), gravity ($g \approx 9.81 \text{ m/s}^2$), and height ($h$).

$$
PE = mgh
$$

**2. Kinetic Energy ($KE$):**
Depends on mass ($m$) and velocity or speed ($v$).

$$
KE = \frac{1}{2}mv^2
$$

**3. The Height of a Pendulum ($h$):**
If you know the length of the string ($L$) and the angle you pulled it back ($\theta$), you can find how much vertical height it gained using trigonometry. 

$$
h = L - L\cos(\theta)
$$

*(We can factor out the $L$ to make it look cleaner: $h = L(1 - \cos(\theta))$)*

---

## The Problem

A pendulum with a length of 1.0 meter is released from an initial angle of $15^\circ$. What is the speed of the pendulum bob at the bottom of its swing?

### Step-by-Step Solution:

**Step 1: Write down what we know.**
* Length ($L$) = 1.0 m
* Angle ($\theta$) = $15^\circ$
* Gravity ($g$) $\approx 9.81 \text{ m/s}^2$
* Speed at the bottom ($v$) = ?

*Note: The problem doesn't give us the mass ($m$) of the pendulum bob! Don't panic. As you'll see in Step 4, we won't actually need it.*

**Step 2: Find the starting height ($h$).**
Before we can use our energy formulas, we need to know how high up the pendulum was when it was released. Let's use our height formula:

$$
h = L(1 - \cos(\theta))
$$

Plug in our length (1.0) and our angle ($15^\circ$):

$$
h = 1.0 \cdot (1 - \cos(15^\circ))
$$

Using a calculator, $\cos(15^\circ)$ is approximately 0.9659.

$$
h = 1.0 \cdot (1 - 0.9659)
$$

$$
h = 1.0 \cdot 0.0341 = 0.0341 \text{ meters}
$$

So, pulling a 1.0-meter pendulum back by $15^\circ$ lifts it up by about 3.4 centimeters.

**Step 3: Set up the Conservation of Energy.**
At the top of the swing, the pendulum has maximum Potential Energy and zero Kinetic Energy (because you are holding it still). 
At the bottom of the swing, it has zero Potential Energy (it has dropped all the way down) and maximum Kinetic Energy. 

Because energy is conserved, the $PE$ at the top equals the $KE$ at the bottom:

$$
PE_{\text{top}} = KE_{\text{bottom}}
$$

Let's plug in the formulas for those:

$$
mgh = \frac{1}{2}mv^2
$$

**Step 4: Simplify the equation.**
Look at both sides of the equation. There is a mass ($m$) on the left, and a mass ($m$) on the right. If we divide both sides by $m$, they completely cancel out! This proves that a heavy pendulum swings at the exact same speed as a light pendulum.

$$
gh = \frac{1}{2}v^2
$$

Now, let's get $v^2$ by itself by multiplying both sides by 2:

$$
2gh = v^2
$$

To get just $v$, we take the square root of both sides:

$$
v = \sqrt{2gh}
$$

**Step 5: Plug in the numbers and solve!**
We know $g = 9.81$ and we found $h = 0.0341$ back in Step 2. 

$$
v = \sqrt{2 \cdot 9.81 \cdot 0.0341}
$$

Multiply the numbers inside the square root first:

$$
v = \sqrt{0.669042}
$$

Take the square root:

$$
v \approx 0.818 \text{ m/s}
$$

**Answer:** At the very bottom of its swing, the pendulum bob will be traveling at a speed of approximately **0.82 meters per second**.
