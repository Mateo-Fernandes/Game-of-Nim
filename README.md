# Game-of-Nim
basic game of nim

Game of Nim
Overview
The Game of Nim is a mathematical game of strategy where players take turns removing objects from piles. The objective is to not be the player who removes the last object. This program allows for two gameplay modes:

Player vs Player: Two human players play against each other.
Player vs AI: A human player competes against an AI opponent that follows an optimal strategy.
This implementation uses Python and runs in a Command-Line Interface (CLI).

How to Play
The game starts with 3 piles of random objects (sizes range between 1 and 7), but the starting configuration cannot be [1, 1, 1].
Players take turns removing objects from one pile at a time:
Choose a pile.
Decide how many objects to remove (at least 1 and at most the number of objects in the chosen pile).
Losing Condition: The player who takes the last object loses the game.
Requirements
Python 3.x installed on your system.
Running the Game
Follow these steps to run the game:

Download the Code: Save the Python code in a file named game_of_nim.py.

Run the Code: Open your terminal or command prompt and navigate to the folder containing the file. Run the following command:

python game_of_nim.py

Choose the Game Mode:

Press 1 for Player vs Player mode.
Press 2 for Player vs AI mode.

Gameplay:

Players (or the AI) will take turns selecting a pile and removing objects.
The current state of the piles will be displayed after each move.
End of Game:

The program announces the winner (the player who didn’t take the last object).
The CLI will pause at the end, allowing you to see the results before exiting.

Example Gameplay

Starting Game:

Welcome to the Game of Nim!
The player who takes the last object loses!
Choose game mode: (1) Player vs Player, (2) Player vs AI: 2

Current piles:
Pile 1: **** (4)
Pile 2: ***** (5)
Pile 3: *** (3)

Player 1's turn:
Choose a pile (1, 2, 3): 2
How many objects to remove? 2

Current piles:
Pile 1: **** (4)
Pile 2: *** (3)
Pile 3: *** (3)

AI's turn:
AI removes 1 object from pile 1.

Current piles:
Pile 1: *** (3)
Pile 2: *** (3)
Pile 3: *** (3)

... (Gameplay continues)
End of Game:

The AI loses! You win!

Press Enter to exit.

Features

Two Modes: Player vs Player and Player vs AI.

AI Strategy: The AI uses the Nim-sum algorithm to play optimally.

User-Friendly CLI: The current state of the game is displayed after each move.

Input Validation: Ensures players make valid moves.

Game Rules: The configuration [1, 1, 1] is not allowed at the start of the game.

How the AI Works
The AI uses the Nim-sum strategy:

The Nim-sum is calculated as the XOR of all pile sizes.
If the Nim-sum is non-zero, the AI makes an optimal move to reduce the Nim-sum to zero.
If no such move exists, the AI removes 1 object from the first non-empty pile.
This strategy ensures that the AI plays intelligently and increases the challenge for the human player.

Credits
Game concept: Traditional Game of Nim
AI strategy: Based on the mathematical Nim-sum algorithm
Developed by: Fernandes Matéo


