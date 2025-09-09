# Polyominoes Puzzle Solver

## Project Overview

This project is an efficient solver for a version of the classic Polyominoes Puzzle. ***The goal is to find a collection of tiles (subsets) that completely covers a given board (set X) without any overlapping. This is a classic Exact Cover Problem, a well-known NP-complete problem that is often solved using metaheuristics.***

<img width="938" height="217" alt="image" src="https://github.com/user-attachments/assets/8ab66f62-0861-4701-ba1d-59482bf7a13e" />

## Problem Description

  - A set **X** (the board)
  - A collection **S** of subsets of **X** (the tiles)

The objective is to find a sub-collection **S*** of **S** such that:

  1. The union of all subsets in **S*** is equal to **X**.
  2. The intersection of any two distinct subsets in **S*** is empty.

## Input File Format

The program should be able to read the problem instances from a plain text file. The format is as follows:

  1. First Line: Describes the components of set X (e.g., 1 2 3 4 5).
  2. Second Line: The number of subsets in the collection S (e.g., 5).
  3. Remaining Lines: Each line describes the contents of a subset (one per line).

## Example Input

```
1 2 3 4 5
5
1 2
3 4
5
1 3
2 5

```

## Output

The program should print the subsets that form the solution if one exists. If no solution can be found, it should indicate that there is no solution.

