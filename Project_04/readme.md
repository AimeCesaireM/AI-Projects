# BustersAgents: Multi-Agent Ghost Tracking for Pacman

This project implements various agents that track and display beliefs about ghost positions in the Pacman game environment. It includes the `BustersAgent`, `BustersKeyboardAgent`, and `GreedyBustersAgent`, which apply different strategies to track ghosts and determine actions based on belief distributions.

## Project Structure

- **bustersAgents.py**: Contains the main implementation for tracking ghosts and performing actions based on belief distributions.
  - `BustersAgent`: A base agent that tracks and updates beliefs about ghost positions using inference.
  - `BustersKeyboardAgent`: A keyboard-controlled version of the `BustersAgent`.
  - `GreedyBustersAgent`: A greedy agent that moves towards the closest ghost.
  
- **game.py**: Provides the game environment and interactions with the agents.
- **inference.py**: Contains the inference modules used by the agents to estimate ghost positions.
- **util.py**: Provides utility functions used throughout the project.

## Algorithms Implemented

### 1. **BustersAgent**
   - The agent tracks ghosts using inference modules, updating its belief distributions about ghost positions. It does not take actions by itself but provides the framework for other agents to act on the ghost beliefs.

### 2. **BustersKeyboardAgent**
   - A version of `BustersAgent` that is controlled via the keyboard. It displays beliefs about ghost positions and allows manual interaction with the game world.

### 3. **GreedyBustersAgent**
   - A greedy agent that charges towards the closest ghost. It computes the most likely position of each living ghost, then selects an action that brings Pacman closest to the ghost, according to maze distance.

### 4. **Inference Module**
   - **KeyboardInference**: A basic inference module that uses noisy observations of ghost positions to update beliefs. It maintains a uniform distribution over positions and updates it based on observation likelihoods.

## Getting Started

### Prerequisites

To run the project, you will need Python 3.x and the following Python libraries:
- `random`
- `sys`
- `util`
- `inference`
- `busters`

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/AimeCesaireM/Project_04.git
    ```

### Running the Project

Run the project using the following command:
```bash
python autograder.py
