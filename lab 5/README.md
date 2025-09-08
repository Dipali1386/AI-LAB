C++ Tic-Tac-Toe Game with AI
This is a classic Tic-Tac-Toe game implemented in C++. You play against an AI opponent that uses the Minimax algorithm with Alpha-Beta pruning to make optimal moves. This ensures the computer will never lose a game if you both play optimally; it will either win or draw.

✨ Features
Human vs. AI Gameplay: Play a one-on-one match against an intelligent AI.

Unbeatable AI: The AI uses the Minimax algorithm with Alpha-Beta pruning, guaranteeing the most strategic move possible.

Simple, Clear Interface: The game is played via the console with a clear and easy-to-understand board layout.

⚙ How to Compile and Run
Prerequisites
You need a C++ compiler installed on your system, such as g++

 How to Play
When you run the game, a 3x3 board will be displayed.

The board positions are numbered 1 through 9.

You are player 'X', and the computer is 'O'.

Enter the number of the position (1-9) where you want to place your 'X'.

The computer will then make its move.

The game ends when one player wins by getting three of their marks in a row (horizontally, vertically, or diagonally) or when all squares are filled, resulting in a draw.

🧠 AI Explained (Minimax with Alpha-Beta Pruning)
The core of this program is the MinMax function, which implements the Minimax algorithm.

Minimax: This is a recursive algorithm used for decision-making in two-player games. It evaluates all possible moves to determine the optimal one. It assumes both players are playing optimally, with the AI trying to maximize its score and the human player trying to minimize it.

Alpha-Beta Pruning: This is an optimization technique for the Minimax algorithm. It allows the algorithm to "prune" or cut off branches of the game tree that it knows will not lead to an optimal move, significantly reducing the number of states it has to evaluate. This makes the AI's move calculation much faster without affecting its performance.

The AI evaluates each possible move by simulating the entire game from that point onward, assigning a score to each final outcome:

+1 if the human wins.

-1 if the AI wins.

0 if the game is a draw.

The AI then chooses the move that leads to the lowest possible score for the human player (the highest score for itself).