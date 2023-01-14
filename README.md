# Caro bot
From https://github.com/Cledersonbc/tic-tac-toe-minimax

## Play game
LINK: https://nxhawk.github.io/caro-bot/

## Game Tree
Below, the best move is on the middle because the max value is on 2nd node on left.

<p align="center">
	<img src="https://github.com/Cledersonbc/tic-tac-toe-minimax/blob/master/preview/simplified-g-tree.png?raw=true"></img>
</p>

Take a look that the depth is equal the valid moves on the board. The complete code is available in **py_version/**.

Simplified game tree:

<p align="center">
	<img src="https://github.com/Cledersonbc/tic-tac-toe-minimax/blob/master/preview/tic-tac-toe-minimax-game-tree.png?raw=true"></img>
</p>

That tree has 11 nodes. The full game tree has 549.946 nodes! You can test it putting a static global variable in your program and incrementing it for each minimax function call per turn.

In a more complex game, such as chess, it's hard to search whole game tree. However, Alpha–beta Pruning is an optimization method to the minimax algorithm that allows us to disregard some branches in the search tree, because he cuts irrelevant nodes (subtrees) in search. For more information, see:

* Book: George T. Heineman; Gary Pollice; Stanley Selkow. Algorithms in a nutshell. O'Reilly, 2009.
* Wikipédia: <https://en.wikipedia.org/wiki/Minimax>
