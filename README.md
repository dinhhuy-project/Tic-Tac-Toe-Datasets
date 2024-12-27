# Tic-Tac-Toe-Datasets
- boards.csv
+ id         
// Unique ID
+ cells      
// Cells of the game board 
// Left-to-right and top-to-bottom 
// Can be 'X', 'O', or 'E' for empty
+ symmetries 
// If another board was excluded based on this board, 
// how was it similar? (duplicate/symmetrical) 
// 'duplicate', 'rotational', or 'reflectional'
+ parents    
// List of game board IDs that preceeded this one
+ children   
// List of game board IDs that followed this one
+ result     
// Game result
// 'false' if the game is ongoing
// 'X', 'O', or 'draw' if the game is over
+ level      
// Game move (0–9)

- tic-tac-toe.csv
+ This datasets encodes the complete set of possible board configurations at the end of tic-tac-toe games, where "x" is assumed to have played first.  The target concept is "win for x" (i.e., true when "x" has one of 8 possible ways to create a "three-in-a-row").  

- tictactoe_games.csv
This dataset contains 255,168 records of Tic-Tac-Toe games. The dataset is structured to represent every possible game sequence where:
+ Player X always starts first.
+ The game continues until there is a winner or a draw.
+ All positions on the board (0,0 through 2,2) are treated as unique—no symmetry optimizations have been applied.
Each row in the dataset represents a complete game, detailing each move and the final outcome.