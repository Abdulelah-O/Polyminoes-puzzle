# Polyominoes Puzzle Solver

## Project Overview

This project is a solver for a version of the classic Polyominoes Puzzle, which is an instance of the Exact Cover Problem. ***The objective is to find a unique collection of tiles (subsets) that perfectly covers a given board (set X) without any elements being left uncovered or overlapped.***

<img width="938" height="217" alt="image" src="https://github.com/user-attachments/assets/8ab66f62-0861-4701-ba1d-59482bf7a13e" />

## Problem Description

Given:

  - A set X representing the board, consisting of a finite number of elements.

  - A collection S of subsets of X, where each subset represents a tile.

The goal is to find a sub-collection S* of S that satisfies the following conditions:

  1. Exact Cover: The union of all subsets in S* is equal to the full set X.

  2. No Overlap: The intersection of any two distinct subsets in S* is empty.

## Files and Directories

  - CS467-Project.ipynb: The main Jupyter Notebook containing the source code for the Tabu Search algorithm and the functions to read input files and solve the problem.

  - ECP_1.txt, ECP_2.txt, ECP_3.txt, ECP_4.txt, ECP_5.txt: These are benchmark files provided as a set of problem instances for testing the solver's performance. Each file follows the specified input format.

## Input File Format

The program reads problem instances from a plain text file. The format is structured as follows:

  1. First Line: Contains the space-separated elements of set X (e.g., 1 2 3 4 5).
  2. Second Line: Contains the number of subsets in the collection S.
  3. Remaining Lines: Each line represents a subset from S, with its elements separated by spaces.

### Example Input (ECP_1.txt):

```
1 2 3 4 5
5
1 2
3 4
5
1 3
2 5
```

## How to Run

  1. Clone this repository to your local machine.
  2. Ensure you have a Python environment with Jupyter Notebook and the necessary libraries.
  3. Place your input file(s) (e.g., the ECP_*.txt files) in a directory accessible to the notebook.
  4. Open CS467-Project.ipynb in Jupyter and modify the file_path variable in the last code cell to point to your desired input file.

     ```
     file_path = "path/to/your/ECP_1.txt"
     ```
  5. Run all the cells in the notebook. The output will be printed directly below the code cell.
     


## Output

The program will print the subsets that form the solution if one is found. If no exact solution is discovered, it will indicate the best non-exact solution found and its cost.

## Contributors

  - Abdulelah Bin Obaid
  - Feras Aldawsari
  - Rami Alraugi

