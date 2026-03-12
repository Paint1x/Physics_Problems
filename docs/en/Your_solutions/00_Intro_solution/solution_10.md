# Infinite Series: The Ant's Final Position

### Problem Summary
An ant moves in a spiral pattern with decreasing step sizes: $1, 1/2, 1/3, 1/4 \dots$ rotating through East, North, West, and South.

### Mathematical Foundations

**1. Horizontal Series (Leibniz Series):**

$$
1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \dots = \frac{\pi}{4}
$$

**2. Vertical Series (Half-Harmonic):**

$$
\frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \dots = \frac{1}{2} \ln(2)
$$

---

### Step-by-Step Solution

**1. Calculate the $x$-coordinate (East/West):**
The ant moves East on steps 1, 5, 9... and West on steps 3, 7, 11...

$$
x = \sum_{n=0}^{\infty} \frac{(-1)^n}{2n+1} = \frac{\pi}{4}
$$

**2. Calculate the $y$-coordinate (North/South):**
The ant moves North on steps 2, 6, 10... and South on steps 4, 8, 12...

$$
y = \sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{2n} = \frac{1}{2} \ln(2)
$$

### Final Result
The ant converges to the point:

$$
\left( \frac{\pi}{4}, \frac{\ln(2)}{2} \right) \approx (0.785, 0.346)
$$
