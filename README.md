# Mini Space Shooter Game Microcontroller

## Project Overview
The Mini Space Shooter Game Microcontroller is a retro-style space shooter game designed for audiences of most ages, regardless of gaming experience. The game is displayed on an OLED screen connected to an Arduino Nano, where players can control a spaceship, shoot enemies, and level up. The game features a start screen, an in-game screen, and a game-over screen.

This project was **heavily** inspired by [Volos Projects](https://www.youtube.com/@VolosProjects) 

## Table of Contents
- Project Components
- How it Works
- Wiring and Setup
- Code Structure
- Challenges Faced
- Results
- References

## Project Components
- Arduino Nano
- 128x64 I2C OLED Display (SSD1306)
- Push Buttons (x3)
- Buzzer
- Breadboard & Jumper Wires

## How it Works
The player controls a spaceship using buttons connected to the Arduino Nano. The OLED screen displays the game interface, and a buzzer plays sound effects for actions like shooting or losing a life. Players can shoot enemy ships, earn points, and level up as they progress. Once all lives are lost, a game-over screen is displayed.

## Features:
- Start screen, game screen, and game-over screen
- Player movement using buttons
- Bullet firing and collision detection
- Scoring, lives, and level progression
- Sound effects using a buzzer
## Wiring and Setup
Connect the components to the Arduino Nano as follows:

- OLED Display: I2C (GND, VCC, SCL, SDA)
- Buttons: Digital pins D3, D12, and D13 (for firing, moving up, and moving down)
- Buzzer: Pin D9

## Code Structure
The code is organized into functions for:

- Game setup (setup())
- Game loop (loop())
- Player controls (updatePlayer())
- Enemy behavior (updateEnemy())
- Display and sound management
- Collision detection

The game uses structured timing via the millis() function for non-blocking delays, ensuring smooth gameplay. Bitmap graphics are used for the player and enemies to maximize the OLED display's potential.

## Challenges Faced
- Display Size: The small size of the OLED screen made it difficult to fit all game elements.
- Wiring Complexity: Organizing the wiring on the breadboard was tricky due to the number of components.
- Sound Quality: Tuning the buzzer to produce clear sound effects was challenging, as adjusting frequencies led to distorted sounds initially.

## Results
The project was successfully tested using Wokwi, an online electronics simulator, and the game runs smoothly, offering a fun, retro-style experience. Users can easily control the ship, score points, and advance through levels.

## References
- Ismailov A. S. & Jo‘Rayev Z. B. (2022): Study of Arduino Microcontroller Board.
- [Arduino Nano Documentation](https://www.mantech.co.za/datasheets/products/a000005-6s.pdf)
- [OLED Display Module](https://sensorkit.arduino.cc/sensorkit/module/lessons/lesson/10-the-oled-screen)
- [Arduino Star Wars Game - how to make](https://www.youtube.com/watch?v=lOz_GuME63E)

## Contributors
- [Abdulmohiamin Giamal Bashir](https://github.com/ValhallaAMB)
- Muhammad Bilal
- Abdulrahman Mekkaoui
- Shirina Maci
