# Sudoku Solver and Game

## Description
This project is a Sudoku solver and game implemented in Python using Pygame. It allows users to play Sudoku manually or watch an automated solver find the solution using a backtracking algorithm.

## Features
-   **Graphical User Interface (GUI):** Play Sudoku interactively through a user-friendly interface.
-   **Automated Solver:** Utilizes a backtracking algorithm to find solutions to Sudoku puzzles.
-   **Visual Feedback:** Watch the solver in action as it tries different numbers.
-   **Input Validation:** Checks if entered numbers are valid according to Sudoku rules.
-   **Sketch/Temporary Input:** Allows users to pencil in temporary numbers before confirming.
-   **Time Tracking:** Keeps track of the time spent on a puzzle.
-   **Strike Counter:** Counts incorrect permanent entries.

## Files
-   **`GUI.py`:** Manages the graphical user interface using Pygame, handles user interactions (mouse clicks, keyboard inputs), and integrates the solver logic to display the game. It's the main file to run the game.
-   **`solver.py`:** Contains the core backtracking algorithm for solving Sudoku puzzles. It includes functions to find empty cells, check the validity of numbers in rows, columns, and 3x3 subgrids.
-   **`solver (text).py`:** A command-line based Sudoku solver. This provides a simpler, non-GUI way to solve Sudoku puzzles.

## How to Run
1.  **Prerequisites:**
    *   Ensure you have Python 3 installed.
    *   Install the Pygame library: `pip install pygame`
2.  **Running the Game:**
    *   Open your terminal or command prompt.
    *   Navigate to the directory where you cloned or downloaded this project.
    *   Run the GUI version of the game using the command: `python GUI.py`
3.  **Running the Text-Based Solver (Optional):**
    *   If you wish to use the text-based solver, you can modify `solver (text).py` to include a board and run it: `python "solver (text).py"`

## Controls (GUI)
-   **Select a Cell:** Click on any cell in the grid with your mouse to select it. The selected cell will be highlighted with a red border.
-   **Enter a Temporary Number (Sketch):** Once a cell is selected, press a number key (1-9) to pencil in a temporary value. This will appear as a small grey number.
-   **Confirm a Number:**
    *   After sketching a number, press the `Enter` key to make it permanent.
    *   If the number is valid and part of a correct solution path, it will be accepted.
    *   If the number is incorrect (violates Sudoku rules or leads to an unsolvable board), it will count as a "strike."
-   **Delete a Temporary Number:** Select a cell with a temporary number and press the `Delete` or `Backspace` key.
-   **Automated Solver:** Press the `Spacebar` to activate the automated solver. The GUI will visually update as the algorithm works to solve the puzzle.
-   **Quit:** Close the Pygame window to exit the game.
