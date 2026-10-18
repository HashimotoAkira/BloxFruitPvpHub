# Blox Fruits Combat Hub

![Version](https://img.shields.io/badge/version-3.0.0-blue.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

A configurable Blox Fruits utility hub for combat, movement, visual information, and quality-of-life controls. Version 3.0.0 introduces a redesigned WindUI interface with searchable tabs and subtabs.

This repository contains the **public release loader**. The editable source and build workspace are maintained separately.

## Features

- **Combat:** configurable combat and aim hotkeys, silent aim, camera aim, FOV controls, target filters, and target priorities.
- **Movement:** fruit flight, free flight and glide, speed controls, jump and Geppo adjustments, dash and rush tuning, Flashstep, and water walking.
- **Visuals:** ESP for players, monsters, and sea events; configurable labels and tracers; environment options including fog clearing and extended camera zoom.
- **Player:** attack speed options, anti-stun controls, Auto Buso Haki, Observation Haki options, and team switching.
- **VFX:** fruit visual styles and custom gradients.
- **Utilities:** anti-AFK and capability-dependent anti-kick protection.
- **Home monitor:** live script/game uptime, memory, FPS, and ping information.
- **Appearance:** built-in themes, custom window background color, and transparent-window option.
- **Configurations:** save, load, delete, and auto-load a selected config using WindUI's configuration manager.

Features that rely on executor APIs may be unavailable in executors that do not provide those APIs.

## Controls

| Key | Action |
| :---: | :--- |
| **`K`** | Toggle the interface. |
| Combat and aim hotkeys | View or change them in the **Combat** tab. |
| Movement controls | View the selected flight mode and its controls in **Movement**. |

## Quick Start

Run this in a supported Roblox executor:

```lua
getgenv()["BFP_AutoTeam"] = "Pirates" -- Optional: "Pirates" or "Marines"
loadstring(game:HttpGet("https://raw.githubusercontent.com/HashimotoAkira/BloxFruitPvpHub/main/BloxFruitPvpLoader.luau"))()
```

The interface can also be shown or hidden with **K** after it loads.

## Configuration Notes

Version 3.0.0 uses WindUI's configuration format. Configurations created by the previous Fluent-based version are **not imported**; create and save new configurations from the **Configs** tab, then select one and enable **Auto-load selected config** to restore it when the hub starts.

## Changelog

See [Changelog.md](./Changelog.md) for release notes.

## Disclaimer

Use responsibly and in accordance with Roblox's terms and the game's rules. This project is provided as-is; executor compatibility and availability of individual features may vary.
