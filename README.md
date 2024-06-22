
# Candy Crush Clone

This project is a simple console-based clone of the popular game Candy Crush. It uses backtracking to generate the game board and manage moves and scoring.

## Features

- **Dynamic Board Size:** The game allows you to specify the size of the board (NxN).
- **Random Tile Generation:** Tiles are randomly generated with a specified maximum number of different types.
- **Move Validation:** The game checks for valid moves and scoring structures.
- **Scoring System:** The game calculates and displays the score based on the cleared tiles.

## Getting Started

### Prerequisites

- A C++ compiler (e.g., GCC)
- Basic understanding of C++ and console-based applications

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/candy-crush-clone.git
   cd candy-crush-clone
   ```

2. **Compile the game:**
   ```sh
   g++ -o candy_crush_clone main.cpp
   ```

3. **Run the game:**
   ```sh
   ./candy_crush_clone
   ```

## How to Play

1. **Enter the board dimensions:**
   ```
   The board dimension: 
   ```
   Specify the size of the board (N).

2. **Enter the maximum number of tile types:**
   ```
   The maximum amount of color on the board: 
   ```
   Specify the number of different tile types (D).

3. **Enter the seed for random number generation:**
   ```
   Seed for generation of pseudo-random numbers, any integer value: 
   ```
   Specify a seed value for reproducible randomization.

4. **Make moves:**
   ```
   Source row: 
   Source column: 
   Target row: 
   Target column: 
   ```
   Enter the coordinates for the source and target positions to swap tiles.

5. **Score and Board Updates:**
   The game will display the score after each valid move and update the board.

6. **Game Over:**
   The game ends when no valid moves are available.
   ```
   End of the game.
   Total score: 
   ```

## Code Overview

### `main.cpp`

The main C++ file contains the logic for the game, including:

- **Board Initialization:** Allocates memory for the board and sets edges.
- **Tile Generation:** Uses backtracking to generate a board without initial scoring structures.
- **Move Validation:** Ensures that moves are valid and checks for scoring structures.
- **Scoring System:** Calculates and updates the score based on cleared tiles.
- **Game Loop:** Manages the main game loop, user input, and board updates.

### Functions

- `allocateBoard()`: Allocates memory for the board and initializes edges.
- `ConstructBoard()`: Generates the board using backtracking.
- `ImprimeBoard()`: Prints the current state of the board.
- `Movepart()`: Executes a move and updates the board.
- `calculatePunctuation()`: Calculates the score based on cleared tiles.
- `ReConstructBoard()`: Re-generates parts of the board as needed.
- `movementisvalid()`: Checks if a move is valid.
- `ExistMovement()`: Checks if there are any valid moves left.

## Acknowledgments

- Inspired by the popular game Candy Crush.
- Developed for educational purposes to demonstrate backtracking and game logic in C++.
