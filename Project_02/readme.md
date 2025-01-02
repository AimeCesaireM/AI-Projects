# Multi-Agent Pacman AI

This project implements several artificial intelligence algorithms for Pacman, including reflex agents, minimax, alpha-beta pruning, and expectimax. It uses multi-agent search techniques to make decisions in a Pacman game environment. The goal is to help Pacman navigate through the maze, collect food, and avoid ghosts.

## Project Structure

- **multiAgents.py**: Contains the implementation of various agents, including the ReflexAgent, MinimaxAgent, AlphaBetaAgent, and ExpectimaxAgent.
- **game.py**: Provides the game environment and utilities for the agents to interact with the game world.
- **util.py**: Includes utility functions such as Manhattan distance calculation.

## Algorithms Implemented

### 1. ReflexAgent
- A reflex agent that chooses an action based on a state evaluation function. It calculates the best action by evaluating all possible actions and selecting the one with the highest score.

### 2. MinimaxAgent
- Implements the Minimax algorithm for decision-making. The agent simulates the game for a specified number of depth levels and chooses the optimal move based on the minimax decision rule.

### 3. AlphaBetaAgent
- Extends the Minimax agent by adding Alpha-Beta pruning to optimize the decision-making process by eliminating branches in the search tree that do not need to be explored.

### 4. ExpectimaxAgent
- A variation of Minimax where ghosts are modeled as choosing moves uniformly at random, resulting in an "expected" score rather than a worst-case scenario.

### 5. Evaluation Function
- The evaluation function is designed to assess the quality of a game state based on various factors, including proximity to ghosts, food, and the number of remaining food pellets.

## Getting Started

### Prerequisites

To run the project, you need Python 3.x installed on your machine. You will also need the following Python libraries:
- `random`
- `sys`

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/AimeCesaireM/Project_02.git
    ```


### Running the Project

Run the autograder, which links all the other code, using the following command:
```bash
python autograder.py
```
