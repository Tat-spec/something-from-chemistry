# something-from-chemistryimport matplotlib.pyplot as plt

# Define coordinates of chlorine atoms
chlorine1 = (0, 0)
chlorine2 = (2, 0)  # Assuming a distance of 2 units between the atoms

# Plotting the chlorine molecule
plt.figure(figsize=(6, 3))

# Plot chlorine atoms
plt.plot(chlorine1[0], chlorine1[1], 'bo', markersize=10, label='Chlorine 1')
plt.plot(chlorine2[0], chlorine2[1], 'go', markersize=10, label='Chlorine 2')

# Draw bond between chlorine atoms
plt.plot([chlorine1[0], chlorine2[0]], [chlorine1[1], chlorine2[1]], 'k-', linewidth=2)

# Adding labels and title
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Chlorine Molecule (Cl₂)')
plt.legend()

# Set equal scaling and display grid
plt.axis('equal')
plt.grid(True)

# Show plot
plt.show()
