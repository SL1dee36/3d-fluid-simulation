# 3D Fluid Simulation

**Version:** 1.0

**Author:** [SL1dee36](https://github.com/SL1dee36)

This program simulates a 3D fluid using the Smoothed Particle Hydrodynamics (SPH) method. It allows users to interact with the fluid by creating new particles and manipulating existing ones in a three-dimensional space.


## Features

* **3D Fluid Dynamics:** Simulates fluid movement, pressure, viscosity, and interaction with boundaries in a 3D environment.
* **Perspective Rendering:** Renders particles with a perspective projection, providing a sense of depth.
* **Interactive Controls:**
    * **Left Mouse Button:** Creates new particles at the cursor's 3D position (projected onto a plane).
    * **Right Mouse Button:** Drags and interacts with particles within a radius in 3D space.
    * **Mouse Wheel:** Zoom in and out by changing the camera's position.
    * **W, A, S, D Keys:** Move the camera forward, left, backward, and right, respectively.
    * **Spacebar & Left Shift:** Move the camera up and down, respectively.
    * **Ctrl + Mouse Movement:** Rotate the camera's yaw and pitch.
    * **R Key:** Clears all particles.
* **Obstacle Interaction:** Includes a spherical obstacle that particles can collide with.
* **Visual Representation:** Renders particles with a color gradient based on their speed.
* **Performance Optimizations:** Implements efficient neighbor search and force calculation algorithms.
* **Dynamic Window Title:** Displays real-time information about the number of particles, camera position, and cursor coordinates in 3D space.


## Dependencies

* **SDL2:** Simple DirectMedia Layer 2 library for graphics rendering and input handling.

## Building and Running

1. **Install SDL2:** Instructions for installing SDL2 can be found on the official website: [https://www.libsdl.org/download-2.0.php](https://www.libsdl.org/download-2.0.php)
2. **Compile the code:** Use a C++ compiler that supports SDL2 (e.g., g++):
   ```bash
   g++ -o fluid_simulation_3d fluid_simulation_3d.cpp -lSDL2
   ```
3. **Run the executable:**
   ```bash
   ./fluid_simulation_3d
   ```

## Configuration

The simulation parameters can be adjusted by modifying the constants at the beginning of the code. These parameters are similar to the 2D version but with added considerations for the Z-axis and camera controls.


## Known Issues

* Performance may degrade with a large number of particles.
* The simulation is not perfectly accurate and may exhibit some unrealistic behavior in certain scenarios.
* The current implementation uses a simplified perspective projection; a more robust method could be implemented.


## Future Improvements

* Implement more advanced SPH features, such as surface tension and more realistic boundary handling.
* Optimize performance further to handle more particles.
* Implement a more sophisticated camera system with better controls and perspective projection.
* Add more interactive features and customization options.


## License

This project is released under the MIT License. See the LICENSE file for details.
