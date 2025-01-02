# Project_03: Q-Learning and Value Iteration Agents

This repository contains implementations of Q-learning and Value Iteration algorithms, which are used to solve decision-making problems in environments such as grid worlds and Pacman. The goal is to develop intelligent agents capable of learning optimal policies through reinforcement learning techniques.

## Components

### 1. Q-Learning Agents (`qlearningAgents.py`)
This file contains the following classes:

- **QLearningAgent**: Implements a standard Q-learning agent, which learns an optimal policy using Q-values. It includes methods for:
  - Computing Q-values for state-action pairs.
  - Choosing actions based on exploration (epsilon-greedy) or exploitation (greedy).
  - Updating Q-values using the Bellman equation.
  
- **PacmanQAgent**: A specialized Q-learning agent for the Pacman environment. This subclass inherits from `QLearningAgent` and uses different default parameters for epsilon, gamma, and alpha.

- **ApproximateQAgent**: An extension of the Q-learning agent that uses a feature-based approximation for Q-values. This agent applies linear regression to learn optimal policies, with weights assigned to features of the state-action pairs.

### 2. Value Iteration Agents (`valueIterationAgents.py`)
This file implements a value iteration agent for solving Markov Decision Processes (MDPs):

- **ValueIterationAgent**: Performs value iteration to find the optimal policy. It uses the Bellman equation to compute state values and Q-values iteratively. The agent also computes the best action for each state based on the values.

## Getting Started

### Prerequisites

To run the code, ensure you have the following dependencies installed:

- Python 3.x
- `numpy`, `pygame`, and other necessary libraries (if using Pacman environment)

### Running the Agents

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Project_03.git
   cd Project_03
2. Run the autograder:
   ```bash
   python autograder.py
   ```
