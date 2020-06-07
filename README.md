# Quantum_Tic-Tac-Toe
Quantum version of the game Tic-Tac-Toe

This game is a modification of the classical tic-tac-toe game. It adds a quantum flavour to the game in a way mentioned below. We took a bit of help for making our UI from this repo (https://github.com/kunalsinghal/tictactoe).

The game of Quantum tic-tic-toe is very different from the classical version of the same but still some of the basic rules remains the same. Each player take alternative turns to make their moves with player 1 starting the game and a square marked by white color belongs to player 1 and square marked by black to player 2.  To win the game, a player has to get k consecutive squares, marked by their color, in a row, column or a diagonal.  Here k is called the winning parameter which in the classical version of 3x3 tic-tac-toe is 3.  Also,the grid size of the game is NxN. Both the parameters N and k are given before the game starts.

The game is initialized by an NxN matrix M of cells where each cell is colored grey and is in the super position of the black and white state. Following are the two types of moves that a player can do.

1) Classical move : To make this move the player must choose an unmarked cell i.e. a grey cell.  After making the move, the state of the cell will be measured and hence it will collapses to black or white state. Based on the collapsed state, the color will beassigned to it.

2) Quantum move : To make this move the player must choose two cells, one marked and one unmarked cell (and therefore can’t be the first move of the game).  After making the move the cells are entangled and measuring the unmarked cell of this pair might cause the marked cell to change it's state and hence it's color. The color of the marked cell will be flipped if the unmarked cell collapses to a black state and the marked cell remain as it is if the unmarked cell collapses to a white state.

3) Hadamard move : To make this move the player must select a marked cell which is not entangeled with any other cell. After applying the move, the cell resets to it's initial grey state i.e. becomes an unmarked cell. 
