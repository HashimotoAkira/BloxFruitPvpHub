
---

# Blox Fruits Combat Hub - Pro Edition

![Version](https://img.shields.io/badge/version-2.6.0-blue.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

---

## Overview

Blox Fruits Combat Hub - Pro Edition is a feature-rich utility script for Blox Fruits built around a fast targeting system, movement enhancements, ESP, and quality-of-life automation. Version 2.6.0 focuses on broader movement controls, flexible ESP rendering, runtime monitoring, and more complete resource cleanup.

This project is maintained as a modular Luau script with a dedicated UI, entity tracking, and a configuration system. The latest version in the source tree is `v2.6.0`.

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
- Silent Aim and camera aim support for players, monsters, and supported sea-event targets.
- FOV circle, target filter controls, and priority settings.
- Target selection by low health, monster priority, and distance-to-character logic.
- Tracks players, monsters, boats, and sea beasts/Leviathans for targeting and ESP.
- Aim lock key and configurable max aim distance.

### Movement & Mobility
- Configurable speed and flight modifiers with a maximum flight-speed cap.
- M1/skill rush movement modifiers.
- Custom dash, flashstep, and Geppo/sky-jump controls.
- Infinite jump and custom jump power options.
- Transformation-aware movement adjustments and water walking.

### Visuals / ESP
- Selectable Drawing API or ScreenGui rendering backends, with pooled ESP objects.
- Player, monster, ally/shadow, and sea-beast rendering options.
- Distance, level, display-name, tracer, box, and target-indicator options.
- Clear map fog and visual shake cleanup.
- Customizable tracer origin and range.
- Infinite zoom support.

### Player Utilities
- Attack speed boosts and gun fire speed modifications.
- Anti-stun and unbreakable armor behavior.
- Observation Haki-related features and safe utility hooks.
- Faction switching and combat quality-of-life automation.

### World / Server Tools
- Server browser enhancements with player/bounty sorting, bounty filtering, refresh, and travel controls.
- Auto team selection and manual faction switching.
- Layout support for desktop and mobile UI contexts.

### Performance & Safety
- Live script/game uptime, FPS, ping, and memory monitoring.
- Anti-kick and anti-AFK protective logic.
- Configuration save/load flow with UI-based management.
- Centralized cleanup for hooks, tasks, connections, entity tracking, and render pools.
- Optional executor API lookup with environment fallbacks; unsupported APIs are not emulated.

## Latest Update Summary (v2.6.0)

- Expanded the modular entity-tracking flow for players, monsters, boats, and sea beasts.
- Added more configurable movement controls, including M1/skill rush modifiers and separate dash, flashstep, and Geppo options.
- Improved ESP backend selection and object reuse for Drawing API and ScreenGui rendering.
- Added live runtime monitoring and expanded server-browser sorting, filtering, and travel handling.
- Strengthened lifecycle cleanup for hooks, tasks, connections, and render resources.

---

## Getting Started

1. Open a Roblox executor that supports Luau or script injection.
2. Open the UI with the configured keybind (`K` by default).
3. Enable the desired features from the tabs and tune them to your preference.

### Executor API lookup

`src/core/Executor.luau` resolves optional APIs from `getgenv()` first, then
the current script environment and `getrenv()`. It only discovers APIs supplied
by the executor; it does not emulate them. For example, `gethui` is optional
and the ESP UI falls back to `CoreGui` or `PlayerGui` when it is unavailable.

The environment separation follows the [ProjectReal environment reference](https://docs.projectreal.gg/en/reference/environment/),
and its [Drawing API reference](https://docs.projectreal.gg/en/reference/drawing/).

Example generic execution pattern:

```lua
getgenv()["BFP_AutoTeam"] = "Pirates" -- "Pirates" or "P" or "Marines" or "M"
loadstring(game:HttpGet("https://raw.githubusercontent.com/HashimotoAkira/BloxFruitPvpHub/main/BloxFruitPvpLoader"))()
```

> Use the script only in a supported environment and on accounts you are allowed to play.

---

## Disclaimer

This project is intended for educational and personal customization use. The author is not responsible for account penalties, executor issues, or misuse of automation tools in Roblox.
