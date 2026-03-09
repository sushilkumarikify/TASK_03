# TASK_03



# Sudoku Solver (C++)

## Project Description

This project implements a **Sudoku Solver using C++ and the Backtracking Algorithm**.
The program automatically solves a 9×9 Sudoku puzzle by filling in the missing numbers while ensuring that all Sudoku rules are satisfied.

The solver checks each empty cell and recursively tries possible numbers until the puzzle is solved.

---

## Features

* Solves standard **9×9 Sudoku puzzles**
* Uses **Backtracking Algorithm**
* Validates Sudoku constraints:

  * Row constraint
  * Column constraint
  * 3×3 subgrid constraint
* Console-based output
* Efficient recursive solving approach

---

## How It Works

1. The Sudoku grid is represented using a **2D array (9×9)**.
2. Empty cells are represented by **0**.
3. The program searches for an empty cell.
4. It tries numbers **1 to 9** in that cell.
5. Before placing a number, it checks:

   * If the number already exists in the **row**
   * If the number already exists in the **column**
   * If the number exists in the **3×3 subgrid**
6. If valid, the number is placed and the solver moves to the next empty cell.
7. If no valid number can be placed, the algorithm **backtracks** and tries another possibility.

---

## Sudoku Rules Implemented

A number can only be placed if:

* It does **not appear in the same row**
* It does **not appear in the same column**
* It does **not appear in the same 3×3 box**

---

## Example Input Grid

```
5 3 0 0 7 0 0 0 0
6 0 0 1 9 5 0 0 0
0 9 8 0 0 0 0 6 0
8 0 0 0 6 0 0 0 3
4 0 0 8 0 3 0 0 1
7 0 0 0 2 0 0 0 6
0 6 0 0 0 0 2 8 0
0 0 0 4 1 9 0 0 5
0 0 0 0 8 0 0 7 9
```

---

## Example Output

```
Solved Sudoku:

5 3 4 6 7 8 9 1 2
6 7 2 1 9 5 3 4 8
1 9 8 3 4 2 5 6 7
8 5 9 7 6 1 4 2 3
4 2 6 8 5 3 7 9 1
7 1 3 9 2 4 8 5 6
9 6 1 5 3 7 2 8 4
2 8 7 4 1 9 6 3 5
3 4 5 2 8 6 1 7 9
```

---

## Project Structure

```
Sudoku-Solver/
│
├── sudoku_solver.cpp
└── README.md
```

---

## How to Compile

Use a C++ compiler such as **g++**.

```bash
g++ sudoku_solver.cpp -o sudoku_solver
```

---

## How to Run

After compiling, run the program:

```bash
./sudoku_solver
```

---

## Technologies Used

* C++
* Recursion
* Backtracking Algorithm
* 2D Arrays
* Console-based application

---

## Possible Improvements

Future enhancements for this project:

* Allow **user input for Sudoku puzzle**
* Add **Graphical User Interface (GUI)**
* Support **different Sudoku sizes**
* Improve solving speed with **optimization techniques**

---

## Learning Outcomes

Through this project, I learned:

* Implementation of **Backtracking Algorithms**
* Use of **recursion in problem solving**
* Handling **2D arrays in C++**
* Applying **constraint checking algorithms**

