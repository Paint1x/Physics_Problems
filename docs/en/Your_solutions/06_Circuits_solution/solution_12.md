# 12. Transformer Currents

**The Simple Explanation:**
Transformers are like electrical gears made of two coils of wire. They work on a simple ratio. If the second coil has 5 times fewer loops of wire than the first coil, the voltage will drop and be 5 times lower! However, as a trade-off, the current behaves in reverse and will be 5 times *higher*.

**The Setup:**
* Primary turns/loops ($N_p$) = $1000$
* Secondary turns/loops ($N_s$) = $200$
* Primary voltage ($V_p$) = $120 \text{ V}$
* Secondary current ($I_s$) = $3 \text{ A}$

**Step-by-Step Math:**

**1. Secondary Voltage ($V_s$):**

$$
\frac{V_s}{V_p} = \frac{N_s}{N_p}
$$

$$
V_s = 120 \cdot \left(\frac{200}{1000}\right) = 120 \cdot 0.2 = 24 \text{ V}
$$

**2. Primary Current ($I_p$):** *(Remember, current works in reverse!)*

$$
\frac{I_p}{I_s} = \frac{N_s}{N_p}
$$

$$
I_p = 3 \cdot \left(\frac{200}{1000}\right) = 3 \cdot 0.2 = 0.6 \text{ A}
$$
