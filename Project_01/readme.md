# Pacman Search Agents

This repository contains a collection of AI-based search agents for the classic Pacman game. The agents use various search algorithms such as Depth-First Search (DFS), Breadth-First Search (BFS), and A* search to navigate through the maze, solving different tasks like collecting food, visiting corners, and more. The project was developed as part of a university course to understand and implement basic search algorithms in artificial intelligence.

## Features

- **Search Algorithms**: Implementations of DFS, BFS, A*, and other search techniques.
- **Custom Agents**: AI agents that can be configured to perform specific tasks in the Pacman environment.
- **Problem-Solving Tasks**: Including the CornersProblem, FoodSearchProblem, and AnyFoodSearchProblem, which simulate various challenges in Pacman's environment.

## Setup and Installation

### Prerequisites

- Python 3.x
- Required libraries such as `numpy` and `game.py` (included in the project)

### Installation Steps

1. Clone the repository to your local machine:
    ```bash
    git clone https://github.com/AimeCesaireM/AI-Projects/Project_01.git
    ```

2. Navigate to the project directory:
    ```bash
    cd Project_01
    ```

3. Run the Pacman game with the desired agent. The command looks as such:
   ```bash
    python pacman.py -p <AgentName> -a <parameter1=value1,parameter2=value2,...>
    ```
   For exapmple:
    ```bash
    python pacman.py -p AStarCornersAgent -a fn=depthFirstSearch
    ```

### Available Agents

- `AStarCornersAgent`: An agent using A* search to visit all four corners of the maze.
- `AStarFoodSearchAgent`: An agent using A* search to collect all food dots.
- `ClosestDotSearchAgent`: An agent using BFS to find the closest food dot and collect it.
- `SearchAgent`: A generic agent that can be configured with different search strategies.
