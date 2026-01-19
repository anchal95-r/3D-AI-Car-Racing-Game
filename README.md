# 3D Car Racing Game with Realistic Vehicle Dynamics and AI Pathfinding

A Unity-based 3D racing simulation that combines realistic vehicle physics, rule-based AI pathfinding, and custom 3D assets created in Blender. This project demonstrates how physics simulation, artificial intelligence, and game design can work together to create an immersive and educational racing experience.

---

## 📌 Project Overview

This project is a **3D Car Racing Game** developed using **Unity** and **Blender**, featuring:

* Realistic car physics using Unity’s **Wheel Collider system**
* AI-driven opponent vehicles with **rule-based path-following intelligence**
* Custom-designed 3D assets (cars, tracks, and environment)
* A complete game flow with menus, lap systems, and race logic

Players compete against AI-controlled cars on a visually rich track while experiencing natural driving behavior such as traction, braking, steering, and downforce.

---

## 🎮 Features

### 🚗 Realistic Vehicle Dynamics

* Physics-based movement using **WheelColliders**
* Torque, traction control, and braking simulation
* Downforce for high-speed stability
* Gear and engine rev simulation

### 🤖 AI Pathfinding & Behavior

* Rule-based (Deterministic) AI system
* Waypoint-based path following
* Adaptive braking on sharp turns
* Speed control on straights and corners
* Collision avoidance using trigger detection

### 🏗️ Custom 3D Assets

* Car models and race tracks designed in **Blender**
* FBX-based asset import into Unity
* Optimized meshes and textures
* Environmental objects (barriers, trees, lighting poles, etc.)

### 🖥️ Game Flow

* Main menu and race setup screen
* Track and lap selection
* Checkpoints and lap counting
* Race completion logic
* Background music and sound effects

---

## 🛠️ Technologies Used

| Tool / Tech              | Purpose                                             |
| ------------------------ | --------------------------------------------------- |
| **Unity Engine**         | Game development, physics, rendering, and scripting |
| **Blender**              | 3D modeling and asset creation                      |
| **C#**                   | Game logic and AI scripting                         |
| **WheelCollider System** | Vehicle physics simulation                          |

---

## 📂 Project Structure

```
Assets/
├── Models/          # 3D car, track, and environment models
├── Materials/      # Textures and shaders
├── Scripts/
│   ├── CarController.cs   # Player car physics and control
│   └── CarAIControl.cs   # AI vehicle behavior and pathfinding
├── Scenes/         # Main menu and race scenes
└── Prefabs/        # Reusable game objects
```

---

## 🧠 AI System Explanation

This project uses **Rule-Based (Symbolic) AI**, not machine learning. The AI behavior is driven by predefined mathematical rules:

### Core Logic

* Follows **waypoints** placed along the track
* Calculates steering angle based on target position
* Adjusts speed near corners using a cautious braking factor
* Detects barriers and cars to avoid repeated collisions

### AI Capabilities

* Lane following
* Speed modulation
* Adaptive turning
* Collision handling

This approach ensures predictable, fair, and competitive AI opponents.

---

## 🚙 Physics & Key Formulas

### Speed Conversion

Unity uses meters per second (m/s). The game converts this to:

```
Speed (KPH) = Velocity (m/s) × 3.6
Speed (MPH) = Velocity (m/s) × 2.2369
```

### Steering

```
θ = Steering Input × Max Steering Angle
```

### Downforce

```
Fd = Cd × Velocity
```

### Torque Distribution

```
T = Engine Torque / Number of Driven Wheels
```

These formulas ensure realistic traction, handling, and stability.

---

## 📜 Core Scripts

### `CarController.cs`

Handles all player vehicle physics:

* Acceleration & braking
* Steering
* Traction control
* Gear shifting
* Downforce application

### `CarAIControl.cs`

Controls AI vehicles:

* Waypoint navigation
* Steering angle calculation
* Speed control near turns
* Collision avoidance

Both scripts use Unity’s physics engine to ensure consistent behavior between player and AI cars.

---

## ▶️ How to Run the Project

### Step 1: Install Unity

* Download **Unity Hub** from [https://unity.com/](https://unity.com/)
* Install the **LTS version** of Unity

### Step 2: Open Project

* Launch Unity Hub
* Click **Open Project**
* Select this repository folder

### Step 3: Play

* Open the main scene from `Assets/Scenes`
* Click the **Play** button in Unity

---

## 🎯 Learning Outcomes

This project demonstrates:

* Physics-based vehicle simulation
* AI pathfinding and decision logic
* Game system architecture
* 3D asset pipeline (Blender → Unity)
* Scene management and UI integration

It can also serve as a foundation for:

* Autonomous vehicle simulation
* Reinforcement learning environments
* Traffic or driver behavior research

---

## 🚀 Future Improvements

* Multiplayer mode
* Machine learning-based AI drivers
* Dynamic weather system
* More tracks and vehicles
* Enhanced graphics using URP/HDRP

---

## 👩‍💻 Author

**Anchal Kumari**
B.Tech Computer Science & Engineering

---

## 📄 License

This project is intended for **educational and academic use**. You are free to modify and extend it for learning purposes.

---

⭐ If you find this project helpful, consider starring the repository!
