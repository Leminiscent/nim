# Nim

This Python project implements a classic game of Nim, alongside an AI that learns to play using Q-learning, a form of reinforcement learning. The game of Nim is a mathematical game of strategy in which two players take turns removing objects from distinct piles. On each turn, a player must remove at least one object, and may remove any number of objects provided they all come from the same pile. The goal is to be the player to remove the last object.

## Features

- Implementation of the Nim game logic.
- AI that learns to play Nim using Q-learning.
- Ability to train the AI by playing against itself.
- Option to play against the AI.

## How It Works

The project is divided into two main components: the `Nim` class, which handles the game logic, and the `NimAI` class, which implements the AI player using Q-learning.

### Nim Class

- Manages the state of the game, including the piles, the current player, and the winner.
- Provides methods to make moves and switch players.
- Checks for winning conditions.

### NimAI Class

- Implements Q-learning to learn from each game played.
- Stores Q-values in a dictionary mapping `(state, action)` pairs to their corresponding Q-values.
- Provides methods to choose actions based on the current state, update Q-values, and determine the best future rewards.

## Training the AI

The AI is trained through repeated self-play. Each game it plays updates its Q-values based on the outcomes of its actions, gradually improving its strategy.

## Playing Against the AI

Once trained, you can play against the AI. The game randomly decides whether the human or the AI goes first. The current state of the game is displayed on each turn, and the player is prompted to make a move.

## Setup and Execution

To run this project:

1. Ensure you have Python installed on your system.
2. Save the code in a file structure as described above (`nim.py` for the game and AI logic, `play.py` for running the game).
3. Run the `play.py` script to start training the AI and play against it once training is complete.

## Dependencies

- Python 3.x
- No external libraries are required for the game logic or the AI.

## Conclusion

This project demonstrates a simple application of Q-learning in a classic game scenario. It provides a foundation for exploring reinforcement learning techniques and game theory.

Enjoy playing Nim against your AI opponent!
