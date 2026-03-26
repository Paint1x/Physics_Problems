import numpy as np
import matplotlib.pyplot as plt

# Define constants
a, b, w = 5, 2, 1
t = np.linspace(0, 20, 1000)

# Calculate coordinates
x = a * np.cos(w * t)
y = b * np.sin(w * t)
z = b * t

# Plotting
fig = plt.figure(figsize=(10, 7))
ax = fig.add_subplot(111, projection='3d')
ax.plot(x, y, z, label='Trajectory (Elliptical Helix)', color='blue')
ax.set_xlabel('X axis (a cos(wt))')
ax.set_ylabel('Y axis (b sin(wt))')
ax.set_zlabel('Z axis (bt)')
plt.title("Motion of Point M")
plt.legend()
plt.show()
