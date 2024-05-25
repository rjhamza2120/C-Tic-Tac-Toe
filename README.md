Project Description:
    This project is a console-based implementation of the classic Tic-Tac-Toe game developed in C++. It allows two players to play against each other on a 3x3 grid. The game alternates turns between Player 1 (X) and Player 2 (O) until there is a winner or a draw. The game provides an engaging and interactive way to practice basic C++ programming concepts such as arrays, conditionals, loops, and functions.

Features:
    Dynamic Board Display: The game board updates in real-time after each move.
    Turn-Based Gameplay: Players take turns to place their marks (X or O) on the board.
    Input Validation: Ensures that players cannot select already occupied spaces.
    Win/Draw Detection: Determines and announces the winner or if the game is a draw.
    
How to Play:
    Starting the Game: Run the program to start the game.
    Player Turns: Players will be prompted to enter the number corresponding to the cell they want to mark.
    Win/Draw Conditions: The game will check for a win or draw after each move and will announce the result accordingly.
    
Code Explanation:
    Global Variables
    board[3][3]: A 2D array representing the Tic-Tac-Toe board.
    turn: A char variable indicating the current player ('X' or 'O').
    row, column: Integer variables to store the chosen cell's row and column.
    draw: A boolean variable to indicate if the game ended in a draw.
    
Functions:
    
    void display_board()
    Displays the current state of the board. Clears the screen and prints the board along with player information.
    
    void player_turn()
    Handles the player's turn. Prompts the player to enter their choice, validates the input, updates the board, and switches the turn to the other player.
    
    bool game_over()
    Checks if the game is over by looking for a winning combination or a draw. Returns true if the game should continue, false if it has ended.
    
    Main Function
    The main function runs a loop that continues to display the board and handle player turns until the game is over. It then announces the result of the game.

How to Compile and Run
Compile the Code:

bash
Copy code
g++ -o tic_tac_toe tic_tac_toe.cpp
Run the Executable:

bash
Copy code
./tic_tac_toe
Example Output
mathematica
Copy code
   *** T I C - T A C - T O E ***   

 Player 1 = [X] 
 Player 2 = [O] 

        |    |    
      1 |  2 |  3 
    ____|____|____
        |    |    
      4 |  5 |  6 
    ____|____|____
        |    |    
      7 |  8 |  9 
        |    |    

    Player 1 [X] turn: 5

   *** T I C - T A C - T O E ***   

 Player 1 = [X] 
 Player 2 = [O] 

        |    |    
      1 |  2 |  3 
    ____|____|____
        |    |    
      4 |  X |  6 
    ____|____|____
        |    |    
      7 |  8 |  9 
        |    |    

    Player 2 [O] turn: 1

   *** T I C - T A C - T O E ***   

 Player 1 = [X] 
 Player 2 = [O] 

        |    |    
      O |  2 |  3 
    ____|____|____
        |    |    
      4 |  X |  6 
    ____|____|____
        |    |    
      7 |  8 |  9 
        |    |    

    ...
Future Enhancements
Implementing a single-player mode with AI.
Adding a graphical user interface (GUI) for better user experience.
Enhancing input validation and error handling.
