# physics-sim-engine
A custom physics simulation engine built in Unity using C# that simulates sphere dynamics, force systems, and collision detection integrated into an interactive maze game.

Overview
Built a physics engine from scratch implementing force calculations, Euler integration, and collision response for sphere and plane colliders. The engine powers an interactive maze game where a player-controlled sphere navigates a maze, collects objects, and collides with walls.


# Features


Physics Engine

- Euler's method integration for solving position and velocity at each timestep
- Gravity as a constant force
- Viscous drag force (F = −kd × v)
- Sphere-sphere collision detection and response
- Sphere-plane collision detection and response including edge and corner cases
- Restitution constant for controlling velocity attenuation on bounce
- Normal force handling to keep spheres stable on plane surfaces

- https://github.com/user-attachments/assets/f037b5ce-b594-4005-ac7f-c5ab4142e7b6
- https://github.com/user-attachments/assets/ab0eb8cb-46c5-4388-941d-dd81d8b1f72f
- https://github.com/user-attachments/assets/2f106a68-a5c1-4dd8-9c05-5ce5e8572e11
- https://github.com/user-attachments/assets/08fe6f33-79aa-44f9-9bfb-e2ab28068bd0

Maze Game

- Player controlled sphere navigating a maze using the physics engine
- Collectible pickup detection via sphere collider
- Wall collisions via plane colliders
- Sphere emitter system with configurable period, scale, and max sphere count

https://github.com/user-attachments/assets/df0dafa1-03d1-4e80-99b8-3a0b7916a7a1


Technical Details
- Language: C#
- Engine: Unity
- Physics: Custom Euler integration, no Unity physics engine used
- Collision: Sphere-sphere and sphere-plane detection in local collider space with world space response conversion

Scenes
- SimTest — isolated physics engine testing with multiple collider configurations
- MazeGame — full game integration with collectibles and end wall
