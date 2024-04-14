# Solving the Sliding Puzzle in Python

This program implements algorithms to solve the sliding puzzle, a classic board game.

## Module Imports

The code uses three Python modules:

- `collections.deque` for implementing queues.
- `random` for shuffling the tiles of the puzzle.
- `heapq` for managing the priority queue in the A* algorithm.

## Main Functions

### initial_list(degree)

This function creates an initial grid for the sliding puzzle.

- **Parameter**: `degree` - the size of the grid.
- **Returns**: A square grid in the form of a list of lists with numbered tiles and an empty space (0).

### display(board)

This function displays the puzzle grid in a formatted manner.

- **Parameter**: `board` - the puzzle grid to display.

### shuffle_list(list)

This function shuffles the tiles in the puzzle grid.

- **Parameter**: `list` - the puzzle grid.
- **Returns**: A shuffled grid.

### find_empty(board)

This function finds the position of the empty space in the grid.

- **Parameter**: `board` - the puzzle grid.
- **Returns**: The coordinates of the empty space.

### generate_next_states(board, i, j)

This function generates all possible states from the current state by moving the empty space.

- **Parameters**: `board` - the current state, `i`, `j` - position of the empty space.
- **Returns**: List of possible states after a move.

### bfs(initial_board, target_board)

This function implements the breadth-first search (BFS) algorithm.

- **Parameters**: `initial_board` and `target_board`.
- **Returns**: Path from the initial state to the target state, if it exists.

### dfs(initial_board, target_board, depth_limit)

This function implements the depth-first search (DFS) algorithm with a depth limit.

- **Parameters**: `initial_board`, `target_board`, `depth_limit`.
- **Returns**: Path from the initial state to the target state, if it exists.

### heuristic(board, target_board)

This function calculates the number of misplaced tiles.

- **Parameters**: `board` and `target_board`.
- **Returns**: Number of misplaced tiles.

### a_star(initial_board, target_board)

This function implements the A* algorithm to solve the puzzle.

- **Parameters**: `initial_board` and `target_board`.
- **Returns**: Path from the initial state to the target state, if it exists.

### solve_puzzle_bfs(degree)

### solve_puzzle_dfs(degree)

### solve_puzzle_A(degree)

These functions solve the sliding puzzle using the BFS, DFS, and A* algorithms respectively.

- **Parameter**: `degree` - the size of the puzzle grid.
- **Behavior**: Displays the solution path, if it exists.

## Program Usage

To use the program, simply choose the grid size and the resolution algorithm, then execute the corresponding function. The program will display the shuffled grid and attempt to find a path to the target configuration.

## 🗓️ CompletionDate

November 28, 2023