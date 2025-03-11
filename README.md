# N-Queens-Problem

Overview
This project provides a Python program to solve the N-Queens problem using Backtracking. The N-Queens problem is about placing N queens on an N×N chessboard so that no two queens attack each other.

How It Works (Step by Step Execution)
--> Create the Board:

A N×N board is created with 0, meaning empty spaces.

1 means a queen is placed in that spot.

--> Placing the Queens Using Backtracking:

Start from the first row and try placing a queen in each column.

Check if the position is safe (no queen in the same column, row, or diagonals).

If safe, place the queen (1) and move to the next row.

If no safe position is found in a row, go back to the previous row and try a different column.

Repeat until all queens are placed correctly.

--> Printing Solutions:

Once a valid placement is found, it is saved and printed.

The program continues to find more solutions if they exist.

Algorithm Used
The program uses Backtracking, which works as follows:

Try placing queens one by one: Start with an empty board and place queens row by row.

Check for safety: Before placing a queen, ensure it does not conflict with others.

Backtrack if needed: If a queen cannot be placed in a row, go back to the previous row and try a different column.

Repeat until all queens are placed correctly.

Understanding 0 and 1 in the Board
0: Represents an empty space where no queen is placed.

1: Represents a queen's position on the board.

The board updates as queens are placed (1) and removed (0) during backtracking.

Performance
The time complexity is O(N!), meaning it takes longer for larger N.

Works well for N ≤ 15. For very large N, other methods like Hill Climbing or Genetic Algorithms might be faster.

How to Run
Install Python if not already installed.

--> Clone this repository:

git clone https://github.com/Ritu8701raj/n-queens-solver.git 
cd n-queens-solver

--> Run the script:

python n_queens_solver.py

Change n in the script to solve for different board sizes.

Example Output (for N=8)
Q . . . . . . . . . . . Q . . . . . . . . . . Q . . . . . Q . . . . Q . . . . . . . . . . . Q . . Q . . . . . . . . . Q . . . .

Total solutions for 8-Queens: 92

Contributions
Feel free to submit issues, suggestions, or pull requests to improve this project!
