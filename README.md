# 🛣️ Highway Simulation Engine

## Overview
The Highway Simulation Engine is a lightweight, 2D top-down vehicular avoidance game built entirely with HTML5 Canvas and Vanilla JavaScript. Designed with a strict distributed architecture, it demonstrates core game loop mechanics, dynamic entity rendering, algorithmic difficulty scaling, and state machine management without the overhead of heavy third-party game engines.

## 🎮 How to Play
Navigate your vehicle through high-speed traffic, intercepting target assets (gifts) while avoiding critical collisions with road barriers. 

### Controls
*   **Steer Left:** `Left Arrow` or `A`
*   **Steer Right:** `Right Arrow` or `D`

### Operating Modes
The simulation is divided into two distinct protocols:

1.  **Levels Mode:** A finite progression system. Collect the required number of target items to advance through stages. Each stage features increased velocity and hazard density.
2.  **Unlimited (Endless) Mode:** A continuous survival loop. Driven by a dynamic scaling algorithm, the environment's velocity and barrier spawn rates increment over time based on delta time (`dt`). Survive as long as possible to achieve a maximum high score.

## 🏗️ System Architecture
The application utilizes a distributed, multi-file architecture to enforce a separation of concerns and eliminate DOM rendering conflicts:
*   `index.html`: The core dashboard and routing interface.
*   `levels.html`: Manages finite state progression, level arrays, and visual telemetry (dot-based UI).
*   `unlimited.html`: Manages the dynamic difficulty scaling algorithm and continuous numerical scoring.

## 🚀 Installation & Execution
Because the simulation relies entirely on client-side web technologies, no build pipeline, package manager, or local server is strictly required for basic execution.

Clone the repository to your local machine:
   ```bash
   git clone [https://github.com/YourUsername/highway-simulation-engine.git](https://github.com/YourUsername/highway-simulation-engine.git)

1. Navigate to the local project directory.

2. Ensure the asset files (car.png, barrier.png, gift.png) are located in the root folder alongside the HTML files.

3. Open index.html directly in any modern web browser to launch the dashboard.

👨‍💻 Author
Gabriel
