# Halo Settings & Cheats for Ultrahand Overlay

An [Ultrahand Overlay](https://github.com/ppkantorski/Ultrahand-Overlay) package for Nintendo Switch that provides an in-game menu for toggling cheats, game actions, display options, and performance settings in Halo: Combat Evolved.

[![Halo CE Ultrahand Cheats Overlay](https://img.youtube.com/vi/gJC8OGUAqBc/maxresdefault.jpg)](https://www.youtube.com/watch?v=gJC8OGUAqBc)

---

## Requirements

Before installing, make sure your Switch has the following installed and working:

1. **Custom Firmware**: A modified Nintendo Switch running [Atmosphère](https://github.com/Atmosphere-NX/Atmosphere).
2. **Overlay Environment**: [Ultrahand Overlay](https://github.com/ppkantorski/Ultrahand-Overlay) (along with nx-ovlloader / Tesla environment).
3. **Halo Port**: Supported on both:
   - [Open CE Universal](https://github.com/thelinkin3000/halo-ce-universal) (build 119 or later)
   - [ChupaThingyCE / warthog-switch](https://github.com/ChupathingyCE/warthog-switch)

---

## Features

### 🎮 Cheats
- **God Mode**: Toggle deathless player (`On` / `Off`).
- **Infinite Ammo**: Toggle unlimited ammo reserves (`On` / `Off`).
- **Bottomless Clip**: Toggle bottomless clip without reloading (`On` / `Off`).
- **Super Jump**: Toggle high jump height (`On` / `Off`).
- **Medusa Mode**: Toggle Medusa gaze mode (`On` / `Off`).
- **Bump Possession**: Toggle bumping into NPCs to possess them (`On` / `Off`).
- **Easy Rider**: Prevent vehicle ejection when taking damage (`On` / `Off`).
- **Spawn All Weapons**: Instantly drop all weapons nearby *(hold to execute)*.
- **Spawn All Powerups**: Instantly drop all powerups nearby *(hold to execute)*.
- **Spawn All Vehicles**: Instantly spawn all vehicles nearby *(hold to execute)*.

### 🕹️ HUD
- **HUD Visibility**: Toggle in-game HUD display (`On` / `Off`).
- **Crosshair**: Toggle reticle visibility (`On` / `Off`).
- **Health Bar**: Toggle health bar indicator (`On` / `Off`).
- **Shield Bar**: Toggle shield bar indicator (`On` / `Off`).
- **Motion Sensor**: Toggle radar / motion tracker (`On` / `Off`).

### 🎥 Camera
- **Default Player Camera**: Switch to the standard first-person player camera.
- **Cinematic Camera**: Switch to the scripted cinematic camera.
- **Load Debug Camera**: Load saved debug camera coordinates.
- **Save Debug Camera**: Save current debug camera position.
- **Teleport to Camera**: Teleport player character directly to current camera location.

### ⚡ Game Speed
- **Speed Options**: Set gameplay speed to `1x (Normal)`, `2x`, `3x`, `4x`, `5x`, or `10x`.

### ⚙️ System & Performance
- **VSync**: Toggle VSync (`On` / `Off`).
- **Interpolation**: Toggle frame interpolation (`On` / `Off`).
- **Show Resolution & FPS**: Toggle live resolution and framerate display (`On` / `Off`).
- **Wireframe Mode**: Toggle wireframe rendering (`On` / `Off`).
- **Environment Textures**: Toggle environment diffuse textures (`On` / `Off`).
- **Revert Checkpoint**: Revert game state to last saved checkpoint *(hold to execute)*.

### 📦 Settings
- **Engine Status**: Active engine detection indicator (`OpenCE` / `ChupaThingyCE`).
- **Advanced Mode**: Toggle advanced configuration menu items (`On` / `Off`).
- **Update Halo Overlay**: Download and extract the latest package release directly from GitHub *(hold to execute)*.

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
                   ├── camera_cinematic.txt
                   ├── camera_default.txt
                   ├── camera_load.txt
                   ├── camera_save.txt
                   ├── camera_teleport.txt
                   ├── clip_off.txt
                   ├── clip_on.txt
                   ├── crosshair_off.txt
                   ├── crosshair_on.txt
                   ├── easy_rider_off.txt
                   ├── easy_rider_on.txt
                   ├── env_diffuse_false.txt
                   ├── env_diffuse_true.txt
                   ├── game_revert.txt
                   ├── god_off.txt
                   ├── god_on.txt
                   ├── health_off.txt
                   ├── health_on.txt
                   ├── hud_off.txt
                   ├── hud_on.txt
                   ├── interp_false.txt
                   ├── interp_true.txt
                   ├── medusa_off.txt
                   ├── medusa_on.txt
                   ├── motion_sensor_off.txt
                   ├── motion_sensor_on.txt
                   ├── possession_off.txt
                   ├── possession_on.txt
                   ├── shield_off.txt
                   ├── shield_on.txt
                   ├── show_res_false.txt
                   ├── show_res_true.txt
                   ├── speed_1.txt
                   ├── speed_2.txt
                   ├── speed_3.txt
                   ├── speed_4.txt
                   ├── speed_5.txt
                   ├── speed_10.txt
                   ├── spawn_powerups.txt
                   ├── spawn_vehicles.txt
                   ├── spawn_weapons.txt
                   ├── super_jump_off.txt
                   ├── super_jump_on.txt
                   ├── vsync_false.txt
                   ├── vsync_true.txt
                   ├── wireframe_false.txt
                   └── wireframe_true.txt
   ```
3. Reinsert the microSD card into your Switch (or transfer via FTP / DBI / USB).

---

## Usage

1. Launch **Halo: Combat Evolved** on your Switch.
2. Open the Tesla / Ultrahand Overlay menu (default hotkey is `L + D-Pad Down + R3`).
3. Select **Halo Settings** from the Ultrahand packages menu.
4. Navigate through the categories and select your desired option.
   - For commands marked with `;hold=true`, hold the confirm button to execute.

---

## Credits

- **Ryan**: Package author & maintainer.
- **[thelinkin3000](https://github.com/thelinkin3000/halo-ce-universal)**: Open CE Universal Nintendo Switch port.
- **[ChupathingyCE](https://github.com/ChupathingyCE/warthog-switch)**: ChupaThingyCE (warthog-switch) port.
- **[ppkantorski](https://github.com/ppkantorski/Ultrahand-Overlay)**: Ultrahand Overlay package manager.
- **[Atmosphère-NX](https://github.com/Atmosphere-NX/Atmosphere)**: Atmosphère Custom Firmware.
