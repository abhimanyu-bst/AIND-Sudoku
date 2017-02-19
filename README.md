# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: I somehow visualize naked twins as an extension to the elimintaion strategy. In elimination, we are sure that a box has a single value therefore its peers cannot have this value. Similarly, when we have two boxes which share 2 same values, we are sure that the rest of the peers cannot have any of these 2 digits. I also extended this idea (please correct me if I'm wrong) to 3 or even more boxes which share exactly same value equal to the length in consideration. 

1 box -> length 1
2 box -> length 2 (twins)
3 box -> length 3 and so on..

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: In diagonal sudoku, we added a constraint of diagonal values containing 1-9. We can simply add this to our previous constraints (1-9 in a row, column and 3*3 square). 

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

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
