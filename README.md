# Reverse Pac Man

A custom Pygame twist on the classic arcade game where the tables are turned! Built entirely in Python, this version changes the fundamental rules of the maze: the ghosts are the ones hungry for dots, and Pac-Man must balance speed, score, and survival. 

## The twists

* **Ghost Power-Ups:** The ghosts are actively eating the maze's pellets. Every regular pellet a ghost consumes permanently increases its movement speed. 


* **Power Pellet Penalty:** Beware of the big dots! When a ghost eats a Power Pellet, Pac Man is immediately inflicted with a severe speed loss.


* **Tactical Sprint:** Hold the `Left Shift` key to give PacMan a burst of speed to escape tight situations or to capture ghosts. However, you can **only sprint if you have a score greater than 0**, and sprinting rapidly drains your score (30 points per second)! Use it wisely.


* **Level Progression & The Fruit Shortcut:** There are two ways to complete a level:
  1. **The Hard Way:** Force all four ghosts into their spawn base at the exact same time. 
  
  2. **The Easy Way (The Fruit Shortcut):** Eating a fruit instantly sends all ghosts to spawn, immediately advancing you to the next level. However, taking this shortcut comes at a heavy price: **it will cost you one life!**

## Controls
* **Space bar:** Start/Pause the game
* **Up / Down / Left / Right Arrows:** Move Pac Man
* **Left Shift (Hold):** Sprint (Requires more than 0 points; drains score)

## Installation & Running

This game is built using Python and the `pygame-ce` (Pygame Community Edition) library.

1. Clone or download the repository to your local machine.
2. Ensure you have Python installed.
3. Install the required Pygame Community Edition library by running:
   ```bash
   pip install pygame-ce
4. Start the game by executing the main file:
   ```bash
   python main.py
## Project Architecture
This project utilizes an Object Oriented Programming (OOP) structure. This means entities, game logic, constants, and other things are separated into modules:

main.py - Main game loop, rendering, and core event handling.

pacman.py - Player logic, input handling, and sprint mechanics.

ghosts.py - Ghost AI, dynamic speed scaling, and pellet eating logic.

entity.py - Base class handling physics, nodes, and collision detection.

###### (And more)

## Credits
https://pacmancode.com
(original code)