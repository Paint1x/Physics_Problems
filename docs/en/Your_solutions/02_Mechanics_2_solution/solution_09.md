# Physics: Motion with Air Resistance (Drag)

Welcome! This is a more advanced, real-world physics problem. In introductory physics, we often pretend we are in a vacuum to make the math easy. But in reality, when you throw a ball into the air, the air pushes back! That "push back" is called **air resistance** or **drag**. 

Because you asked for a deep explanation from absolute scratch, we are going to walk through the calculus step-by-step. Don't let the scary-looking math intimidate you; I will explain exactly what every symbol means.

## 1. Necessary Definitions

* **Differential Equation:** The equation you were given is a "differential equation." It is basically a math puzzle. Instead of solving for a regular number (like $x = 5$), you are solving for an entire formula. 
* **Velocity ($v$):** How fast you are going.
* **Position ($x$):** Where you are (your height).
* **Time ($t$):** The stopwatch.
* **Derivative ($\frac{dv}{dt}$):** This is calculus language for "how much is velocity changing as time passes?" In physics, a change in velocity is called **acceleration**.
* **Mass ($m$):** How heavy the object is.
* **Gravity ($g$):** The downward pull of the Earth (usually $9.81 \text{ m/s}^2$).
* **Drag Coefficient ($k$):** A number that represents how much the air fights back. A feather has a high $k$, a bowling ball has a low $k$.
* **Initial Conditions:** Where you start when the stopwatch reads zero ($t=0$). 
    * $v(0) = v_0$ (You started by throwing it upward at a speed of $v_0$)
    * $x(0) = 10$ (You threw it while standing on a balcony $10$ meters high)

## 2. Reading the Equation

Let's look at the equation you were given:

$$
m\frac{dv}{dt} = -mg - kv
$$

This is actually just **Newton's Second Law** ($Force = mass \times acceleration$).
* $m\frac{dv}{dt}$ is Mass $\times$ Acceleration.
* $-mg$ is the force of gravity pulling the object DOWN (that's why it's negative).
* $-kv$ is the force of the air pulling the object DOWN. It is negative because air resistance always fights the direction you are moving.

---

## Part 1: Solve the equation by analytical methods

To solve this, we need to find two formulas: one for velocity $v(t)$, and one for height $x(t)$.

### Step 1A: Finding Velocity $v(t)$

We need to get all the $v$ terms on one side, and all the $t$ terms on the other. This is called **Separation of Variables**.

First, let's factor out the negative sign on the right side:

$$
m\frac{dv}{dt} = -(mg + kv)
$$

Now, divide both sides by $(mg + kv)$ and multiply both sides by $dt$:

$$
\frac{m}{mg + kv} dv = - dt
$$

Divide by $m$ to get it out of the way:

$$
\frac{1}{mg + kv} dv = -\frac{1}{m} dt
$$

Now we use an **integral** ($\int$) to add up all the tiny changes. We integrate both sides:

$$
\int \frac{1}{mg + kv} \, dv = \int -\frac{1}{m} \, dt
$$

The integral of $\frac{1}{x}$ is the natural logarithm, $\ln(x)$. But because there is a $k$ next to our $v$, we have to divide by $k$ (a rule in calculus):

$$
\frac{1}{k} \ln(mg + kv) = -\frac{t}{m} + C
$$

*(Note: $C$ is a constant. Whenever you integrate, you have to add $C$ because we don't know the exact starting point yet).*

**Finding $C$:**
We know that at $t=0$, the velocity is $v_0$. Let's plug those in to find $C$:

$$
\frac{1}{k} \ln(mg + kv_0) = -\frac{0}{m} + C
$$

So, $C = \frac{1}{k} \ln(mg + kv_0)$. Let's plug $C$ back into our main equation:

$$
\frac{1}{k} \ln(mg + kv) = -\frac{t}{m} + \frac{1}{k} \ln(mg + kv_0)
$$

Multiply everything by $k$:

$$
\ln(mg + kv) = -\frac{kt}{m} + \ln(mg + kv_0)
$$

Subtract $\ln(mg + kv_0)$ from both sides. A rule of logarithms is that $\ln(A) - \ln(B) = \ln(\frac{A}{B})$:

$$
\ln\left(\frac{mg + kv}{mg + kv_0}\right) = -\frac{kt}{m}
$$

To get rid of the "$\ln$", we use its mathematical opposite: the exponential function ($e$). We apply $e$ to both sides:

$$
\frac{mg + kv}{mg + kv_0} = e^{-\frac{kt}{m}}
$$

Multiply the bottom part to the right side:

$$
mg + kv = (mg + kv_0) e^{-\frac{kt}{m}}
$$

Finally, subtract $mg$ and divide by $k$ to get velocity ($v$) completely alone!

$$
v(t) = \left(v_0 + \frac{mg}{k}\right) e^{-\frac{kt}{m}} - \frac{mg}{k}
$$

*(This is your formula for exactly how fast the object is moving at any given second!)*

---

### Step 1B: Finding Position $x(t)$

Velocity is just the change in position over time ($v = \frac{dx}{dt}$). To find position, we take the integral of the velocity formula we just found.

$$
x(t) = \int v(t) \, dt
$$

$$
x(t) = \int \left( \left(v_0 + \frac{mg}{k}\right) e^{-\frac{kt}{m}} - \frac{mg}{k} \right) dt
$$

When you integrate an exponential function $e^{at}$, you divide by the constant $a$. Here, our constant is $-\frac{k}{m}$. So dividing by it means multiplying by $-\frac{m}{k}$:

$$
x(t) = -\frac{m}{k}\left(v_0 + \frac{mg}{k}\right) e^{-\frac{kt}{m}} - \frac{mg}{k}t + C_2
$$

**Finding $C_2$:**
We know from our initial conditions that at $t=0$, the starting height is $x=10$. Also remember that $e^0 = 1$. Let's plug those in:

$$
10 = -\frac{m}{k}\left(v_0 + \frac{mg}{k}\right)(1) - 0 + C_2
$$

So, $C_2 = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)$. 
Plug this back into our $x(t)$ equation and organize it neatly:

