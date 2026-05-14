# 3. Biot-Savart Law

**The Simple Explanation:**
Instead of a long wire, we only have a tiny piece of one. We need to measure how much magnetic force just this tiny piece creates at point P.

**The Setup:**
* Length of segment ($\Delta L$) = $0.1 \text{ m}$
* Current ($I$) = $3 \text{ A}$
* Distance to point ($r$) = $0.2 \text{ m}$
* Angle ($\theta$) = $90^\circ$ (perpendicular, so $\sin(90^\circ) = 1$)

**Step-by-Step Math:**
We use the simplified Biot-Savart formula for a short segment:

$$
\Delta B = \frac{\mu_0 \cdot I \cdot \Delta L \cdot \sin(\theta)}{4\pi \cdot r^2}
$$

Plug in the constants and our numbers:

$$
\Delta B = \frac{4\pi \times 10^{-7} \cdot 3 \cdot 0.1 \cdot 1}{4\pi \cdot (0.2)^2}
$$

The $4\pi$ on top and bottom cancel out cleanly:

$$
\Delta B = \frac{10^{-7} \cdot 0.3}{0.04}
$$

**Final Answer:**

$$
\Delta B = 7.5 \times 10^{-7} \text{ T}
$$
