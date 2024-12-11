# Pacman - Autonomous Robot Finding <br>
## Project Overview
This project implements a navigation system for an autonomous robot (inspired by Pac-Man) to traverse a 2D grid-based maze. The robot must avoid obstacles and find a valid path to its destination using a stack-based algorithm.

## Key Features
* Maze Representation: A 2D grid where cells are marked as vacant (0) or blocked by obstacles (1). <br> 
* Pathfinding: Efficiently finds a path from a starting position to the destination, avoiding obstacles. <br> 
* Stack Utilization: Navigation is implemented using a custom stack structure. <br> 
## Classes and Functionalities
1. Maze <br>
* add_ghost(x, y): Marks a cell (x, y) as blocked. <br>
* remove_ghost(x, y): Clears a blocked cell (x, y). <br>
* is_ghost(x, y): Checks if a cell (x, y) is blocked. <br>
* print_grid(): Displays the current maze layout. <br>
2. Navigator <br>
* find_path(start, end): Finds a path from start to end using stack-based traversal. <br>
* Returns a list of coordinate pairs representing the path. <br>
* Raises an exception if no path is found. <br>
3. Stack <br>
* Custom implementation used for maintaining the traversal path. <br>
## How It Works
1. The maze is initialized as a 2D grid of user-defined dimensions. <br>
2. Obstacles can be added or removed dynamically. <br>
3. The Navigator class uses a stack to explore the grid, ensuring efficient traversal and avoiding revisiting cells. <br>
4. If a path exists, it is returned as a sequence of coordinate pairs; otherwise, an exception is raised. <br>
## Requirements
Python 3.6+
## Files
* maze.py: Contains the Maze class implementation.
* navigator.py: Contains the Navigator class implementation.
* stack.py: Contains the Stack class implementation.
* exception.py: Defines exceptions for pathfinding errors.
main.py: Test and debug your implementation.
## How to Run
1. Clone the repository.
2. Set up your maze and obstacles in main.py.
3. Call find_path(start, end) from the Navigator class.
4. Run the program using python3 main.py.
