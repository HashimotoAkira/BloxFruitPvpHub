
---

# Blox Fruits Combat Hub - Pro Edition

![Version](https://img.shields.io/badge/version-2.5.0-blue.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

---

## Overview

Blox Fruits Combat Hub - Pro Edition is a feature-rich utility script for Blox Fruits built around a fast targeting system, movement enhancements, ESP, and quality-of-life automation. The latest build focuses on cleaner entity detection, better sea-event targeting, and improved map-visual control.

This project is maintained as a compact, modular script bundle with a dedicated UI and a configuration system. The latest version in the source tree is `v2.5.0`.

---

## Key Controls

| Key | Action | Description |
| :--- | :--- | :--- |
| `K` | Toggle UI | Opens or hides the main interface. |
| `G` | Combat toggle | Enables or disables the active combat/aiming system. |
| `B` | Aim Lock | Pins the current target so it stays locked while fighting. |
| Right Mouse (`M2`) | Camera aim | Smoothly tracks the current target with camera aimbot behavior. |

---

## Main Features

### Combat
- Silent Aim and camera aim support for players, monsters, and sea-event targets.
- FOV circle, target filter controls, and priority settings.
- Target selection by low health, monster priority, and distance-to-character logic.
- Supports special sea targets including boats and sea beasts/leviathans.
- Aim lock key and configurable max aim distance.

### Movement & Mobility
- Speed modifiers and flight speed control.
- Dash and flashstep enhancements.
- Jump and geppo/skyjump improvements.
- Infinite jump and custom jump power options.
- Water walking support and boat speed utility placeholders.

### Visuals / ESP
- Player, monster, and sea-beast rendering toggles.
- Distance, level, display-name, tracer, and box options.
- Clear map fog and visual shake cleanup.
- Customizable tracer origin and range.
- Infinite zoom support.

### Player Utilities
- Attack speed boosts and gun fire speed modifications.
- Anti-stun and unbreakable armor behavior.
- Observation Haki-related features and safe utility hooks.
- Faction switching and combat quality-of-life automation.

### World / Server Tools
- Server browser style list with sorting and filtering.
- Quick travel and world hopping helpers.
- Compatible layout for desktop and mobile UI contexts.

### Performance & Safety
- Real-time script/game uptime, FPS, ping, and memory monitoring.
- Anti-kick and anti-AFK protective logic.
- Configuration save/load flow with UI-based management.
- Cleanup and teardown routines to reduce executor instability on teleport or shutdown.

---

## Latest Update Summary (v2.5.0)

Compared with the backup version, the latest script includes:

- Expanded sea target detection for `Boat` and `SeaBeast`/`Leviathan` entities.
- Improved aim and ESP classification for sea-event mobs and boat-like enemies.
- Stabilized map fog removal, including a fix for the issue where fog could not be cleared completely.
- Better entity tracking and filtering logic for combat and visuals.
- Continued optimization around performance, targeting, and script safety.

---

## Getting Started

1. Open a Roblox executor that supports Luau or script injection.
2. Load the latest script from `src/BFP.luau` or the project loader you use for this hub.
3. Open the UI with the configured keybind (`K` by default).
4. Enable the desired features from the tabs and tune them to your preference.

Example generic execution pattern:

```lua
loadstring(readfile("BFP.luau"))()
```

> Use the script only in a supported environment and on accounts you are allowed to play.

---

## Disclaimer

This project is intended for educational and personal customization use. The author is not responsible for account penalties, executor issues, or misuse of automation tools in Roblox.
