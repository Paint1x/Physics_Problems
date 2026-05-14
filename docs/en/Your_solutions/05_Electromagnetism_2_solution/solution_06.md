# 6. EM Wave Analysis

**The Simple Explanation:**
We are given a mathematical map of a wave. By matching our wave to the standard physics formula, we can unlock all its secrets (like how long it is and how fast it wiggles).

**The Setup:**
* Given Equation: $E_y(x,t) = 100 \sin(10^7 x - \omega t)$
* Standard Equation: $E(x,t) = E_{max} \sin(kx - \omega t)$
* By comparing them, we know the "wave number" ($k$) is $10^7$.
* Speed of light ($c$) = $3 \times 10^8 \text{ m/s}$.

**Step-by-Step Math:**

**1. Direction:** Because it is $(kx - \omega t)$, the minus sign means it is traveling in the positive $x$-direction.

**2. Wavelength ($\lambda$):** 

$$
\lambda = \frac{2\pi}{k}
$$

$$
\lambda = \frac{2\pi}{10^7} \approx 6.28 \times 10^{-7} \text{ m} \text{ (or 628 nm)}
$$

**3. Angular Frequency ($\omega$):**

$$
\omega = k \cdot c
$$

$$
\omega = 10^7 \cdot (3 \times 10^8) = 3 \times 10^{15} \text{ rad/s}
$$

**4. Magnetic Field Equation ($B_z$):** The magnetic field is just the electric field divided by the speed of light.

$$
B_{max} = \frac{E_{max}}{c} = \frac{100}{3 \times 10^8} \approx 3.33 \times 10^{-7} \text{ T}
$$

$$
B_z(x,t) = 3.33 \times 10^{-7} \sin(10^7 x - 3 \times 10^{15} t) \text{ T}
$$
