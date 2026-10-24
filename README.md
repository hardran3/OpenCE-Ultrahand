# Halo Settings & Cheats for Ultrahand Overlay

An [Ultrahand Overlay](https://github.com/ppkantorski/Ultrahand-Overlay) package for Nintendo Switch that provides an in-game menu for toggling cheats, game actions, display options, and performance settings in Halo: Combat Evolved.

[![Halo CE Ultrahand Cheats Overlay](https://img.youtube.com/vi/gJC8OGUAqBc/maxresdefault.jpg)](https://www.youtube.com/watch?v=gJC8OGUAqBc)

---

## Requirements

Before installing, make sure your Switch has the following installed and working:

1. **Custom Firmware**: A modified Nintendo Switch running [Atmosphère](https://github.com/Atmosphere-NX/Atmosphere).
2. **Overlay Environment**: [Ultrahand Overlay](https://github.com/ppkantorski/Ultrahand-Overlay) (along with nx-ovlloader / Tesla environment). Tested working on Ultrahand version 2.5.3; updating to the latest version is recommended.
3. **Halo Port**: The Nintendo Switch port (build 119 or later) of [Open CE Universal](https://github.com/thelinkin3000/halo-ce-universal).

---

## Features

### 🎮 Cheats
- **God Mode**: Toggle deathless player (`On` / `Off`).
- **Infinite Ammo**: Toggle unlimited ammo reserves (`On` / `Off`).
- **Bottomless Clip**: Toggle bottomless clip without reloading (`On` / `Off`).
- **Super Jump**: Toggle high jump height (`On` / `Off`).
- **Medusa Mode**: Toggle Medusa gaze mode (`On` / `Off`).
- **Bump Possession**: Toggle bumping into NPCs to possess them (`On` / `Off`).
- **Spawn All Weapons**: Instantly drop all weapons nearby *(hold to execute)*.
- **Spawn All Powerups**: Instantly drop all powerups nearby *(hold to execute)*.
- **Spawn All Vehicles**: Instantly spawn all vehicles nearby *(hold to execute)*.

### 🔄 Game Actions
- **Revert to Last Checkpoint**: Revert game state to the last saved checkpoint *(hold to execute)*.

### ⚙️ Config & Performance
- **Toggle VSync**: Enable or disable VSync (`On` / `Off`).
- **Toggle Interpolation**: Enable or disable display frame interpolation (`On` / `Off`).
- **Show Resolution & FPS**: Enable or disable real-time resolution and framerate overlay (`On` / `Off`).

### 📦 Updates
- **Update Overlay Package**: Download and install the latest release directly from GitHub *(hold to execute)*.

---

## Installation

1. Download or clone this repository.
2. Copy the `switch` folder to the root of your Switch's microSD card:
   ```text
   sdmc:/
   └── switch/
       └── .packages/
           └── halo/
               ├── package.ini
               └── commands/
                   ├── ammo_off.txt
                   ├── ammo_on.txt
                   ├── clip_off.txt
                   ├── clip_on.txt
                   ├── game_revert.txt
                   ├── god_off.txt
                   ├── god_on.txt
                   ├── interp_false.txt
                   ├── interp_true.txt
                   ├── medusa_off.txt
                   ├── medusa_on.txt
                   ├── possession_off.txt
                   ├── possession_on.txt
                   ├── show_res_false.txt
                   ├── show_res_true.txt
                   ├── spawn_powerups.txt
                   ├── spawn_vehicles.txt
                   ├── spawn_weapons.txt
                   ├── super_jump_off.txt
                   ├── super_jump_on.txt
                   ├── vsync_false.txt
                   └── vsync_true.txt
   ```
3. Reinsert the microSD card into your Switch (or transfer via FTP / DBI / USB).

---

## Usage

1. Launch **Halo: Combat Evolved** on your Switch.
2. Open the Tesla / Ultrahand Overlay menu (default hotkey is `L + D-Pad Down + R3`).
3. Select **Halo Settings** from the Ultrahand packages menu, accessed by pressing right on d-pad.
4. Navigate through the categories (**Cheats**, **Game Actions**, **Config & Performance**, or **Updates**) and select the desired command.
   - For commands marked with `;hold=true` (such as spawns and revert), hold the confirm button to execute.

### How It Works

When an option is selected in the overlay:
1. Ultrahand verifies that no previous command is currently pending (`!path_exists /switch/halo/overlay/command.txt`).
2. The corresponding command snippet from `/switch/.packages/halo/commands/` is copied atomically to `/switch/halo/overlay/command.txt`.
3. Halo's internal overlay listener polls for this file, executes the command, and clears the file.
4. An on-screen system notification confirms whether the command was successfully dispatched or if the command queue is busy.

---

## Credits

- **Ryan**: Package author & maintainer.
- **[thelinkin3000](https://github.com/thelinkin3000/halo-ce-universal)**: Halo: Combat Evolved Universal Nintendo Switch port.
- **[ppkantorski](https://github.com/ppkantorski/Ultrahand-Overlay)**: Ultrahand Overlay package manager.
- **[Atmosphère-NX](https://github.com/Atmosphere-NX/Atmosphere)**: Atmosphère Custom Firmware.
