# 🏃 Timmy's Run

A fast-paced, high-performance 3D endless runner built in Unity. Dodge obstacles, collect coins, and push your reflexes to the limit in an ever-accelerating procedurally generated gauntlet.

   _____ _                                    _       _____             
  |_   _(_)                                  's      |  __ \            
    | |  _ _ __ ___  _ __ ___  _   _ ___      _ __   | |__) |   _ _ __  
    | | | | '_ ` _ \| '_ ` _ \| | | / __|    | '_ \  |  _  / | | | '_ \ 
    | | | | | | | | | | | | | | |_| \__ \    | | | | | | \ \ |_| | | | |
    |_| |_|_| |_| |_|_| |_| |_|\__, |___/    |_| |_| |_|  \_\__,_|_| |_|
                                __/ |                                   
                               |___/                                    

<div align="center">

[![Engine - Unity 3D](https://img.shields.io/badge/Engine-Unity%203D-000000?style=for-the-badge&logo=unity&logoColor=white)](https://unity.com/)
[![Language - C#](https://img.shields.io/badge/Language-C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)](https://learn.microsoft.com/en-us/dotnet/csharp/)
[![IDE - Visual Studio](https://img.shields.io/badge/IDE-Visual%20Studio-5C2D91?style=for-the-badge&logo=visualstudio&logoColor=white)](https://visualstudio.microsoft.com/)
[![License - MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)

**Dodge. Collect. Survive. How far can Timmy go?**

[Explore Documentation](docs/) · [Report Bug](https://github.com/yourusername/timmys-run/issues) · [Request Feature](https://github.com/yourusername/timmys-run/issues)

</div>

---

## 📖 Overview

**Timmy's Run** is an immersive, high-octane 3D endless runner designed to test player reflexes through a dynamically generated world. Players guide Timmy across three structural lanes, executing split-second maneuvers to bypass hazardous obstacles and capture valuable coins. As distance increases, so does the speed—demanding perfect precision. The path never ends, but one single wrong move spells game over.

### Key Gameplay Loop
1. **Navigate:** Swap seamlessly between 3 distinct lanes (Left, Center, Right) using snappy controls.
2. **Collect:** Gather coins structurally positioned along procedural paths to maximize high scores.
3. **Survive:** Dodge dynamically spawning hazards. Game speed scales asymptotically over time to naturally escalate difficulty.

---

## ✨ Features

| Feature | Category | Description | Technical Implementation |
| :--- | :--- | :--- | :--- |
| 🔀 **Dynamic Lane Movement** | Mechanics | Fluid left/right shifting with snappy, predictable handling. | Framerate-independent `Mathf.MoveTowards` / `Vector3.Lerp` interpolation. |
| 🪙 **Coin & Score System** | Systems | Real-time score calculation combining collected coins and distance traveled. | Decoupled event-driven architecture using C# actions. |
| ♾️ **Procedural Generation** | Architecture | Infinite, random road sections spawned ahead of the player while recycling passed segments. | Dedicated Object Pooler to prevent runtime garbage collection spikes. |
| 🎨 **Clean UI/UX Layout** | Interface | Minimalistic HUD, highly functional main menu, and contextual Game Over dashboard. | Designed with Unity UI (uGUI), anchored dynamically for multi-resolution scaling. |

---

## 🛠️ Tech Stack & Architecture

* **Core Engine:** Unity 2021.3 LTS (Long Term Support)
* **Scripting Language:** C# (Object-Oriented, Type-Safe Architecture)
* **IDE Development:** Visual Studio / VS Code (Roslyn Analyzers enforced)
* **UI Prototyping & Layout Modeling:** HTML / Wolfram API data formatting schemas

### Game Lifecycle Architecture Block Diagram
[Main Menu Scene] ──(User Interaction)──> [Load Game Scene]
│
▼
┌─────────────────┐
│  Initialize:    │
│  - GameManager  │
│  - Object Pools │
└────────┬────────┘
│
▼
┌─────────────────┐ <───┐
│   Core Loop     │     │
│ - Read Input    │     │
│ - Move Player   │     │
│ - Check Collide │     │
└────────┬────────┘     │
│              │ (Per Frame)
(Is Collision?)        │
├── No ──────────────┘
└── Yes ──> [Trigger Game Over UI]


---

## 📁 Project Structure

Below is a breakdown of the production-ready directory structure for the core codebase:
