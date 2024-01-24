# AI: Reasoning & Problem Solving Assignment 1

## Description
This repository contains an assignment completed for the university course "AI: Reasoning & Problem Solving". The purpose of the assignment is to demonstrate proficiency in implementing and understanding various AI algorithms and strategies, particularly in the context of puzzles and labyrinths.

## Implementation Details

### Game Implementation
This section is based on the game implementation provided by the professor. It forms the foundation for the exercises that follow.

### Exercise 1: BFS Modifications
- **Report the Number of Visited Nodes**: A counter was implemented to increment every time a new node is visited during the BFS traversal.
- **Report the Effective Branching Factor**: The effective branching factor is calculated as the ratio of the number of nodes generated to the number of nodes visited.

<p align="center">
  <img src="https://i.ibb.co/z7q69d1/Screenshot-2023-10-10-at-11-17-09-PM.png" alt="Screenshot 1" width="200" height="300" style="margin: 0 10px;">
</p>

### Exercise 2: A* Implementation for Sliding-Tile Puzzles
- **Sliding-tile Puzzles with A* Search**: Implemented A* search with the following heuristics:
  - **Manhattan Distance**: Computes the sum of the absolute values of the horizontal and vertical distances for each tile from its goal position.
  - **Misplaced Tiles**: Counts the number of tiles that are not in their goal position.
  - **Linear Conflict**: Incorporates the Manhattan Distance and adds a penalty for tiles that are in the correct row or column but are reversed relative to each other.
- **Report Metrics**: The number of visited nodes and the effective branching factor are reported for A* search.

<p align="center">
  <img src="https://i.ibb.co/x79QMxx/Screenshot-2023-10-10-at-11-23-31-PM.png" alt="Screenshot 1" width="200" height="300" style="margin: 0 10px;">
  <img src="https://i.ibb.co/PGwMSzj/Screenshot-2023-10-10-at-11-23-39-PM.png" alt="Screenshot 1" width="200" height="300" style="margin: 0 10px;">
</p>

### Exercise 3: Labyrinth Implementation
- **Labyrinth Class**: The class offers methods to determine the end state, retrieve the initial state, and expand possible actions.
- **Uninformed Strategy**: Bidirectional Search was implemented as the uninformed strategy. This approach conducts both forward and backward searches from the initial and goal states, respectively. The search concludes once both searches intersect.

<p align="center">
  <img src="https://i.ibb.co/F7zvKwg/Screenshot-2023-10-10-at-11-28-14-PM.png" alt="Screenshot 1" width="150" height="250" style="margin: 0 10px;">
  <img src="https://i.ibb.co/D987mJr/Screenshot-2023-10-10-at-11-29-05-PM.png" alt="Screenshot 1" width="150" height="250" style="margin: 0 10px;">
</p>

- **Informed Strategy for Labyrinth**: A* search was repurposed with a suitable heuristic tailored for pathfinding in the labyrinth.

<p align="center">
  <img src="https://i.ibb.co/9NyYHcm/Screenshot-2023-10-10-at-11-32-44-PM.png" alt="Screenshot 1" width="150" height="250" style="margin: 0 10px;">
  <img src="https://i.ibb.co/sQTM34q/Screenshot-2023-10-10-at-11-31-57-PM.png" alt="Screenshot 1" width="150" height="250" style="margin: 0 10px;">
</p>

## Performance Comparisons
A comprehensive comparison of the heuristics—Manhattan Distance, Misplaced Tiles, and Linear Conflict—was conducted for the sliding-tile puzzles. The results offer insights into the efficiency and effectiveness of each heuristic in guiding the A* search.

## Usage
To run the Jupyter notebook:
1. Clone the repository.
2. Navigate to the directory containing the notebook.
3. Run `jupyter notebook` and open `Assignment_1_GabrieldeOlaguibel.ipynb`.

## License & Acknowledgments
The assignment and base game implementation are credited to IE University and professor, Eugenio Manchiori. All third-party resources and libraries used are acknowledged within the notebook.

