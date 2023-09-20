## Documentation
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Contributing

Please read our [Contribution Guidelines](CONTRIBUTING.md) before contributing to this project.


### Introduction

The "Tic Tac Toe" game is an open-source two-player game played on a 3x3 grid. This project demonstrates various programming concepts and is available for community contributions under the MIT License. It covers topics such as lambda expressions, classes, object-oriented programming, exception handling, conditional statements, loops, and the use of external libraries like `tabulate`.

### Installation

To get started, you need to install the `tabulate` module. You can do this using pip:

```
pip install tabulate
```

### Usage

1. **Start the Game**
   - Run the `Main()` constructor from the `main.py` file to begin the game:

     ```python
     from main import Main

     Main()
     ```

2. **Game Menu**
   - The game presents a menu with the following options:
     - Play game
     - View score card
     - Quit

#### Play game

- Choose option 1 to play the game.
- Enter the number of matches you want to play and start playing.
- After each match, the result will be displayed on the screen.

#### View score card

- Choose option 2 to view the score card.
- The score card will display the following statistics:
  - Number of matches played
  - Number of matches won by player X
  - Number of matches won by player O
  - Number of draws

#### Quit

- Choose option 3 to quit the game.

### Classes

#### Game

- `__init__`: Initializes the game board and the win conditions for player X and player O.
- `play_game`: Draws the board and takes input from the user.
- `draw_board`: Draws the current state of the board using the `tabulate` module.
- `play_move`: Places the mark of the current player on the board, updates the game board, and draws the updated board.
- `input`: Takes user input, validates it, and makes a move if the input is valid. It also checks if the game has ended.
- `draw_condition`: Checks if the game has ended in a draw.
- `wins`: Checks if the game has ended and returns the winner (1 for X, 0 for O, -1 for no winner).
- `gameNotFinished`: Checks if the game is still ongoing.
- `is_unplayable`: Checks if the game is in an impossible state (both X and O have won, or the difference between X and O moves is greater than 1).
- `diagonalMat`: Returns the two diagonals of the board.
- `colMat`: Returns the columns of the board.
- `countX`: Counts the number of 'X' marks on the board.
- `countO`: Counts the number of 'O' marks on the board.
- `has_empty_cells`: Checks if the board has any empty cells.

#### Main

- `__init__`: The constructor initializes the game menu loop.
- `play`: Plays a specified number of games, tracks scores, and prints game results.
- `score_card`: Displays game statistics in a tabular format.
- `greet_user`: Displays a welcome message and the game menu.
- `add_score`: Updates game statistics (total games played, X wins, O wins, draws).
- **Open Source**: This project is open source and welcomes contributions from the community under the MIT License.
