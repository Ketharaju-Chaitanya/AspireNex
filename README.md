**TIC-TAC-TOE Using AI:**

**Methodology**

The goal was to create an unbeatable AI for the Tic-Tac-Toe game using the Minimax algorithm. The methodology involved the following steps:

1. Game Setup: Define the board and the rules of the game.
2. Minimax Algorithm Implementation: Implement the Minimax algorithm to evaluate the best possible moves.
3. Move Selection: Use the Minimax algorithm to determine the optimal move for the AI.
4. Game Logic: Implement the game logic, including checking for a winner or a draw and handling player moves.
5. User Interface: Develop a simple interface to allow a human player to interact with the game.
6. Game Loop: Create a loop to alternate turns between the human player and the AI, updating the game state accordingly.
   
**Working**

**1. Game Setup:**
a) The board is represented as a 3x3 grid, initially filled with empty spaces.
b) Players are represented as 'X' (human) and 'O' (AI).

**2. Minimax Algorithm:**
a) Objective: The algorithm aims to minimize the potential loss for the worst-case scenario.
b) Evaluation: Each possible move is evaluated by simulating the game to the end and assigning a score based on the outcome.
c) Recursive Function: A recursive function evaluates all possible moves for both players. The AI (maximizing player) tries to maximize the score, while the human player (minimizing player) tries to minimize it.

**3. Move Selection:** The AI uses the Minimax algorithm to choose the move that maximizes its chances of winning or drawing, never losing.
   
**4. Game Logic:**   
a) Check Winner: A function checks rows, columns, and diagonals for a winner.
b) Best Move: A function best_move is implemented to determine the optimal move for the AI

**5. User Interface:**
a) The board is printed in the console.
b) The human player inputs their moves via the console.

**6. Game Loop:**
a) The game alternates between the human player and the AI.
b) After each move, the game checks for a win or draw.
c) The game continues until there is a winner or a draw.

**Tools used:**
1. **Python**: The primary programming language used for the implementation.
2. **Console Input/Output:** For interacting with the human player and displaying the game board.
3. **Mathematical Functions:** Used in the Minimax algorithm to evaluate scores (from the math library).

-------------------------------------------------------------------------------------------------------------------------------------------------

**RECOMMENDATION SYSTEM:**

**Methodology:**

The goal was to create a recommendation system that suggests items (e.g., movies) to users based on their preferences using collaborative filtering. 
The methodology involved the following steps:

1. Data Preparation: Generate a dataset of user-item interactions with random ratings.
2. User-Item Matrix: Create a matrix where rows represent users and columns represent items, with values representing user ratings.
3. Compute User Similarity: Calculate the similarity between users using cosine similarity.
4. Generate Recommendations: Aggregate ratings from similar users to recommend items to the target user.

**Working:**

**1. Data Preparation:**
   a) Define lists of users and items.
   b) Generate random ratings for a subset of user-item pairs to simulate a real-world scenario where not all users rate all items.
   c) Store the data in a pandas DataFrame.

**2. User-Item Matrix:**
   a) Create a matrix using pivot_table in pandas where rows are users and columns are items.
   b) Fill missing ratings with zeros to handle the sparsity of the data.

**3. Compute User Similarity:**
   a) Convert the user-item matrix to a sparse matrix format for efficient computation.
   b) Use cosine similarity to compute the similarity between user vectors, resulting in a user similarity matrix.

**4. Generate Recommendations:**
   a) For a given user, identify the most similar users based on the similarity scores.
   b) Aggregate the ratings from these similar users for each item.
   c) Recommend items that the target user has not rated but are highly rated by similar users.

**Tools used:**
1. **Python:** The primary programming language used for the implementation.
2. **pandas:** For data manipulation and creating the user-item matrix.
3. **NumPy:** For numerical operations and random rating generation.
4. **scikit-learn:** For computing cosine similarity between users.
5. **SciPy:** For handling sparse matrices efficiently.

