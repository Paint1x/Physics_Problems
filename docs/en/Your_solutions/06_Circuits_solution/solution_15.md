# 15. Resistor Cube*

**The Simple Explanation:**
This is a famous classic physics puzzle! Imagine water (current) flowing into one corner of a cube. Because the cube is perfectly symmetrical, the water splits evenly into 3 identical pipes. Then those split evenly again. By tracking one single path of water from the start to the end, we can figure out the total resistance without doing crazy complex math.

**The Setup:**
* 12 resistors, all with the exact same value of $R$.
* Total current entering the cube = $I$.

**Step-by-Step Math:**
Let's track the current $I$ as it travels from the starting node to the opposite node.

1. **First Split:** Current enters the first corner and splits into 3 identical edges. The current in each edge is $I/3$.
2. **Second Split:** Each of those paths hits another corner and splits into 2 more identical edges. $(I/3)$ divided by $2$ is $I/6$. The current here is $I/6$.
3. **Third Merge:** As the paths approach the final exit corner, they merge back together into 3 final edges. The current is back to $I/3$.

Now, calculate the Voltage drop ($V = I \cdot R$) along any one of those single paths from start to finish:

$$
V_{total} = V_{part1} + V_{part2} + V_{part3}
$$

$$
V_{total} = \left(\frac{I}{3} \cdot R\right) + \left(\frac{I}{6} \cdot R\right) + \left(\frac{I}{3} \cdot R\right)
$$

Factor out the $I \cdot R$:

$$
V_{total} = I \cdot R \left(\frac{1}{3} + \frac{1}{6} + \frac{1}{3}\right)
$$

Find a common denominator (which is 6) to add the fractions:

$$
V_{total} = I \cdot R \left(\frac{2}{6} + \frac{1}{6} + \frac{2}{6}\right) = I \cdot R \left(\frac{5}{6}\right)
$$

Since Ohm's law says Total Resistance ($R_{equivalent}$) is $V_{total} / I$, the $I$ cancels out, leaving us with:

$$
R_{eq} = \frac{5}{6} R
$$
