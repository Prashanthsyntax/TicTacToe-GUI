<h1>Tic Tac Toe Game</h1>
This project is a simple implementation of the classic Tic Tac Toe game using Python and the Tkinter library. The game features a 3x3 grid and supports two players, alternating between "X" and "O". It allows for user interactions with a graphical interface and displays a winner or draw notification at the end of each game.

Table of Contents
Features
Requirements
Installation
Usage
Code Overview
Features
Graphical User Interface (GUI): Built with Tkinter, providing an intuitive interface for players.
Two-Player Gameplay: The game alternates between two players, one using "X" and the other "O".
Win Detection: Automatically checks for a win after each move.
Draw Detection: Ends the game as a draw if all cells are filled without a winner.
Interactive Buttons: Each button in the grid represents a cell; clicking it updates the grid with the player's symbol.
Requirements
Python 3.x
Tkinter library (included with most Python installations)
Installation
Make sure you have Python installed. Download it from Python.org if needed.

Clone or download this repository.

Run the program with:

bash
Copy code
python tic_tac_toe.py
Usage
Run the program to open the Tic Tac Toe window.
Player "X" begins the game, clicking on any cell to place their mark.
Players alternate turns until:
One player has three marks in a row (horizontally, vertically, or diagonally), winning the game.
The grid is fully occupied without a winner, resulting in a draw.
Code Overview
Class TicTacToe
The core functionality is encapsulated in the TicTacToe class, which includes methods for initializing the game, handling moves, checking for a winner, and detecting a draw.

__init__: Sets up the initial game state, including the window, player turn, and an empty 3x3 board.
make_move(row, col): Handles the player's move, updating the board and button text and checking for win/draw conditions.
check_winner(player): Checks if the specified player has won by evaluating rows, columns, and diagonals.
is_draw(): Checks if all cells are filled without a winner, indicating a draw.
run(): Starts the Tkinter main event loop, running the game.
Example Code Execution
python
Copy code
game = TicTacToe()
game.run()
This example code creates a new Tic Tac Toe game instance and starts it.

License
This project is open-source and free to use for educational or personal projects.