$$
x(t) = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right) \left(1 - e^{-\frac{kt}{m}}\right) - \frac{mg}{k}t
$$

*(This is your formula for exactly how high the object is at any given second!)*

---

## Part 2: Determine the maximum height

An object reaches its maximum height at the exact moment it stops moving upward and is about to fall back down. At that split second, its velocity is zero.

**Step 2A: Find the time ($t_{max}$) when velocity is $0$.**
Take our velocity formula and set $v(t) = 0$:

$$
0 = \left(v_0 + \frac{mg}{k}\right) e^{-\frac{kt}{m}} - \frac{mg}{k}
$$

Move $\frac{mg}{k}$ to the left:

$$
\frac{mg}{k} = \left(v_0 + \frac{mg}{k}\right) e^{-\frac{kt}{m}}
$$

Divide by the bracketed term:

$$
e^{-\frac{kt}{m}} = \frac{\frac{mg}{k}}{v_0 + \frac{mg}{k}}
$$

Multiply the top and bottom of the right side by $k$ to clean it up:

$$
e^{-\frac{kt}{m}} = \frac{mg}{kv_0 + mg}
$$

Flip both fractions upside down (which removes the negative sign from the exponent):

$$
e^{\frac{kt}{m}} = \frac{kv_0 + mg}{mg} = 1 + \frac{kv_0}{mg}
$$

Take the natural log ($\ln$) of both sides to bring the time down, and multiply by $\frac{m}{k}$:

$$
t_{max} = \frac{m}{k} \ln\left(1 + \frac{kv_0}{mg}\right)
$$

**Step 2B: Find the max height ($H_{max}$).**
Now that we know *when* it reaches the top, we plug that specific time ($t_{max}$) into our position formula $x(t)$. It gets messy, but if we do the algebra to simplify it, we get:

$$
H_{max} = 10 + \frac{m v_0}{k} - \frac{m^2 g}{k^2} \ln\left(1 + \frac{k v_0}{m g}\right)
$$

---

## Part 3: Compare with the case without drag

What if we were in a vacuum where there is no air ($k=0$)? 

**Without drag:**
* The only force is gravity. 
* Equation: $m\frac{dv}{dt} = -mg$
* Velocity equation: $v(t) = v_0 - gt$
* Position equation: $x(t) = 10 + v_0 t - \frac{1}{2}gt^2$
* Max Height formula: $H_{no\_drag} = 10 + \frac{v_0^2}{2g}$

**The Comparison:**
1. **Height:** With air drag, the object reaches a **lower** maximum height because the air acts like a brake, fighting against its upward movement.
2. **Time:** The object reaches its maximum height **faster** with air drag. Gravity and air resistance are working together to slow it down to $0 \text{ m/s}$, so it stops sooner. 
3. **Shape of flight:** Without drag, the trip up and the trip down take the exact same amount of time (a perfect parabola). With drag, the trip up is shorter than the trip down.

---

## Part 4: Numerical simulation using Python

Sometimes, physics equations get so complicated that we can't solve them with a clean formula. Instead, we use computers to simulate reality step-by-step (adding a fraction of a second at a time). This is called a **Numerical Simulation**. 

Here is a Python script using a very famous, beginner-friendly method called "Euler's Method". You can run this on your own computer!

```python
import matplotlib.pyplot as plt

# --- 1. Set our starting rules (Initial Conditions) ---
m = 1.0        # Mass (kg)
g = 9.81       # Gravity (m/s^2)
k = 0.5        # Drag coefficient (how thick the air is)
v_start = 20.0 # Starting speed (m/s)
x_start = 10.0 # Starting height (m)

# --- 2. Setup the simulation time ---
dt = 0.01      # Time step (we simulate 1/100th of a second at a time)
time = 0.0     # Stopwatch starts at 0

# Lists to save our data so we can graph it later
times = [time]
positions = [x_start]
velocities = [v_start]

# --- 3. Run the simulation ---
# We will loop this math over and over until the object hits the ground (x < 0)
v_current = v_start
x_current = x_start

while x_current >= 0:
    # Newton's Second Law to find the current acceleration
    # a = (-mg - kv) / m
    acceleration = (-m * g - k * v_current) / m
    
    # Update our velocity (New Velocity = Old Velocity + (Acceleration * time_step))
    v_current = v_current + (acceleration * dt)
    
    # Update our position (New Position = Old Position + (Velocity * time_step))
    x_current = x_current + (v_current * dt)
    
    # Update stopwatch
    time = time + dt
    
    # Save the data
    times.append(time)
    positions.append(x_current)
    velocities.append(v_current)

# --- 4. Plot the graph! ---
plt.figure(figsize=(10, 5))
plt.plot(times, positions, label="Height over time", color="blue", linewidth=2)
plt.title("Projectile Motion with Air Resistance")
plt.xlabel("Time (seconds)")
plt.ylabel("Height (meters)")
plt.axhline(0, color='black', linewidth=1) # The ground
plt.legend()
plt.grid(True)
plt.show()

print(f"Simulation finished. The object hit the ground at {time:.2f} seconds.")
print(f"Maximum height reached: {max(positions):.2f} meters.")
