# Tanks-3D

Tanks 3D is a local multiplayer tank battle game developed in **Unity**, where two players compete against each other in a series of rounds by maneuvering their tanks, charging powerful shots, and strategically eliminating their opponent.

## About the game

Tanks 3D is a competitive local multiplayer arena game inspired by classic tank combat games.

Players control individual tanks, move around the battlefield, rotate their turret, charge projectile strength, and fire explosive shells at their opponent. Each successful hit damages the opposing tank, and rounds continue until one player wins the required number of rounds.

The game features automatic camera adjustments, health tracking, round management, and a complete win condition system.

## Getting Started 

1. Clone this repository.
2. Open the project using the **Unity 2022** version.
3. Open the main gameplay scene.
4. Press **Play** in the Unity Editor.

## Core Design Approach

The project follows a modular gameplay architecture where each gameplay system has a dedicated responsibility.

- **GameManager** controls the overall game flow, round progression, player spawning, and win conditions.
- **TankManager** handles the setup, enabling, disabling, and resetting of each individual player.
- **TankMovement** manages player movement, turning, and engine audio using Unity's physics system.
- **TankShooting** controls shell charging, firing mechanics, launch force calculation, and shooting effects.
- **TankHealth** manages player health, damage handling, UI health sliders, and explosion effects.
- **ShellExplosion** applies area of effect damage and explosion forces using Unity physics.
- **CameraControl** dynamically adjusts camera position and zoom to keep all active tanks visible.
- **UIDirectionControl** ensures UI elements remain correctly oriented regardless of camera movement.

## Features

- Local multiplayer tank combat
- Physics based shell firing
- Area of effect explosion damage
- Health system with dynamic UI sliders
- Adjustable shot charging mechanic
- Dynamic camera tracking and zoom
- Engine and shooting sound effects
- Multi-round gameplay with win tracking
- Automatic player spawning and reset
- Particle based explosion effects
- Round management and victory conditions

## Folder Structure 

```
Assets
│
├── Scripts
│   ├── Camera
│   │     CameraControl.cs
│   │
│   ├── Managers
│   │     GameManager.cs
│   │     TankManager.cs
│   │
│   ├── Shell
│   │     ShellExplosion.cs
│   │
│   ├── Tank
│   │     TankMovement.cs
│   │     TankHealth.cs
│   │     TankShooting.cs
│   │
│   └── UI
│         UIDirectionControl.cs
│
├── Prefabs
├── Materials
├── Scenes
├── Audio
└── UI
```

### Script Responsibilities

| Script | Responsibility |
|---------|---------------|
| GameManager | Controls game flow, rounds, spawning and win conditions |
| TankManager | Initialises, resets and manages each tank instance |
| TankMovement | Handles tank movement, turning and engine audio |
| TankShooting | Controls shell charging, firing and projectile launch |
| TankHealth | Tracks player health, damage and explosion effects |
| ShellExplosion | Applies explosion damage and physics force |
| CameraControl | Dynamically positions and zooms the camera |
| UIDirectionControl | Keeps UI correctly oriented toward the player |

## Tech Stack

- Unity
- C#
- Unity UI
- Particle Systems
- AudioSource & AudioClip
- Microsoft Visual Studio
- Git and Github for version control

## Controls

### Player 1

| Action | Control |
|---------|----------|
| Move Forward/Backward | W / S |
| Turn | A / D |
| Fire | Space |

---

### Player 2

| Action | Control |
|---------|----------|
| Move Forward/Backward | Up / Down Arrow |
| Turn | Left / Right Arrow |
| Fire | Enter |

*(Controls can be adjusted through Unity's Input Manager.)*

### Screenshots

<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/d693bf1f-bf17-46b2-a070-8e1088fe8822" />
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/b368c3e2-ef62-4505-94d0-af933acc6322" />
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/9b35a2e5-9ee9-4f03-b67e-ce192fa85363" />
<img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/51cbef0f-d08b-4245-9244-2dd15608bc71" />

## What I Learned

- Object-Oriented Programming in Unity
- Modular gameplay architecture
- Rigidbody based movement and physics
- Projectile mechanics and force calculations
- Area of effect damage systems
- Dynamic camera tracking
- Round based game management
- Player health and UI synchronization
- Audio integration
- Scene and gameplay state management

## Build 

A playable Web build is available on itch.io : https://mukul-19-singh.itch.io/tanks-3d.
