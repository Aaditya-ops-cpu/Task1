
# Software Task 1: A-Star vs. BFS Pathfinding Challenge

This repository contains the solution for Task 1 of the Team Prometheus software recruitment process.

## Overview

The goal of this task is to implement and compare two classic pathfinding algorithms, **Breadth-First Search (BFS)** and **A\* Search**, on a pre-defined 10x10 grid. The robot must find the most efficient path from a start position to a goal (the ball), avoiding obstacles.

The A\* algorithm uses the **Manhattan Distance** as its heuristic.

## File Contents

  * `Pathfinding_Challenge.ipynb`: A single Jupyter Notebook containing all the code for this task.
      * Implementation of the BFS and A\* algorithms.
      * Code to visualize the resulting paths using `matplotlib`.
      * The final comparison of path length and nodes explored.

## How to Run

1.  Ensure you have Python and the following libraries installed:

      * `jupyter`
      * `matplotlib`
      * `numpy`

2.  Launch the Jupyter Notebook:

    ```bash
    jupyter notebook Pathfinding_Challenge.ipynb
    ```

3.  In the notebook interface, select "Run" \> "Run All Cells" to execute the code and generate the comparison and visualizations.

## Results

The script will print a comparison of the two algorithms to the console and display a plot showing the paths found by each.

### Comparison Output

Both algorithms find the same optimal path length, but A\* is significantly more efficient as it explores fewer nodes.

```
BFS Algorithm:
Path Length: 12
Nodes Explored: 58

A* Algorithm:
Path Length: 12
Nodes Explored: 23
```

### Visualization Output

The plot visually confirms that while both paths are identical, the underlying search strategy (which can be inferred from the "Nodes Explored" count) is different.
