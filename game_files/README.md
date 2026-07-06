# Reverse Pac-Man

A custom Pygame twist on the classic arcade game where the tables are turned! Built entirely in Python, this version changes the fundamental rules of the maze: the ghosts are the ones hungry for dots, and Pac-Man must balance speed, score, and survival. 

## Unique Gameplay Mechanics

* **Ghost Power-Ups:** The ghosts are actively eating the maze's pellets. Every regular pellet a ghost consumes permanently increases its movement speed. 
* **Power Pellet Penalty:** Beware of the big dots! When a ghost eats a Power Pellet, Pac-Man is immediately inflicted with a severe speed penalty.
* **Tactical Sprint:** Hold `Left Shift` to give Pac-Man a life-saving burst of speed (150 speed) to escape tight situations. Use it wisely—sprinting rapidly drains your hard-earned score (30 points per second)!
* **The Fruit Bomb:** Fruits aren't just for bonus points anymore. Eating a fruit acts as an emergency reset, instantly teleporting all active ghosts back to their spawn base. Leading to the completion of the level.
* **Dynamic Level Progression:** The moment all four ghosts are sent back to the spawn base simultaneously, the game automatically advances you to the next, more difficult level.

## Controls
* **Space bar:** Start/Pause the game
* **Up / Down / Left / Right Arrows:** Move Pac-Man
* **Left Shift (Hold):** Sprint (Drains score over time)

## Installation & Running

This game is built using Python and the `pygame-ce` (Community Edition) library.

1. Clone or download the repository to your local machine.
2. Ensure you have Python installed.
3. Install the required Pygame Community Edition library by running:
   ```bash
   pip install pygame-ce
Start the game by executing the main file:

    python run.py

## Project Architecture
This project utilizes an Object-Oriented Programming (OOP) structure, separating entities, game logic, and constants into modules:

run.py - Main game loop, rendering, and core event handling.

pacman.py - Player logic, input handling, and sprint mechanics.

ghosts.py - Ghost AI, dynamic speed scaling, and pellet-eating logic.

entity.py - Base class handling physics, nodes, and collision detection.

(And more)

## Credits
https://pacmancode.com
(original code)