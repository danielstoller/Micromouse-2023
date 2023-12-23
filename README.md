# Mouse Maze Solver

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

## Getting Started

To utilize the Mouse Maze Solver, follow the instructions in the documentation to integrate the classes into your project. Sample mazes and test cases are provided to showcase the capabilities of the solver.

