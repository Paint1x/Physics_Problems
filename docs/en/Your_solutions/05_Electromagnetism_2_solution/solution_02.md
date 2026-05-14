# 2. Ampere's Law

**The Simple Explanation:**
We have two wires with electricity flowing in opposite directions. Because they flow in opposite directions, the magnetic circles they create will actually spin in the *same* direction right in the middle. This means we calculate the field of one wire, and then add the second one to it.

**The Setup:**
* Current ($I$) = $5 \text{ A}$
* Total distance between wires = $10 \text{ cm}$ ($0.1 \text{ m}$)
* Distance to the midpoint ($r$) = $5 \text{ cm}$ ($0.05 \text{ m}$)
* Magnetic constant ($\mu_0$) = $4\pi \times 10^{-7} \text{ T m/A}$

**Step-by-Step Math:**
First, we find the magnetic field ($B$) from wire 1 using Ampere's formula:

$$
B_1 = \frac{\mu_0 \cdot I}{2\pi \cdot r}
$$

Plug in the numbers:

$$
B_1 = \frac{4\pi \times 10^{-7} \cdot 5}{2\pi \cdot 0.05}
$$

The $2\pi$ cancels out part of the $4\pi$, leaving $2$:

$$
B_1 = \frac{2 \times 10^{-7} \cdot 5}{0.05} = 20 \times 10^{-6} \text{ T}
$$

Because both wires push the magnetic field in the same direction at the midpoint, we multiply by 2:

$$
B_{total} = B_1 + B_2 = 20 \mu\text{T} + 20 \mu\text{T} = 40 \mu\text{T}
$$

**Final Answer:**
The magnetic field is **$40 \mu\text{T}$**. The direction is perpendicular to the plane containing the wires, determined by the Right-Hand Rule.
