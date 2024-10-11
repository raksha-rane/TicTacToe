# Tic-Tac-Toe Game

## Overview

The **Tic-Tac-Toe** project is a command-line game developed in C++ where a human player competes against the computer. The game utilizes the **Minimax algorithm**, a classic artificial intelligence technique, to ensure that the computer always makes the optimal move. This creates a challenging game where the computer either wins or forces a draw.

## Features

- **Human vs. Computer**: Play against a computer opponent that uses AI to make decisions.
- **Minimax Algorithm**: The computer uses this algorithm to evaluate the best possible move in every scenario.
- **Unbeatable AI**: The algorithm ensures that the computer never loses. The game will either end in a win for the computer or a draw.
- **Command-Line Interface**: Simple and clean interface using the command line.

## Technologies Used

- **C++**: The core logic of the game is implemented in C++ for efficient handling of game states and AI decision-making.
- **Minimax Algorithm**: The AI logic is based on the Minimax algorithm, which explores all possible moves and selects the best outcome for the computer.

## How It Works

1. **Board Setup**: The game board is a 3x3 grid where each cell can hold either an 'X', 'O', or be empty.
2. **Player Turns**: The human player chooses whether to be 'X' or 'O' and takes the first or second turn.
3. **Minimax Algorithm**: On the computer's turn, it evaluates all possible moves and uses the Minimax algorithm to determine the best move to either win or force a draw.
4. **Game End**: The game ends when there is either a win or a draw. The board will be displayed after each move.

### Minimax Algorithm Explained

- **Initial Setup**: The algorithm checks all empty cells and simulates placing 'X' or 'O' in each one.
- **Maximizing and Minimizing**: The algorithm alternates between maximizing the computer’s score (for 'O') and minimizing the player’s score (for 'X').
  - A win for the computer is scored as +10.
  - A win for the player is scored as -10.
  - A draw is scored as 0.
- **Recursive Search**: The algorithm recursively explores all possible game states, backtracking to evaluate different scenarios.
- **Optimal Move**: The computer chooses the move that maximizes its chances of winning.

## Data Structures Used

- **3x3 Array (Grid Representation)**: The board is represented as a 3x3 array where each cell holds 'X', 'O', or a blank space.
- **Recursive Call Stack**: The Minimax algorithm relies on recursion to evaluate future game states.

## Getting Started

### Prerequisites
- A C++ compiler (such as g++ or clang)

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/tic-tac-toe.git
    ```

2. Navigate to the project directory:

    ```bash
    cd tic-tac-toe
    ```

3. Compile the code:

    ```bash
    g++ -o tic-tac-toe tic-tac-toe.cpp
    ```

4. Run the game:

    ```bash
    ./tic-tac-toe
    ```

## Usage

- Follow the on-screen instructions to play.
- The human player can choose to play first or second.
- Input the number corresponding to the cell where you want to place your mark ('X' or 'O').
- The computer will then make its move using the Minimax algorithm.
- The game will display the winner or declare a draw at the end.


