# Ultimate Quiz Battle

Ultimate Quiz Battle is a command-line Python application that simulates a multi-question quiz. The game allows users to answer general knowledge questions with a focus on clean user experience, robust input handling, and minimalist design. It is built entirely using core Python without any external libraries or dependencies.

---

## Overview

The project demonstrates core concepts in Python such as:

- Control flow using `if-else` statements and loops
- User input handling using `input()` and string processing
- Type conversion and validation
- Function abstraction and modular design
- State management across game rounds

---

## Core Functionality

The game presents a sequence of multiple-choice questions. Each question is stored as a dictionary containing:

- `text`: The question string
- `options`: A list of possible answers
- `correct`: The index of the correct option (1-based)

Players can answer each question either by selecting the option number or by typing the full text of the answer (case-insensitive). A special “Quit” option is always included at the end of the list, allowing the user to exit the game voluntarily and keep the winnings earned so far.

Each question allows up to two attempts. On the first incorrect input, the player is notified and prompted to try again. On the second failure, the game ends, and the player’s total winnings are displayed.

Correct answers increment the player's score. The game continues until the player either quits or answers all questions.

---

## Design Goals

- **Reliability**: The game handles invalid inputs gracefully, including non-numeric input and out-of-range selections.
- **Flexibility**: Users may answer with either option numbers or actual answer strings.
- **Simplicity**: No imports or third-party packages are used, keeping the code fully portable and dependency-free.
- **Reusability**: The code is organized into functions for readability, reusability, and extensibility.

---

## Execution

To run the game, save the script to a `.py` file and execute it using Python 3 from the command line:

