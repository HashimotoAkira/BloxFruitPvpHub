
---

# Blox Fruits Combat Hub - Pro Edition

![Version](https://img.shields.io/badge/version-2.7.1-blue.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

---

## Overview

Blox Fruits Combat Hub - Pro Edition is a feature-rich utility script for Blox Fruits built around a fast targeting system, movement enhancements, ESP, and quality-of-life automation. Version 2.7.1 improves fruit F flight speed, M1/Skill Rush boosts, and transitions between Free Flight and skills.

The latest release is `v2.7.1`.

---

## Key Controls

| Key | Action | Description |
| :--- | :--- | :--- |
| `K` | Toggle UI | Opens or hides the main interface. |
| `G` | Combat toggle | Enables or disables the active combat/aiming system. |
| `B` | Aim Lock | Pins the current target so it stays locked while fighting. |
| `Space` / `Q` | Free Flight (when enabled) | Hold Space while airborne to fly, tap Space while flying to cancel flight, hold Q+Space to glide, tap Q for a 0.2-second dash with a 0.4-second total cooldown; dashing while moving doubles the configured Q dash speed. |
| `H` | Lock Flight (Ground Lock) | Toggle ground-landing lock on/off (prevents flight/glide from canceling when touching ground or obstacles). |
| Right Mouse (`M2`) | Camera aim | Smoothly tracks the current target with camera aimbot behavior. |

---

## Main Features

### Combat
- Silent Aim and camera aim support for players, monsters, and supported sea-event targets.
- FOV circle, target filter controls, and priority settings.
- Target selection by low health, monster priority, and distance-to-character logic.
- Tracks players, monsters, boats, and sea beasts/Leviathans for targeting and ESP.
- Aim lock key and configurable max aim distance.

### Movement & Mobility
- Configurable speed and flight modifiers with a maximum flight-speed cap.
- Flight boost duration, peak multiplier, temporary cap multiplier, and maximum flight speed are adjustable from the Movement tab.
- M1 Rush and Skill Rush toggles and speed multipliers are available in the Movement tab.
- Custom dash, flashstep, and Geppo/sky-jump controls.
- Optional Free Flight and glide modes with camera steering, adjustable flight/glide/dash speeds, and Angel-style flight animations. Free Flight remains steerable while a skill is held, yields after release until the cast ends, and yields immediately to fruit F flight.
- Infinite jump and custom jump power options.
- Transformation-aware movement adjustments and water walking.

### Visuals / ESP
- ESP display options for supported drawing and on-screen GUI modes.
- Player, monster, ally/shadow, and sea-beast rendering options.
- Distance, level, display-name, tracer, box, and target-indicator options.
- Clear map fog and visual shake cleanup.
- Customizable tracer origin and range.
- Infinite zoom support.

### Player Utilities
- Attack speed boosts and gun fire speed modifications.
- Anti-stun and unbreakable armor behavior.
- Observation Haki-related features and utility options.
- Faction switching and combat quality-of-life automation.

### World / Server Tools
- Server browser enhancements with player/bounty sorting, bounty filtering, refresh, and travel controls.
- Auto team selection and manual faction switching.
- Layout support for desktop and mobile UI contexts.

### Performance & Safety
- Live script/game uptime, FPS, ping, and memory monitoring.
- Anti-kick and anti-AFK protective logic.
- Configuration save/load flow with UI-based management.
- Automatic cleanup of temporary effects and movement state.

## Latest Update Summary (v2.7.1)

- Fruit F flight speed boost now applies while holding F; the additional acceleration ramp begins when F is released.
- Improved M1 Rush and Skill Rush speed boosts during movement skills.
- Reduced unexpected speed changes after skills end or weapons are unequipped.
- Free Flight remains steerable while a skill is held, then yields after release until the cast ends; fruit F flight takes control over Free Flight.
- Fixed flight/skill transitions that could leave the character rigid or facing incorrectly.

---

## Getting Started

1. Open a Roblox executor that supports Luau or script injection.
2. Open the UI with the configured keybind (`K` by default).
3. Enable the desired features from the tabs and tune them to your preference.

Example generic execution pattern:

```lua
getgenv()["BFP_AutoTeam"] = "Pirates" -- "Pirates" or "P" or "Marines" or "M"
loadstring(game:HttpGet("https://raw.githubusercontent.com/HashimotoAkira/BloxFruitPvpHub/main/BloxFruitPvpLoader"))()
```

> Use the script only in a supported environment and on accounts you are allowed to play.

---

## Disclaimer

This project is intended for educational and personal customization use. The author is not responsible for account penalties, executor issues, or misuse of automation tools in Roblox.
