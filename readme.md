# Chaikin's Algorithm Step-by-Step Animation

This project implements **Chaikin's algorithm** for curve generation. The user can interactively draw control points, trigger an animation that shows the algorithm's steps, and visualize how the curve evolves over 7 steps. Once the animation completes, it will restart.

## Table of Contents

- [Overview](#overview)
- [What I Learned](#what-i-learned)
- [Functionality](#functionality)
- [Usage](#usage)
- [Bonus Features](#bonus-features)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Contributing](#contributing)

## Overview

Chaikin's algorithm is a curve generation method that smoothes a polyline by recursively adding points. In this project, the user can draw control points on a canvas, and the program will animate each step of the algorithm. The animation will run through 7 steps of Chaikin's algorithm and will restart once completed. The user can also interact with the canvas by placing new points and resetting the process.

## What I Learned

Through this project, I learned how to:

- Implement **Chaikin's algorithm** for generating smooth curves from control points.
- Handle user input for drawing points and triggering animations.
- Work with **canvas-based rendering** and **animation** in a graphical application.
- Use **event handling** for keyboard and mouse interactions.
- Implement interactive functionality such as clearing the screen and dragging control points.

## Functionality

The application allows the user to:

1. **Draw Points**: Use the left mouse button to place control points on the canvas.
2. **Start Animation**: Press the **Enter** key to start the animation, showing the progressive steps of Chaikin's algorithm. The animation will play for 7 steps and then restart.
3. **Visualize Points**: Control points are drawn as small circles on the canvas to indicate where the user has placed them.
4. **Handle Edge Cases**: 
    - If only one control point is drawn, no animation will play, and the point will remain visible.
    - If only two control points are drawn, a straight line is drawn between them, with no animation.
    - If no points are drawn, pressing Enter will do nothing.
5. **Quit Program**: Press **Escape** to quit the application.
6. **Clear Screen**: Optionally, users can clear the screen to select new control points.
7. **Drag Control Points**: Optionally, users can drag the control points in real time to change the curve dynamically.

## Usage

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/yourusername/chaikin-animation.git
   cd chaikin-animation
    cargo run
