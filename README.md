# C++: Grid-Based Maze System
**University Year 1 | Game Programming Fundamentals**

A technical exploration of 2D grid logic and file persistence in C++, built using a custom framework over the SFML library.

## 🕹️ Project Overview
This project focuses on the core engineering principles of grid-based games. It features a fully functional maze traversal system where the environment is defined by a 2D array, allowing for complex level layouts, enemy AI, and persistent save/load functionality.

> **[🔗 View the full technical breakdown on my Portfolio](https://sites.google.com/view/myles-coleman/projects/game-programming-fundamentals)**

## 🛠️ Key Technical Features

### Data-Driven Level Design
* **2D Array Mapping:** The game world is managed via a 2D `char` array. This allows for efficient tile-based rendering and collision checks by map coordinates.
* **File I/O Persistence:** Implemented a robust saving and loading system using `std::ifstream` and `std::ofstream`. Levels are stored as `.txt` files, allowing players to save their progress or load custom-designed maze layouts.
* **Dynamic Level Progression:** The system handles transitions between stages by automatically updating file strings (e.g., "mapFile-1", "mapFile-2") upon reaching the goal ('G').

### Gameplay Engineering
* **Collision Validation:** Developed a `canMoveThere` system that validates coordinates against the 2D array before updating the player's position, preventing movement through "Wall" ('W') tiles.
* **Enemy AI Behaviour:** Engineered a basic AI that selects random cardinal directions and validates movement against the map grid to navigate the maze autonomously.
* **Game Loop & Input Handling:** Utilises a standard game loop with a framework wrapper for SFML, handling real-time event polling and keyboard input for movement and system commands.

## 💻 Technical Specs
* **Language:** C++
* **Library:** SFML (Simple and Fast Multimedia Library)
* **Compiler:** Visual Studio (MSVC)
* **Data Format:** Plain-text (.txt) level data
