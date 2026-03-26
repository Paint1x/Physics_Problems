# Solutions goes here
import numpy as np
import matplotlib.pyplot as plt

# Constants
v0 = 100        # Initial velocity (m/s)
angle = 37      # Launch angle (degrees)
g = 9.81        # Gravity (m/s^2)

# Convert angle to radians for math functions
theta = np.radians(angle)

# Initial velocity components
v0x = v0 * np.cos(theta)
v0y = v0 * np.sin(theta)

# 1. Time of Flight
t_flight = (2 * v0y) / g

# 2. Maximum Height
h_max = (v0y**2) / (2 * g)

# 3. Horizontal Range
range_x = v0x * t_flight

print(f"Time of Flight: {t_flight:.2f} s")
print(f"Max Height: {h_max:.2f} m")
print(f"Range: {range_x:.2f} m")

# Generate trajectory points for plotting
t_points = np.linspace(0, t_flight, num=100)
x_points = v0x * t_points
y_points = (v0y * t_points) - (0.5 * g * t_points**2)

# Plotting
plt.figure(figsize=(10, 5))
plt.plot(x_points, y_points)
plt.title(f'Projectile Trajectory ({v0}m/s at {angle} degrees)')
plt.xlabel('Distance (m)')
plt.ylabel('Height (m)')
plt.grid(True)
plt.show()
