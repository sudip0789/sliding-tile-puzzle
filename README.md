# Solving sliding 8-tile puzzle using A* algorithm

This project is a digital implementation of the classic **Sliding Tile Puzzle** game. It challenges players to arrange scrambled tiles in their correct order by sliding them into the empty space. The puzzle is both an engaging pastime and an excellent test of logical thinking and spatial awareness.

![Sliding Tile Puzzle](https://github.com/sudip0789/sliding-tile-puzzle/blob/main/states.png)

The image above shows the game interface with tiles and the empty space for sliding.

## Solution using A* Algorithm

**Initialization:** Start with the initial configuration of the puzzle. Initialize the priority queue with this state and an empty dictionary to track the cost of reaching each state.

**Expand the nodes:** Expand the current state by generating all possible successor states through valid tile moves (up, down, left, right).

**Evaluate and queue:** For each successor state, calculate the cost g(n) and the heuristic h(n). If the new path to this state is shorter than any previously found, update the cost and queue the state with its f(n) value.

**Check for goal state:** Continue this process until the goal state is reached or the priority queue is empty (indicating no solution).

**Path reconstruction:** Once the goal state is reached, reconstruct the path from the initial state to the goal state by backtracking through the tracked states.

The shortest path to the goal state was achieved with a total of 27 steps for the above example. If you are interested in viewing the 27 steps taken by the algorithm then simply run this command "print(path)" on your notebook.

### For additional details, refer to the detailed [project page](https://sudipdas-projects.netlify.app/sliding-tile-puzzle/)
