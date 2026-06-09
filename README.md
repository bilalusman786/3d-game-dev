
# Timmy's Run - 3D Endless Runner

An endless runner game developed in Unity where the player controls **Timmy**, navigating through a hazardous path, dodging obstacles, and collecting coins to achieve the highest score.

## 🚀 Features
* **Dynamic Lane Movement:** Smooth left and right movement to dodge incoming obstacles.
* **Score & Coin System:** Track collected coins and distance traveled in real-time.
* **Procedural Generation:** Endless path generation to keep the gameplay fresh and challenging.
* **Clean UI:** Main menu, HUD, and Game Over screens.

## 🛠️ Tech Stack
* **Game Engine:** Unity (3D)
* **IDE:** Visual Studio
* **Programming Language:** C#
* **Web Integration / Data (Optional):** HTML / Wolfram API (used for UI layout / data modeling)

## 🎮 Controls
| Action | Input (Keyboard) |
| --- | --- |
| **Move Left** | Left Arrow / A |
| **Move Right**| Right Arrow / D |


## 📁 Project Structure & Scripts
Here are the core C# scripts driving the game mechanics:
* `PlayerController.cs` - Handles Timmy's input, lane switching, and movement mechanics.
* `ObstacleSpawner.cs` - Manages the procedural generation and recycling of obstacles.
* `Coin.cs` - Detects collisions with Timmy, triggers audio, and updates the score manager.
* `GameManager.cs` - Controls the game states (Start, Playing, Game Over) and UI overlays.

## ⚙️ Setup & Installation
1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/yourusername/timmys-run.git](https://github.com/yourusername/timmys-run.git)
