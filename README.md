<div align="center">
🏃 Timmy's Run
A fast-paced 3D endless runner built in Unity
![Unity](https://img.shields.io/badge/Engine-Unity%203D-000000?style=flat&logo=unity)
![Language](https://img.shields.io/badge/Language-C%23-239120?style=flat&logo=csharp)
![IDE](https://img.shields.io/badge/IDE-Visual%20Studio-5C2D91?style=flat&logo=visualstudio)
![License](https://img.shields.io/badge/License-MIT-blue.svg)
Dodge. Collect. Survive. How far can Timmy go?
</div>
---
📖 Overview
Timmy's Run is a 3D endless runner where you guide Timmy through a procedurally generated gauntlet of obstacles. Switch lanes at lightning speed, collect coins, and push your distance record as far as possible — the path never ends, but one wrong move does.
---
✨ Features
Feature	Description
🔀 Dynamic Lane Movement	Fluid left/right lane switching with smooth interpolation
🪙 Coin & Score System	Real-time tracking of coins collected and distance traveled
♾️ Procedural Generation	Endlessly varied obstacle and path layouts
🎨 Clean UI	Polished Main Menu, in-game HUD, and Game Over screens
---
🛠️ Tech Stack
Game Engine: Unity (3D)
Language: C#
IDE: Visual Studio
Optional / Web: HTML · Wolfram API (UI layout & data modeling)
---
🎮 Controls
Action	Keyboard
Move Left	`←` Arrow  /  `A`
Move Right	`→` Arrow  /  `D`
---
📁 Project Structure
```
TimmysRun/
├── Assets/
│   ├── Scripts/
│   │   ├── PlayerController.cs     # Input, lane switching & movement
│   │   ├── ObstacleSpawner.cs      # Procedural generation & recycling
│   │   ├── Coin.cs                 # Collision detection & score updates
│   │   └── GameManager.cs          # Game states & UI management
│   ├── Scenes/
│   │   ├── MainMenu.unity
│   │   └── Game.unity
│   ├── Prefabs/
│   └── Materials/
├── Packages/
├── ProjectSettings/
└── README.md
```
Core Scripts
`PlayerController.cs`
Handles all player input, lane-switching logic, and Timmy's movement along the path.
`ObstacleSpawner.cs`
Manages procedural spawning and object-pooling/recycling of obstacles to keep performance smooth and gameplay unpredictable.
`Coin.cs`
Detects trigger collisions with Timmy, fires the pickup sound effect, and notifies the `GameManager` to update the coin count.
`GameManager.cs`
Central state machine controlling transitions between Start, Playing, and Game Over states, and driving all UI overlays accordingly.
---
⚙️ Getting Started
Prerequisites
Unity Hub with Unity 2021.3 LTS or later
Visual Studio (or VS Code with the C# extension)
Installation
Clone the repository
```bash
   git clone https://github.com/yourusername/timmys-run.git
   cd timmys-run
   ```
Open in Unity
Launch Unity Hub
Click Open → Add project from disk
Select the cloned `timmys-run/` folder
Load the Main Scene
In the Project panel, navigate to `Assets/Scenes/`
Open `MainMenu.unity` to start from the menu, or `Game.unity` to jump straight in
Play
Press the ▶ Play button in the Unity Editor toolbar
---
🗺️ Roadmap
[ ] Mobile touch controls (swipe left / swipe right)
[ ] Power-ups (shield, speed boost, coin magnet)
[ ] Multiple character skins
[ ] Global leaderboard integration
[ ] Sound & music settings panel
---
🤝 Contributing
Contributions are welcome! To get started:
Fork the repository
Create a feature branch: `git checkout -b feature/your-feature-name`
Commit your changes: `git commit -m "Add: your feature description"`
Push to the branch: `git push origin feature/your-feature-name`
Open a Pull Request
Please follow the existing code style and add comments where the logic is non-obvious.
---
📄 License
This project is licensed under the MIT License.
---
<div align="center">
Made with ❤️ and a lot of `Debug.Log()` calls.
</div><div align="center">
🏃 Timmy's Run
A fast-paced 3D endless runner built in Unity
![Unity](https://img.shields.io/badge/Engine-Unity%203D-000000?style=flat&logo=unity)
![Language](https://img.shields.io/badge/Language-C%23-239120?style=flat&logo=csharp)
![IDE](https://img.shields.io/badge/IDE-Visual%20Studio-5C2D91?style=flat&logo=visualstudio)
![License](https://img.shields.io/badge/License-MIT-blue.svg)
Dodge. Collect. Survive. How far can Timmy go?
</div>
---
📖 Overview
Timmy's Run is a 3D endless runner where you guide Timmy through a procedurally generated gauntlet of obstacles. Switch lanes at lightning speed, collect coins, and push your distance record as far as possible — the path never ends, but one wrong move does.
---
✨ Features
Feature	Description
🔀 Dynamic Lane Movement	Fluid left/right lane switching with smooth interpolation
🪙 Coin & Score System	Real-time tracking of coins collected and distance traveled
♾️ Procedural Generation	Endlessly varied obstacle and path layouts
🎨 Clean UI	Polished Main Menu, in-game HUD, and Game Over screens
---
🛠️ Tech Stack
Game Engine: Unity (3D)
Language: C#
IDE: Visual Studio
Optional / Web: HTML · Wolfram API (UI layout & data modeling)
---
🎮 Controls
Action	Keyboard
Move Left	`←` Arrow  /  `A`
Move Right	`→` Arrow  /  `D`
---
📁 Project Structure
```
TimmysRun/
├── Assets/
│   ├── Scripts/
│   │   ├── PlayerController.cs     # Input, lane switching & movement
│   │   ├── ObstacleSpawner.cs      # Procedural generation & recycling
│   │   ├── Coin.cs                 # Collision detection & score updates
│   │   └── GameManager.cs          # Game states & UI management
│   ├── Scenes/
│   │   ├── MainMenu.unity
│   │   └── Game.unity
│   ├── Prefabs/
│   └── Materials/
├── Packages/
├── ProjectSettings/
└── README.md
```
Core Scripts
`PlayerController.cs`
Handles all player input, lane-switching logic, and Timmy's movement along the path.
`ObstacleSpawner.cs`
Manages procedural spawning and object-pooling/recycling of obstacles to keep performance smooth and gameplay unpredictable.
`Coin.cs`
Detects trigger collisions with Timmy, fires the pickup sound effect, and notifies the `GameManager` to update the coin count.
`GameManager.cs`
Central state machine controlling transitions between Start, Playing, and Game Over states, and driving all UI overlays accordingly.
---
⚙️ Getting Started
Prerequisites
Unity Hub with Unity 2021.3 LTS or later
Visual Studio (or VS Code with the C# extension)
Installation
Clone the repository
```bash
   git clone https://github.com/yourusername/timmys-run.git
   cd timmys-run
   ```
Open in Unity
Launch Unity Hub
Click Open → Add project from disk
Select the cloned `timmys-run/` folder
Load the Main Scene
In the Project panel, navigate to `Assets/Scenes/`
Open `MainMenu.unity` to start from the menu, or `Game.unity` to jump straight in
Play
Press the ▶ Play button in the Unity Editor toolbar
---
🗺️ Roadmap
[ ] Mobile touch controls (swipe left / swipe right)
[ ] Power-ups (shield, speed boost, coin magnet)
[ ] Multiple character skins
[ ] Global leaderboard integration
[ ] Sound & music settings panel
---
🤝 Contributing
Contributions are welcome! To get started:
Fork the repository
Create a feature branch: `git checkout -b feature/your-feature-name`
Commit your changes: `git commit -m "Add: your feature description"`
Push to the branch: `git push origin feature/your-feature-name`
Open a Pull Request
Please follow the existing code style and add comments where the logic is non-obvious.
---
📄 License
This project is licensed under the MIT License.
---
<div align="center">
Made with ❤️ and a lot of `Debug.Log()` calls.
</div>
