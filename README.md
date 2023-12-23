# Micromouse

Micromouse is a robotics competition where small autonomous robots, known as micromice or mice, navigate through a maze to reach a designated target area. The Mouse Maze Solver is an intelligent algorithmic program designed specifically for micromouse competitions. It comprises two main components: the `Maze` class, responsible for representing the maze structure and its properties, and the `Mouse` class, an algorithmic entity utilizing the maze to solve navigation challenges.


# Maze Solver

## Overview

The Mouse Maze Solver is an intelligent algorithmic program designed to navigate through a maze efficiently. The project comprises two main components: the `Maze` class, responsible for representing the maze structure and its properties, and the `Mouse` class, an algorithmic entity utilizing the maze to solve navigation challenges.

## Maze Class

### Design Highlights:

- **Modular Structure:** The `Maze` class encapsulates the maze structure, separating concerns related to walls, boxes, and exploration status. This modular approach enhances maintainability and readability.

- **Accessor and Mutator Functions:** Well-defined accessor functions allow access to maze properties, while mutator functions facilitate dynamic updates, such as setting walls, exploring boxes, and modifying costs.

- **FloodFill Functionality:** The class incorporates flood-fill algorithms for maze exploration. The `floodFill` function efficiently calculates the cost of reaching each box, aiding in pathfinding optimization.

## Mouse Class

### Design Highlights:

- **Directional Management:** The `Mouse` class handles its orientation intelligently, utilizing directional enums and helper functions for smooth navigation. This design simplifies turning and movement operations.

- **Sensor Integration:** The mouse employs sensors to detect walls in its surroundings. Sensor data is processed to make informed decisions during maze traversal, enhancing adaptability to different maze configurations.

- **Dynamic Movement:** The mouse is designed to move dynamically based on its current direction and sensor input. This allows for responsive navigation, adapting to maze changes in real-time.

- **Dead-End Detection:** The mouse can identify dead-end situations, which can occur in two ways:

  - **Physical Trap:** The mouse recognizes a dead end when all adjacent boxes have walls, making further movement impossible. In this case, the mouse backtracks to explore alternative paths.

  - **Higher Costs in Adjacent Squares:** A dead end is also detected when the costs of adjacent boxes are higher than the current box's cost. The mouse intelligently identifies such scenarios and adjusts its path to explore more promising routes.

## Advantages of the Design:

1. **Modularity and Extensibility:** The modular design of the `Maze` class allows for easy extensions or modifications without affecting other components. New functionalities can be added without major disruptions.

2. **Efficient Pathfinding:** The use of flood-fill algorithms and intelligent decision-making in the `Mouse` class ensures that the algorithm finds an optimal path through the maze, minimizing exploration time.

3. **Readable and Maintainable:** The codebase emphasizes readability and maintainability through descriptive function names, well-commented code, and a consistent coding style.

4. **Adaptability:** The mouse's reliance on sensor data makes it adaptable to various maze configurations. It can navigate through mazes of different sizes and layouts.

5. **Algorithmic Intelligence:** The mouse exhibits intelligent decision-making, such as identifying dead ends and choosing optimal paths, making it suitable for complex maze-solving scenarios.


# Maze Solver Simulation

## Overview

The Micromouse Maze Solver Simulation is a tool designed to facilitate testing and visualization of the maze-solving algorithm developed for Micromouse robotics competitions. The simulation allows users to input custom maze configurations, including walls, and observe the algorithm's behavior in real-time. Key features include a visual representation of the maze, tracking the mouse's position, displaying explored areas, and highlighting the current best path.

## Features

1. **Customizable Maze Input:**
   - Users can input maze configurations by setting walls in a visual interface.
   - Provides flexibility to create diverse maze layouts for testing.

2. **Real-Time Visualization:**
   - The simulation provides a dynamic display of the maze, updating in real-time as the algorithm progresses.
   - Users can observe the mouse's movement, areas explored, and the evolving best path.

3. **Algorithm Testing:**
   - Enables thorough testing of the maze-solving algorithm under various conditions.
   - Users can assess the algorithm's performance and make informed adjustments.

4. **User-Friendly Interface:**
   - Intuitive controls for maze configuration and simulation execution.
   - Easy-to-understand visual cues for the mouse's actions and the state of the maze.

## Usage

1. **Setting Up the Maze:**
   - Use the maze editor to define walls and configure the maze layout.
   - Ensure a clear start and finish point for the mouse.

2. **Running the Simulation:**
   - Initiate the simulation to observe the algorithm's execution.
   - Visualize the mouse's movement, exploration of squares, and the evolving solution path.

3. **Analyzing Results:**
   - Assess the effectiveness of the maze-solving algorithm based on the visual feedback.
   - Make necessary adjustments to optimize navigation strategies.

## Advantages

- **Isolated Testing Environment:**
  - The simulation provides a controlled environment for testing without external variables.
  - Ideal for fine-tuning the algorithm before real-world implementation.

- **Visual Debugging:**
  - Real-time visualization aids in identifying potential issues or inefficiencies in the algorithm.
  - Allows users to debug and optimize the solution visually.

- **Scenario Exploration:**
  - Users can simulate various scenarios by adjusting maze configurations.
  - Evaluate how the algorithm responds to different maze layouts and challenges.

