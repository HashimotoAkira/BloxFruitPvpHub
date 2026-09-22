# Blox Fruits Combat Hub - Pro Edition

![Version](https://img.shields.io/badge/version-2.1.0-blue.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

---

## 📖 Introduction

**Blox Fruits Combat Hub - Pro Edition** is a comprehensive enhancement suite for Blox Fruits, delivering combat assistance, advanced mobility, visual ESP, and player utilities wrapped in a sleek, customizable user interface. It features real-time performance diagnostics and an integrated configuration manager.

---

## ⌨️ Hotkeys & Quick Controls

| Input / Key | Feature | Description |
| :--- | :--- | :--- |
| **`K`** | **Toggle UI Menu** | Show or hide the main interface window. |
| **`G`** | **Master Combat Hotkey** | Instantly toggle the combat and targeting system. Includes a cursor indicator dot (Green = Active, Red = Inactive). |
| **Hold Right Mouse Button (`M2`)** | **Camera Aimbot** | Smoothly locks and tracks the camera onto the active target. |

---

## 🌟 Features Overview

### 1. ⚔️ Combat
* **Aura Hit (Manual M1)**: Automatically extends melee attack reach during standard attacks (M1).
* **Master Combat Hotkey**: Global toggle key for all targeting and combat features (Default: `G`).
* **Silent Aim**: Automatically directs attacks and skill projectiles to the target within your aim radius without turning or shaking your camera.
* **Camera Aimbot**:
  * Option to lock the camera directly onto targets when holding Right Mouse Button (`M2`).
  * **Camera Smoothness**: Slider to calibrate camera tracking smoothness (1 to 20).
* **FOV Configuration (Field of View)**:
  * **Show FOV Circle**: Toggle visual display of the targeting circle centered on your cursor.
  * **FOV Radius**: Slider to adjust the targeting area size (10 to 1000).
* **Target Filters & Priority**:
  * **Target: Players**: Toggle targeting of other players (automatically skips crew and party allies).
  * **Target: Monsters**: Toggle targeting of NPCs and monsters.
  * **Prioritize Monsters**: Prioritizes NPCs over players when both are present.
  * **Prioritize Lowest Health**: Prioritizes targets with the lowest remaining HP.
  * **Prioritize Distance to Character**: Calculates closest target relative to your character's position rather than the cursor.
  * **Max Aim Distance**: Maximum 3D engagement range slider (100 to 6000 studs).
  * *Targeting Priority Hierarchy:* Level Bracket -> Entity Category -> Lowest Health -> Distance.

---

### 2. 👁️ Visuals (ESP)
* **Master ESP Controls**:
  * Toggle ESP overlays across the game world.
  * Independent toggles for **Players** (`Render Players`) and **Monsters** (`Render Monsters`).
  * **Render Allies & Shadows**: Highlights allies and shadow entities with distinctive green coloring.
* **Information Tags**:
  * **Display Distance**: Shows distance to the target in meters/studs.
  * **Display Level**: Displays the target's current level.
  * **Display DisplayName**: Displays display names instead of usernames.
  * **Truncate Long Names**: Automatically shortens lengthy names for a cleaner display.
  * **Ken Haki Status**: Displays Observation Haki status and remaining dodges.
* **Tracers**:
  * Draws visual tracer lines from your screen to targets.
  * **Tracer Origin**: Select line starting position (`Bottom` of screen, `Mouse` cursor, or `Center` of screen).
  * **Tracer Range**: Maximum distance limit slider for drawing tracer lines (100 to 6000 studs).
* **Environment Enhancements**:
  * **Infinite Camera Zoom**: Removes camera zoom limits for unrestricted zoom-out distance.
  * **Clear Map Fog & Visual Shakes**: One-click button to clear all ocean/map fog and remove camera shaking effects.

---

### 3. 🏃 Player & Mobility
* **Attack & Speed Buffs**:
  * **Loop Attack Speed Multiplier**: Toggle and slider to boost basic attack / sword swing speed (1x to 5x).
  * **Gun Shoot Speed**: Slider to increase gun firing speed (1x to 5x).
  * **Speed Multiplier**: Multiplies character running speed (1x to 10x).
  * **Unbreakable Super Armor**: Prevents skill animations and charge-ups from being interrupted when taking damage.
  * **Anti-Stun Engine**: Minimizes crowd control effects, allowing movement, gun fire (M1), and neutralizing enemy pull/drag forces.
* **Fruit Flight**:
  * **Fly Speed Mod**: Increases movement speed while flying with fruit abilities (1x to 5x).
* **Custom Dash**:
  * **Custom Dash Engine**: Optimizes dash responsiveness and reduces stamina consumption.
  * **Dash Length Buff**: Increases dash travel distance (1 to 100 studs).
* **Jump & Geppo (Skyjump)**:
  * **Custom Geppo Engine**: Upgraded multi-stage jump mechanics.
  * **Infinite SkyJump Charges**: Unlimited Geppo jumps without running out of charges.
  * **Infinite Space Jump**: Jump repeatedly in mid-air by holding the space bar.
  * **Custom Jump Power**: Slider to adjust jump height (50 to 300).
* **Custom Flashstep (Soru)**:
  * **Modded Flashstep**: Increases teleport distance, automatically targets locked enemies, and remains usable while stunned.
  * **Air Flashstep Cursor Aim**: Teleports towards sky/air coordinates based on cursor location.
  * **Reduce Flashstep Cooldown**: Slider to decrease the cooldown time between Flashsteps.
* **Water Walking**:
  * **Solid Water Surface**: Solidifies water surfaces, allowing you to walk, run, and jump over water without sinking or taking sea damage.
* **Anti Lava**:
  * **Lava Remove**: No longger lava dmg (passive)
* **Faction Switcher**:
  * **Switch Team: Pirates**: One-click button to switch to the Pirates faction.
  * **Switch Team: Marines**: One-click button to switch to the Marines faction.

---

### 4. ✨ Fruit VFX Customization
* **Visual Style Mode**: Customizes the color appearance of fruit ability visual effects:
  * **Rainbow**: Dynamic cycling across the full color spectrum.
  * **Custom Transition**: Smooth gradient transition between two custom colors.
  * **Static Presets**: Solid color choices including `Red`, `Blue Moonlight`, `Purple-pink`, `Lotus Pink`, `White`, and `Black`.
* **Custom Color Gradient**: Dual color pickers (`Color 1` and `Color 2`) for creating personalized color transitions.

---

### 5. 📊 Performance Monitor
* Real-time statistics display:
  * **Script Uptime**: Total runtime of the script session.
  * **Game Uptime**: Total uptime of the current game server.
  * **Memory Usage (Lua)**: RAM consumed by the script environment (MB).
  * **Frames Per Second (FPS)**: Live FPS counter.
  * **Ping**: Current network latency to the server (ms).

---

### 6. ⚙️ Settings & Utilities
* **Protection**:
  * **Anti-Kick Protection**: Blocks client-side disconnect and kick attempts.
  * **Anti-AFK Keep Alive**: Prevents being disconnected for 20-minute idle inactivity.
* **Config Manager**:
  * Create, save, load, and delete custom setting profiles.
  * **Autoload Config**: Automatically applies your preferred settings upon script execution.
* **External Utilities**:
  * **Open Dex Explorer**: Launches the Dex game explorer.
  * **Open Infinite Yield**: Launches the Infinite Yield administration command suite.
* **Lifecycle**:
  * **Completely Unload Script**: Safely unbinds all listeners, clears UI elements, and restores original game settings.

---

## 🚀 How to Use

### 1. Auto Team Selection (Optional)
To automatically join a faction upon entering the game, set the environment variable prior to executing the loader:

```lua
-- Options: "Pirates" (or "P") / "Marines" (or "M")
getgenv()["BFP_AutoTeam"] = "Pirates"
```

### 2. Loader Script
Execute the following script in your executor:

```lua
getgenv()["BFP_AutoTeam"] = "Pirates" -- "Pirates" or "P" or "Marines" or "M"
loadstring(game:HttpGet("https://raw.githubusercontent.com/HashimotoAkira/HashimotoAkira-BloxFruitPvpHub/main/BloxFruitPvpLoader"))()
```

> **Note:** For optimal stability, execute the script manually after fully loading into the game rather than placing it in Auto Execute.

---

## ⚠️ Disclaimer
Please use this script responsibly. The developers are not liable for any account restrictions or consequences resulting from its usage.
