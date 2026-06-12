# Pac-Man Game

A 2D Pac-Man game built with Unity Engine and C# -- featuring player-controlled movement, AI ghost pathfinding, and classic arcade gameplay mechanics.

![Unity](https://img.shields.io/badge/Unity-000000?style=flat&logo=unity&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=flat&logo=csharp&logoColor=white)

> Project Assignment 3 -- Computer Game Development and Animation, [NIT Warangal](https://nitw.ac.in/) (Winter 2021)

## Overview

A faithful recreation of the classic Pac-Man arcade game built in Unity Engine. The player navigates Pac-Man through an enclosed maze, eating dots while avoiding four colored ghosts. The game implements smooth movement with raycasting-based collision detection, ghost AI with predefined patrol patterns, and score tracking.

<img src="images/Gameplay.png" alt="Gameplay" width="100%">

## Gameplay

- **Objective**: Eat all dots placed in the maze
- **Controls**: Arrow keys for directional movement
- **Win Condition**: Collect every dot in the maze
- **Lose Condition**: Contact with any ghost

### Ghost Characters

| Ghost | Color | Behavior |
|-------|-------|----------|
| Blinky | Red | Aggressive chaser |
| Pinky | Pink | Ambush positioning |
| Inky | Cyan | Unpredictable movement |
| Clyde | Orange | Random patrol pattern |

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Game Engine | Unity Engine |
| Language | C# (MonoBehaviour) |
| Editor | Visual Studio Code |
| Physics | Unity 2D Raycasting |

## Project Structure

```
PacMan-Game__UnityEngine/
├── Scripts/
│   ├── PacmanMove.cs       # Player movement, input handling, collision
│   ├── GhostMove.cs        # Ghost AI patrol patterns and speed
│   └── Pacdot.cs           # Dot positions, collection, and score
├── images/
│   └── Gameplay.png        # Gameplay screenshot
└── README.md
```

## Script Details

### PacmanMove.cs
- Smooth grid-based movement using `Vector2.MoveTowards()`
- Keyboard input handling (arrow keys)
- Raycasting for wall collision detection
- Animation parameter updates for directional sprites
- Movement validation before each step

### GhostMove.cs
- Predefined waypoint-based movement paths for each ghost
- Individual movement speeds per ghost
- Continuous patrol behavior with path cycling

### Pacdot.cs
- Dot position management on the grid
- Collision-triggered destruction on Pac-Man contact
- Score increment on collection

## Availability

The playable Windows build (`Pac-Man Build.zip`, run via `Pac-man 2D.exe`) was previously distributed through a Google Drive folder that is no longer available. This repository contains the game's C# scripts and a gameplay screenshot only -- the full Unity project (scenes, assets, `ProjectSettings/`) is not included, so the game cannot currently be downloaded or built from this repo.

## License

MIT
