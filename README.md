# Sudoku Solver using CSP 

## Project Overview

This project implements a Sudoku solver using concepts from Constraint Satisfaction Problems (CSP). The solver is capable of solving Sudoku puzzles of different difficulty levels using backtracking search along with constraint propagation techniques.

The main techniques used are:

* Backtracking Search
* Forward Checking
* AC-3 (simplified version)

---

## Input Format

The program reads Sudoku boards from text files.

Each file must:

* Contain exactly 9 lines
* Each line must have exactly 9 digits (0–9)
* 0 represents an empty cell

### Example

```
004030050
609400000
005100489
000060930
300807002
026040000
453009600
000004705
090050200
```

---

## How the Program Works

### Backtracking

The algorithm fills empty cells by trying numbers from 1 to 9 and recursively explores valid possibilities.

### Forward Checking

Before continuing deeper, the algorithm checks whether future assignments are still possible. If not, it stops early.

### AC-3 

If a cell has only one valid value, it is assigned immediately. This reduces the search space.

---

## How to Run

1. Open the code in Jupyter Notebook or any Python environment
2. Run the program
3. The program will:

   * Create input files automatically
   * Solve all Sudoku boards
   * Display results in the console

---

## Output

For each Sudoku board, the program displays:

* The solved Sudoku grid
* Number of backtracking calls
* Number of failures

---

## Files Included

* easy.txt
* medium.txt
* hard.txt
* veryhard.txt
* Python source code

---

## Key Concepts

* Constraint Satisfaction Problem (CSP)
* Backtracking Algorithm
* Forward Checking
* Constraint Propagation


