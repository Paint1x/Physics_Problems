# Physics: Position, Velocity, and Acceleration

This problem tests your understanding of how to use calculus to move between position, velocity, and acceleration. 

## 1. The Core Concept

* **Position ($x$):** Where the object is located.
* **Velocity ($v$):** How fast the object is changing its position. You find this by taking the **derivative** of position.
* **Acceleration ($a$):** How fast the velocity is changing. You find this by taking the **derivative** of velocity.

To go the opposite direction (from acceleration back to velocity, or velocity back to position), you take the **integral**. 

---

## Part 1: Finding the Acceleration (The Derivative)

**Step 1: Start with the given velocity formula.**

$$
v(t) = t^2 + 2t - 5
$$

**Step 2: Take the derivative.**
To find acceleration, we take the derivative of velocity with respect to time ($t$). Using the power rule ($t^n \rightarrow n t^{n-1}$):
* $t^2$ becomes $2t$
* $2t$ becomes $2$
* The constant $-5$ becomes $0$

$$
a(t) = 2t + 2
$$

**Step 3: Solve for $t=3$.**
The problem asks for the acceleration at $3$ seconds. Plug in $3$ for $t$:

$$
a(3) = 2(3) + 2
$$

$$
a(3) = 6 + 2 = 8
$$

**Answer 1:** The acceleration at exactly $3$ seconds is **$8$**.

---

## Part 2: Finding the Position (The Integral)

**Step 1: Set up the integral.**
To go from velocity up to position, we take the integral of our original velocity equation.

$$
x(t) = \int (t^2 + 2t - 5) \, dt
$$

**Step 2: Integrate.**
Using the reverse power rule (increase the exponent by $1$, then divide by the new exponent):
* $t^2$ becomes $\frac{1}{3}t^3$
* $2t$ becomes $t^2$
* $-5$ becomes $-5t$
* *Crucial step:* Add the unknown constant of integration, $C$.

$$
x(t) = \frac{1}{3}t^3 + t^2 - 5t + C
$$

**Step 3: Find the starting point ($C$).**
The problem gives us an initial condition: at $t=0$, the position is $x=4$. Plug $0$ in for $t$ and $4$ in for $x(t)$:

$$
4 = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C
$$

Since all the terms with $t$ just become zero, we are left with:

$$
C = 4
$$

Now we can write our complete, final position formula:

$$
x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4
$$

**Step 4: Solve for position at $t=3$.**
Plug $3$ into our complete position formula:

$$
x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4
$$

First, calculate the exponents ($3^3 = 27$ and $3^2 = 9$):

$$
x(3) = \frac{1}{3}(27) + 9 - 15 + 4
$$

Multiply the fraction:

$$
x(3) = 9 + 9 - 15 + 4
$$

Add and subtract:

$$
x(3) = 7
$$

**Answer 2:** The position of the object at exactly $3$ seconds is **$7$**.
