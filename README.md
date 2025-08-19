# THE FORSAKEN CRYPT

**THE FORSAKEN CRYPT** is a simple 2D dungeon-style action game built in **C++** using the **raylib** library. The player controls a Samurai who battles against a Demon boss inside a crypt. The crypt is structured like a dungeon with multiple rooms connected by door portals, allowing movement between different areas. The game includes character movement, attacks, blocking, dashing, and AI-driven enemy behavior.

---

## What the Code Does

* **Samurai (Player):** Can move, jump, attack, block, dash (double‑tap A/D), and has health management with invincibility frames.
* **Demon (Enemy):** Controlled by an AI system that decides when to chase, attack, or retreat based on the player’s distance. Includes large hitboxes and sound effects.
* **Collision System:** Handles body, attack, and hurtbox collisions. Debug mode allows you to see collision boxes.
* **Dungeon Rooms:** TMX maps define multiple rooms with portals/doors that transport the player to new areas.
* **Start Screen:** Displays the game’s title and menu before entering the main crypt.
* **Audio:** Plays background music and various sound effects for combat and atmosphere.

---

## Build Instructions

1. Install **raylib** (via package manager or from source).
2. Compile the main file with:

   ```bash
   g++ -std=c++17 2dgame.cpp -o forsaken -lraylib
   ```
3. Run the executable:

   ```bash
   ./forsaken
   ```

---

## Controls

* **A / D** – Move left / right (double‑tap to dash)
* **Space** – Jump
* **Attack / Block** – Defined in the code logic
* **F1** – Toggle debug boxes
* **P** – Pause
* **M** – Toggle music
* **E** – Exit after completion

---

## Project Files

* `2dgame.cpp` – Main game loop and states
* `Samurai.h` – Player character logic
* `Demon.h` – Enemy AI logic
* `Character.h` – Abstract base for characters
* `CharacterAI.h` – AI state machine
* `CollisionSystem.h` – Collision handling
* `StartScreen.h` – Start menu screen
* `raytmx.h`, `hoxml.h` – Map loading helpers

---

## License

This project is released under an **Educational License** and is intended for learning, teaching, and non-commercial use.

---

## Credits

* Built with **raylib**
* TMX map loader: **raytmx**
* Sprite and audio assets credited to their original creators
