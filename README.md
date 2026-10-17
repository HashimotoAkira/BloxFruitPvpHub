# Blox Fruits Combat Hub - Pro Edition

![Version](https://img.shields.io/badge/version-2.7.1-blue.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

A high-performance utility hub for Blox Fruits designed for fluid PvP combat, aerial mobility, and clean visual enhancements.

---

## Key Controls

| Key | Action | Description |
| :---: | :--- | :--- |
| **`K`** | Toggle UI | Show or hide the main interface. |
| **`G`** | Combat Toggle | Enable or disable combat targeting & silent aim. |
| **`B`** | Aim Lock | Lock onto your current target during battle. |
| **`Space`** | Free Flight | **Hold in air** to fly; **tap** while flying to cancel. |
| **`Q` + `Space`** | Angel Glide | Hold together for winged gliding mode. |
| **`Q`** | Aerial Dash | Quick dash in flight direction (speed doubles while moving). |
| **`H`** | Ground Lock | Prevents flight from canceling when near the ground or obstacles. |
| **`M2`** (Right Click) | Camera Aim | Smoothly tracks locked target with camera aim. |

---

## Features

### ⚔️ Combat
- **Silent Aim & Camera Aim**: Supports players, bosses, sea beasts, and Leviathans with FOV circle and priority filters.
- **Target Routing**: Smart selection based on lowest health, distance, or entity type.
- **Aim Lock**: Keeps your target locked even during fast-paced aerial fights.

### 🕊️ Movement & Free Flight
- **Free Flight & Gliding**: Full 3D camera-directed flight with customizable speeds and Angel V4 style gliding.
- **Mid-air Skill Maneuvering**: Fly freely while holding skills without losing altitude or momentum.
- **Skill & M1 Rush Speed**: Accelerate your melee dashes and skill dashes for rapid gap closing.
- **Extra Mobility**: Infinite jump, custom dash distance, air flashstep, Geppo modifications, and water walking.

### 👁️ Visuals & ESP
- **Entity ESP**: Customizable boxes, tracers, names, levels, and distance for players, monsters, and sea events.
- **Visual Optimizations**: Removes map fog, screen shake, and visual clutter for clean tracking.
- **Infinite Camera Zoom**: Zoom out as far as needed for wide-angle battlefield awareness.

### 🛡️ Utility & Safety
- **Anti-Stun**: Prevents movement lockups from enemy crowd control.
- **Server Utilities**: Built-in server browser with bounty sorting, server hop, and auto team selection.
- **Protection**: Anti-AFK keepalive and anti-kick protection.

---

## Quick Start

Execute the loader in any supported executor:

```lua
getgenv()["BFP_AutoTeam"] = "Pirates" -- "Pirates" or "Marines"
loadstring(game:HttpGet("https://raw.githubusercontent.com/HashimotoAkira/BloxFruitPvpHub/main/BloxFruitPvpLoader"))()
```

---

## Disclaimer

This script is developed for educational and personal testing purposes. Please use responsibly.
