# Changelog

### [New Features - v2.2.0]
- **Advanced Server Browser Overhaul:**
  - Integrated high-speed server fetching combining Roblox Web API with game remotes for real-time accurate player counts.
  - Added dynamic sorting buttons: **Players (Low / High)** and **Bounty (High / Low)**.
  - Added multi-criteria filtering: Search by Region, Server Name, Minimum Bounty, and toggle full server display.
  - Integrated **Quick World & Dungeon Travel**: Instant teleport buttons for Sea 1 (`TravelMain`), Sea 2 (`Dressrosa`), Sea 3 (`Zou`), and Dungeon Hub (`TeleportToDungeonHub`).
  - Added smart progression checks: Dynamically tracks and highlights button readiness based on quest completion (Detective, Key, Ice Boss, Zou) and level requirements (Level 1100+ for Dungeon).
  - Safety & verification mechanisms: Confirmation prompt to avoid accidental teleports, with built-in in-combat teleport blocking.
  - Added responsive UI adaptation that automatically adjusts layout for mobile phone screens.

### [Improvements & Fixes - v2.2.0]
- **Fix Anti-Lava System:** Refactored lava detection to specifically target explicit map containers (`CircleIsland.LavaParts`, `GhostShipInterior.LavaParts`, and `Magma.Lava/LavaParts`), eliminating false positives on other map geometry and reducing scan overhead.
- **Server Hop / Teleport Crash Prevention:** Added an automated `OnTeleport` cleanup pipeline that cancels active threads, disconnects render connections, and purges UI elements prior to cross-server teleportation.
- **Enhanced Metatable Reversion:** Updated `HookManager:Restore` to support an `IsOnTeleport` state, ensuring original metamethods (`__namecall`, `__index`, `__newindex`) and global hook buses are cleanly restored when switching servers.
- **UI Lifecycle Stability:** Removed the aggressive `PlayerGui.ChildRemoved` watchdog loop to eliminate recursive recreation overhead and executor memory leaks.
