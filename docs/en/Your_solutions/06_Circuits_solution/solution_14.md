# 14. RLC Circuit

**The Simple Explanation:**
An RLC circuit has a Resistor, an Inductor, and a Capacitor. In physics, the math for this circuit looks *exactly* the same as the math for a bouncy spring dragging on a rough floor. 
* The **Inductor ($L$)** acts like a heavy weight (Mass). It takes effort to get it moving, and effort to stop it.
* The **Resistor ($R$)** acts like friction (Damping). It slows things down and wastes energy as heat.
* The **Capacitor ($C$)** acts like a bouncy spring (Stiffness). It stores energy and pushes back.

**Step-by-Step Math:**
The differential equation for the RLC circuit is based on Kirchhoff's Voltage Law. (We use charge $Q$ here, noting that current $I$ is just the derivative of $Q$ over time).

$$
L \frac{d^2Q}{dt^2} + R \frac{dQ}{dt} + \frac{1}{C} Q = V(t)
$$

The equation for a physical damped harmonic oscillator (like a mass on a spring) using Newton's Second Law is:

$$
m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + k x = F(t)
$$

**The Direct Analogies:**
By looking at the two equations side-by-side, we can match up the parts perfectly:
* $L$ (Inductance) matches with $m$ (Mass/Inertia)
* $R$ (Resistance) matches with $b$ (Damping/Friction coefficient)
* $1/C$ (Inverse Capacitance) matches with $k$ (Spring constant)
* $Q$ (Electrical Charge) matches with $x$ (Physical Position)
* $V$ (Voltage source) matches with $F$ (External Force)
