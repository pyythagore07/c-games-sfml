# 🗡️ 2D RPG Game — C++ / SFML

A 2D top-down RPG game built from scratch in **C++** using the **SFML** library and **Visual Studio**. This project was developed by following [Mustafa Sibai's](https://www.youtube.com/@MustafaSibai) 30-part YouTube tutorial series *"Game Development in C++ with SFML"* — then extended and adapted as a personal learning project.

<!-- Replace with an actual screenshot of your game -->
<!-- ![gameplay](screenshots/gameplay.png) -->

---

## Features

- **Player movement** — WASD directional controls with frame-rate independent movement (deltaTime)
- **Projectile system** — shoot bullets with directional aiming
- **Collision detection** — AABB (Axis-Aligned Bounding Box) collision handling
- **Tilemap rendering** — tile-based world built from a tilesheet using arrays and lookup tables
- **FPS counter** — real-time framerate display with SFML text rendering
- **Heap & stack memory management** — proper use of pointers and dynamic allocation
- **Object-oriented architecture** — game structured around C++ classes, encapsulation, and separation of concerns

---

## Tech Stack

| Component       | Technology                |
|-----------------|---------------------------|
| Language        | C++                       |
| Graphics        | SFML 2.x                  |
| IDE             | Visual Studio 2019 / 2022 |
| Version Control | Git                       |
| Platform        | Windows                   |

---

## Prerequisites

- **Visual Studio 2019** or later (with C++ Desktop Development workload)
- **SFML 2.5+** — included in the `dependencies/` folder, or [download here](https://www.sfml-dev.org/download.php)

---

## Build & Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/rpg-game.git
   cd rpg-game
   ```

2. **Open the solution** — double-click `RPG-Game.sln` in Visual Studio.

3. **Verify SFML linkage** — the project should already reference the SFML headers and libraries under `dependencies/SFML/`. If not, point the include/library directories to your local SFML install:
   - **Include:** `dependencies/SFML/include`
   - **Lib:** `dependencies/SFML/lib`

4. **Build** — select `Debug` or `Release` (x86 or x64 depending on your SFML build) and hit `Ctrl+F5`.

5. **Run** — make sure the required SFML `.dll` files are next to the executable (or in your system PATH).

---

## Project Structure

```
rpg-game/
├── RPG-Game.sln                  # Visual Studio solution
├── RPG-Game/
│   ├── main.cpp                  # Entry point — game loop
│   ├── Game.h / Game.cpp         # Core game class (window, update, render)
│   ├── Player.h / Player.cpp     # Player entity (movement, shooting)
│   ├── Bullet.h / Bullet.cpp     # Projectile logic
│   ├── Map.h / Map.cpp           # Tilemap loading & rendering
│   ├── Collision.h               # AABB collision utilities
│   ├── assets/                   # Textures, tilesheets, fonts
│   └── ...
├── dependencies/
│   └── SFML/                     # SFML headers & prebuilt libs
├── .gitignore
└── README.md
```

> **Note:** The actual file names in your repo may differ slightly. Update this section to match your project's real structure.

---

## What I Learned

This project was primarily a learning exercise. Key concepts practiced:

- Setting up a C++ project with external libraries (static & dynamic linking)
- The SFML rendering pipeline: window → event loop → draw calls
- Game loop architecture with `deltaTime` for frame-rate independence
- Tile-based map design using 2D arrays and sprite tiling
- Memory management: stack vs heap, pointers, constructors & destructors
- AABB collision detection for game entity interactions
- Structuring a growing codebase with header/source separation

---

## Credits

- **Tutorial series:** [Game Development in C++ with SFML](https://www.youtube.com/playlist?list=PL1xNqYU3-dWRvjpMcp7pXa4eMgME5TAd_) by **Mustafa Sibai** (30 parts, ~365k views)
- **SFML:** [sfml-dev.org](https://www.sfml-dev.org/)

---

## License

This project is for **educational purposes**. The original tutorial code belongs to [Mustafa Sibai](https://github.com/mustafa-sibai). My implementation follows the tutorial structure with personal modifications.

<!-- If you want to add a license, uncomment one of these: -->
<!-- This project is licensed under the MIT License — see [LICENSE](LICENSE) for details. -->
