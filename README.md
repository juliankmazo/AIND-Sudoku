# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?
A: The whole idea is to reduce our search space. So the naked twins stratey consist in
finding two boxes with the same 2 possible digits and in the same unit (row, column, square and even diagonal if the sudoku has a diagonal solution).
As soon as we find two boxes that meets the requirement, it will allow us to constrain the peers in that unit, deleting those two digits from
the peers in the unit and reducint the search space! :D

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?
A: So we have 3 strategies for doing constrain propagation. For solving the diagonal sudoku we only need to add
the diagonals as a unit. This will constrain all the boxes in the diagonals. So when we apply any of the strategies, we will remove
possible digits from it's peers, and those peers will include the diagonal if the box is in a diagonal.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in function.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.