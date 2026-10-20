# Blox Fruits Combat Hub — Source and Build Workspace

![Version](https://img.shields.io/badge/version-3.1.1-blue.svg)

This repository is the editable source and build workspace for Blox Fruits Combat Hub. The public release loader is maintained in the separate **BloxFruitPvPHub** repository; keep its README and changelog in sync with this project's release notes.

## Features

- **Combat:** configurable combat and aim hotkeys, silent aim, camera aim, FOV controls, target filters, and target priorities.
- **Movement:** fruit flight, free flight and glide, speed controls, jump and Geppo adjustments, dash and rush tuning, Flashstep, and water walking.
- **Visuals:** ESP for players, monsters, and sea events; configurable labels and tracers; environment options including fog clearing and extended camera zoom.
- **Player:** attack speed options, Anti-Pin, Anti-Stun and Full Anti-Stun controls, Auto Buso Haki, Observation Haki options, and team switching.
- **VFX:** fruit visual styles and custom gradients.
- **Utilities:** anti-AFK and capability-dependent anti-kick protection.
- **Home monitor:** live script/game uptime, memory, FPS, ping, Bounty, and Honor.
- **Mini live stats:** a compact edge control opens a live panel for FPS, ping, time, Bounty, and Honor. The edge controls can be hidden or shown in **Appearance**.
- **Appearance:** built-in themes, custom window background color, and transparent-window option.
- **Configurations:** save, load, delete, and auto-load a selected config using WindUI's configuration manager.

Features that rely on executor APIs may be unavailable in executors that do not provide those APIs.

## Controls

| Key | Action |
| :---: | :--- |
| **`K`** | Toggle the interface. |
| Combat and aim hotkeys | View or change them in the **Combat** tab. |
| Movement controls | View the selected flight mode and its controls in **Movement**. |

## Build

The BloxFruitPvPMain builder embeds the sibling WindUI build from `..\WindUI\dist\main.lua`. Build WindUI first, then build the hub:

```powershell
Set-Location ..\WindUI
bash build/build.sh build

Set-Location ..\BloxFruitPvPMain
.\build\build.cmd
```

The build writes the bundled script to `dist\BFP.lua`. Set `VERSION` in `.env` before building a release.

## Public Loader

The public loader is in the separate BloxFruitPvPHub repository:

```lua
getgenv()["BFP_AutoTeam"] = "Pirates" -- Optional: "Pirates" or "Marines"
loadstring(game:HttpGet("https://raw.githubusercontent.com/HashimotoAkira/BloxFruitPvpHub/main/BloxFruitPvpLoader.luau"))()
```

## Configuration Compatibility

Version 3.1.0 uses WindUI's configuration format. Previous Fluent-based configurations are intentionally not imported. Save new configurations from the **Configs** tab, then select one and enable **Auto-load selected config** to restore it when the hub starts.

## Changelog

See [changelog.md](./changelog.md) for release notes.

## Disclaimer

Use responsibly and in accordance with Roblox's terms and the game's rules. This project is provided as-is; executor compatibility and availability of individual features may vary.
