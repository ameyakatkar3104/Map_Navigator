# Map_Navigator

## Objective: 
The Map Navigator is designed to find a path from a starting point to a destination in a grid map using the backtracking algorithm. This implementation in C++ involves navigating through a grid with obstacles, finding a valid path, and ensuring all possible routes are explored efficiently.

## Key Features:
1. **Grid Representation:**

    - The map is represented using a 2D array int map[ROWS][COLS].
      - Each cell in the array can hold:
      - 0 for an open path.
      - 1 for an obstacle.
      - S for the start point.
      - D for the destination.
2. **Backtracking Algorithm:**

    - The backtracking algorithm is used to explore all possible paths from the starting point to the destination.
    - It recursively tries to move in four possible directions (up, down, left, right).
    - If a move is valid, it proceeds to the next cell.
    - If a move leads to an invalid path or a dead end, the algorithm backtracks to the previous cell and tries another direction.
3. **Validation:**

    - Functions are used to check if a move is valid:
      - Boundary Check: Ensures the move stays within the grid boundaries.
      - Obstacle Check: Ensures the move does not land on an obstacle.
      - Visited Check: Ensures the move does not revisit a previously visited cell.
4. **Path Storage:**

    - A path array path[ROWS][COLS] is used to store the current path being explored.
    - Successful paths are stored and printed.
## Implementation Details:
1. **Grid Initialization:**

    - The grid is initialized with predefined obstacles, starting point, and destination.
2. **Path Finding:**

    - The findPath() function implements the backtracking algorithm.
    - It uses the isValidMove() function to check if the next move is valid.
    - If a valid path to the destination is found, it is stored and printed.
3. **Printing the Path:**

    - The printPath() function prints the current state of the grid with the path.


  
