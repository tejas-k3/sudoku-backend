# sudoku-backend
Backend for Sudoku Game

# Sudoku Requirements
- When a req with body "START" is sent to API , it must send response "READY" after resetting the game of Sudoku and starting a fresh game.
- When a number is entered, it should return "VALID" or "INVALID"
- Any method can be used for Move Insertion. GET /move/row/col or POST /move with row and column as body or any other way
- Sudoku skeleton can set in the backend or taken in the req form from the user.

# Advance
- The API must return a suggested move after 3 consecutive invalid responses.
- Game should continue until the sudoku is solved.


# Steps involved
- Define the Sudoku game logic: Implement the necessary classes and methods to represent and handle the Sudoku game. This includes the Sudoku grid, methods for validating moves, resetting the game, and generating suggested moves.
- Define an API endpoint to start a new game. When a request with the body "START" is received, reset the game, start a fresh game, and send a response with "READY".
- Define an API endpoint to handle moves. This can be a POST endpoint where the row and column are sent as the request body, or any other suitable approach. Validate the move and return "VALID" or "INVALID" based on the move's correctness.
- Implement the logic to suggest a move after three consecutive invalid responses. Keep track of the number of consecutive invalid moves and generate a suggested move accordingly.
- Implement the game completion logic: Keep track of the Sudoku grid's state and determine when the game is solved. You can use a backtracking algorithm or any other suitable approach to solve the Sudoku puzzle.

