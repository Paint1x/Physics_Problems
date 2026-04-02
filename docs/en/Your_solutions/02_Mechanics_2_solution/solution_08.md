# Physics: The Spring Force and Potential Energy

This problem looks at one of the most important relationships in all of physics: the relationship between force, work, and stored energy. 

The equation you were given, $F(x) = -kx$, is known as **Hooke's Law**. It describes the force of a spring. 
* $x$ is how far you stretch or compress the spring. 
* $k$ is the "spring constant" (how stiff the spring is).
* The negative sign ($-$) just means that the spring always pulls *back* toward its starting resting position. If you pull it right (positive $x$), it pulls left (negative force).

Let's look at the definitions and formulas we need to solve this.

## 1. Necessary Definitions & Math Tools

* **Equation of Motion:** A mathematical sentence that describes how an object's position ($x$) changes as time ($t$) passes.
* **Acceleration ($a$):** How fast your speed is changing. In calculus, acceleration is the "second derivative" of position, written as $\frac{d^2x}{dt^2}$. 
* **Work ($W$):** The total amount of effort it takes to push or pull an object over a distance. Measured in Joules.
* **Integral ($\int$):** A calculus tool used to calculate Work. It is basically a way to add up an infinite number of tiny slices. When a force is changing (like a spring getting harder to pull the further you stretch it), we use an integral to find the total Work.
* **Potential Energy ($U$):** Stored energy. When you do Work on a spring by stretching it, that Work gets stored inside the spring as Potential Energy. 
* **Derivative ($\frac{d}{dx}$):** A calculus tool that finds the "rate of change" or the slope of a curve. It is the exact opposite of an integral. 

## 2. The Master Formulas

**1. Newton's Second Law:**
Force equals mass times acceleration.

$$
F = m \cdot a
$$

**2. Work (Calculus Formula):**
Work is the integral (sum) of Force over a distance from a starting point to an ending point. 

$$
W = \int F \, dx
$$

**3. Relationship between Work and Potential Energy:**
The change in stored energy is the exact opposite of the work done *by* the spring's force.

$$
\Delta U = -W
$$

---

## Step-by-Step Solution

### Part 1: Write down the equation of motion and solve it.

**The Setup:**
We know from Newton's Second Law that Force equals mass times acceleration ($F = ma$).
In calculus, we write acceleration as $\frac{d^2x}{dt^2}$. 

So, our force equation looks like this:

$$
F = m \frac{d^2x}{dt^2}
$$

The problem tells us that $F(x) = -kx$. So we can set them equal to each other to create our **Equation of Motion**:

$$
m \frac{d^2x}{dt^2} = -kx
$$

**The Solution:**
To solve this, we divide both sides by mass ($m$):

$$
\frac{d^2x}{dt^2} = -\frac{k}{m}x
$$

In plain English, this equation asks a math riddle: *"What mathematical function gives you the exact same function back, just negative and multiplied by $\frac{k}{m}$, when you take its derivative twice?"*

In mathematics, the functions that do this are sine and cosine waves! This makes physical sense, because a spring bounces back and forth in a wave-like motion. The solution to this equation is:

$$
x(t) = A \cos\left(\sqrt{\frac{k}{m}} t\right)
$$

*(Here, $A$ is the maximum stretch of the spring, and $t$ is time).*

---

### Part 2: Calculate the work done during the displacement from $0$ to $x_0$.

To find the Work done by the spring as it stretches from $0$ to a specific point ($x_0$), we have to use an integral. We are adding up the force $-kx$ at every tiny millimeter of the stretch.

$$
W = \int_{0}^{x_0} -kx \, dx
$$

**How to solve this integral:**
In calculus, the "power rule" for integrals says that to integrate $x^1$, you raise the power by 1 (to make it $x^2$), and then divide by that new power (divide by 2). The constant $-k$ just stays where it is.

$$
W = \left[ -\frac{1}{2}kx^2 \right]_{0}^{x_0}
$$

Now, we plug in our end point ($x_0$) and subtract what happens when we plug in our start point ($0$). Since plugging in $0$ just makes the whole thing zero, we are left with:

$$
W = -\frac{1}{2}kx_0^2
$$

**Answer:** The total work done by the spring force is **$-\frac{1}{2}kx_0^2$**. It is negative because the spring is trying to pull in the opposite direction that it is being stretched.

---

### Part 3: Interpret the result as potential energy.

How does Work relate to stored energy ($U$)? 
Physics tells us that the Potential Energy stored in a system is equal to the *negative* of the Work done by the internal force (the spring). 

$$
\Delta U = -W
$$

Let's plug in the Work we just calculated:

$$
\Delta U = -\left( -\frac{1}{2}kx_0^2 \right)
$$

The two negative signs cancel each other out, making it positive:

$$
U(x_0) = \frac{1}{2}kx_0^2
$$

**Interpretation:** This means that when you pull a spring to a distance of $x$, the energy required to pull it gets trapped inside the spring as **Potential Energy**. The formula for the stored energy in a spring at any distance $x$ is:

$$
U(x) = \frac{1}{2}kx^2
$$

---

### Part 4: Verify the relationship $F = -\frac{dU}{dx}$.

This formula claims that if you take the negative derivative ($-\frac{d}{dx}$) of the Potential Energy, you will get the Force back. Let's test it!

Start with our Potential Energy equation:

$$
U(x) = \frac{1}{2}kx^2
$$

Now, let's take the derivative with respect to $x$. In calculus, the power rule for derivatives says you take the exponent (the $2$), bring it to the front to multiply, and then lower the exponent by 1. 

$$
\frac{dU}{dx} = 2 \cdot \left(\frac{1}{2}kx^{2-1}\right)
$$

The $2$ and the $\frac{1}{2}$ cancel each other out to become $1$. The $x^1$ just becomes $x$. 

$$
\frac{dU}{dx} = kx
$$

The relationship asks us to make it negative:

$$
-\frac{dU}{dx} = -kx
$$

Look at that! $-kx$ is exactly the force $F(x)$ that we started the problem with. 
**Verification complete:** $F(x) = -\frac{dU}{dx}$ is completely true!

---

### Part 5: Draw the graph of $F(x)$ and $U(x)$.

Since I cannot draw physically on your screen, I will describe exactly how these two graphs look so you can sketch them easily:

**1. The Graph of Force: $F(x) = -kx$**
* **Shape:** A straight line.
* **Details:** Draw a standard graph with an X and Y axis. Because of the negative sign, this line will slope *downwards* from left to right. It passes perfectly through the very center origin point $(0,0)$. 
* **Meaning:** When $x$ is positive (stretched right), the line is in the bottom half of the graph (negative force, pulling left). 

**2. The Graph of Potential Energy: $U(x) = \frac{1}{2}kx^2$**
* **Shape:** A parabola (a "U" shape).
* **Details:** Draw a "U" shape that opens upwards. The very bottom tip (vertex) of the "U" should sit perfectly at the origin $(0,0)$. 
* **Meaning:** At $0$ stretch, there is $0$ stored energy. But whether you stretch the spring forward (positive $x$) or crush it backward (negative $x$), the energy goes UP as a positive number.
