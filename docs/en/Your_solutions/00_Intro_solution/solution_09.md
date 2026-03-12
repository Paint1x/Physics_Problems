# Optimization: Maximizing Area Under a Curve

### Problem Statement
Find the dimensions of a rectangle with the maximum area inscribed under the curve $y = 3 - x^2$ in the first quadrant.

### Formulas
- **Area**: $A = x \cdot y$
- **Curve constraint**: $y = 3 - x^2$

---

### Step-by-Step Solution

**1. Create the Area Function:**
Substitute the curve equation into the area formula:

$$
A = x(3 - x^2) = 3x - x^3
$$

**2. Find the derivative with respect to $x$:**

$$
\frac{dA}{dx} = 3 - 3x^2
$$

**3. Set the derivative to zero to find critical points:**

$$
3 - 3x^2 = 0 \implies x^2 = 1 \implies x = 1
$$

**4. Calculate the corresponding height ($y$):**

$$
y = 3 - (1)^2 = 2
$$

### Final Result
The dimensions for the maximum area are:

$$
\text{Width} = 1, \quad \text{Height} = 2
$$

The maximum area is $1 \times 2 = 2$ square units.
