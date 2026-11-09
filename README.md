# Doom CyberPunk Style

A Python recreation of classic Doom gameplay with a cyberpunk aesthetic. Features raycasting, sprites, NPCs, weapons, and custom textures.

> **Important:** Place sound, sprites, and textures inside a single `resources` folder to avoid errors. Credits to StanislavPetrovV for the original base.

## Features
- Raycasting engine
- Player movement and controls
- NPCs and pathfinding
- Weapons and sprites
- Cyberpunk-themed textures

## Requirements
- Python 3.x
- Pygame

Install Pygame if needed:
```bash
pip install pygame
```

## How to Run
```bash
python main.py
```

## User Manual

### Setup
1. Make sure all asset folders (`sound/`, `sprites/`, `textures/`) are present.
2. Recommended: put them inside a `resources` folder if the code expects that structure.
3. Install Pygame: `pip install pygame`
4. Run the game with `python main.py`.

### Controls
The game uses standard FPS-style controls (mouse + keyboard).

| Input | Action |
|-------|--------|
| Mouse | Look around / aim |
| W / A / S / D | Move forward / left / backward / right |
| Left Mouse Button | Fire weapon |
| ESC | Quit the game |

### Gameplay Tips
- The game runs in fullscreen or windowed mode depending on the resolution set in `settings.py`.
- FPS is displayed in the window title.
- Mouse is captured while playing (press ESC to quit).
- NPCs have basic pathfinding and will react to the player.
- Weapons and sprites are loaded from the asset folders.

### Example Start
1. Open a terminal in the project folder.
2. Run `python main.py`.
3. The game window opens and music starts.
4. Use the mouse to look and WASD to move.
5. Click to shoot.
6. Press ESC to exit.

### Troubleshooting
- If assets fail to load, check that `sound/`, `sprites/`, and `textures/` folders exist in the expected location.
- Make sure Pygame is installed.
- On some systems you may need to run as administrator or adjust file permissions for asset loading.

## Project Structure
- `main.py` - Entry point and game loop
- `player.py` - Player movement and controls
- `raycasting.py` - Raycasting engine
- `npc.py` - Non-player characters
- `map.py` - Level map
- `weapon.py` - Weapon handling
- `sound/` - Sound effects and music
- `sprites/` - Sprite images
- `textures/` - Wall and floor textures

## License
Apache-2.0
