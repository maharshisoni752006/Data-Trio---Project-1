# The Snake Game

**Team Members:** 
 - Mrunali Parmar - 202401122
 - Manya Rana - 202401115
 - Maharshi Soni - 202401108

# Abstract
This is a simple console-based Snake game implemented in C++. The player controls a snake that moves around the grid while eating food to grow in size while avoiding collisions with the walls and itself. The game continues until the snake collides with a wall or itself, at which point the player can restart or exit. The code is OS-dependant.

# How It Works
1. The game uses a `Snake` class to manage the snake's movement, growth, and collision detection.
2. A `Game` class handles food generation, score tracking, rendering the game board, and processing user input.
3. The snake moves in one of four directions (UP, DOWN, LEFT, RIGHT), controlled by the player using the `W`, `A`, `S`, `D` keys.
4. If the snake eats food, it grows, and a new piece of food appears at a random location on the grid.
5. If the snake collides with itself or the boundaries of the grid, the game ends.
6. The player is given the option to restart the game or exit upon losing.

# Some of the Technologies Used
- C++ Standard Library -> `iostream`, `vector`, `deque`, `ctime`, etc.
- Console-based graphics -> ASCII rendering of the grid
- Windows system calls(OS-dependant) -> `system("cls")` for clearing the screen, `_kbhit()` and `_getch()` for keyboard input, `Sleep()` for controlling game speed

# How to Run
1. **Compile the Code**:
   - Use a C++ compiler like `g++` (for MinGW on Windows) or `clang++`.
   - Example compilation command:
     ```sh
     g++ -o snake_game main.cpp -std=c++11
     ```

2. **Run the Code**:
   ```sh
   ./snake_game
   ```

# Controls
- `W` - Move Up
- `S` - Move Down
- `A` - Move Left
- `D` - Move Right
- `R` - Restart the game (after Game Over)
- Any other key - Exit the game (after Game Over)
