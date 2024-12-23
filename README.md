# Boids Simulation  
[Live Preview](https://viveksharma2525.github.io/Boids-p5.js/) (Best viewed on laptop/desktop)  

This project is inspired by *The Coding Train's* Boids coding challenge on YouTube. It recreates Craig Reynolds' Boids model using p5.js, demonstrating emergent flocking behavior of bird-like agents called Boids.  

---

## About the Simulation  
The simulation showcases how simple rules applied to individual agents can lead to complex group behavior. Boids interact based on three core principles:  

1. **Separation**: Avoid crowding by maintaining personal space.  
   - Boids steer away from nearby agents to prevent overlaps.  
2. **Alignment**: Align movement with nearby Boids.  
   - Boids adjust their direction to match the average velocity of neighbors.  
3. **Cohesion**: Move toward the local group's center.  
   - Boids are attracted to the average position of nearby agents.  

### How It Looks in Action  
- **A single Boid in isolation** moves freely in the environment.  
- **A small group of Boids** begins to cluster and align, moving as a flock.  
- **With many Boids**: Complex patterns emerge, mimicking bird flocks or fish schools.  

Adding **Predators** introduces new dynamics:  
- Boids attempt to flee from nearby Predators.  
- Predators pursue Boids using a "look-ahead" feature that predicts their paths.

---

## Additional Features  
- **Predators**:  
  - Hunt Boids by predicting their positions and velocities.  
  - Have a hunger system: Starvation leads to death.  
- **Sight Ranges**: Boids and Predators have limited perception for realistic interactions.  
- **Dynamic Interactions**: Group behavior and wrap-around edges ensure agents interact naturally.  

---

## Controls  
- **Behavior Toggles**:  
  - Press `A` for Alignment, `C` for Cohesion, and `S` for Separation.  
- **Add Agents**:  
  - Hold `B` (Boids) or `P` (Predators) and click within the simulation area.  

*A laptop or desktop is recommended for optimal experience.*  

### Customization  
Simulation parameters like initial values, agent sizes, sight ranges, and interaction weights can be modified in `globals.js`.  

---

## Technical Highlights  
- **OOP Principles**: Implemented with inheritance and polymorphism.  
- **Optimizations**: Uses bin-lattice spatial subdivision for efficient performance.  
- **Vector Math**: Extensive use and optimization of vector operations.  

---

