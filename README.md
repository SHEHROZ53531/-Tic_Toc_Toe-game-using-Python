# -Tic_Toc_Toe-game-using-Python
TIC-TOC_TOE Game using python.
Functions:

sum(a, b, c): Adds three values and returns the sum. It's used to check if any player has achieved a winning condition.
printBoard(xState, zState): Displays the current state of the game board, showing X for Player 1, O for Player 2, and numbers for unoccupied positions.
checkwin(xState, zState): Checks if any player has won by matching their positions with predefined winning combinations.
Winning Combinations: The checkwin function uses the wins list, which contains all possible winning combinations of indices on the board:

[[0, 1, 2], [3, 4, 5], [6, 7, 8], 
 [0, 3, 6], [1, 4, 7], [2, 5, 8], 
 [0, 4, 8], [2, 4, 6]]
If any player's moves match one of these combinations, the game announces the winner.

Game Flow:

The game begins with an empty board and a prompt to the players.
Players take turns entering a number (0–8) to mark their moves.
After each move:
The game board is updated.
It checks for a winner using checkwin.
If a player wins, the game ends, and a message is displayed.
If there's no winner yet, the turn alternates to the other player.
Main Logic:

xState and zState are arrays of size 9, representing the board's state for Player 1 (X) and Player 2 (O), respectively. A 1 in an index indicates a marked position.
turn determines which player's move it is: 1 for Player 1 (X) and 0 for Player 2 (O).
How to Play
Run the program.
Players take turns selecting a number (0-8) corresponding to a position on the board:
diff
Copy code
0 | 1 | 2
--|---|--
3 | 4 | 5
--|---|--
6 | 7 | 8
Player 1 uses X and Player 2 uses O.
The game ends when one player achieves a winning combination or when all positions are filled without a winner.

