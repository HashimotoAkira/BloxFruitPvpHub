# Changelog

## [3.0.0] - 2026-10-18

### Added
- Rebuilt the interface on WindUI with searchable navigation and organized tabs and subtabs.
- Added a Home overview and live monitor for script/game uptime, memory, FPS, and ping.
- Added an Appearance tab with built-in theme presets, custom background color, and window transparency.
- Added an Auto Buso Haki control in the Player tab.
- Added WindUI configuration controls for saving, loading, refreshing, and deleting configurations.

### Changed
- Reorganized Movement into focused groups for jump/Geppo/speed, Flashstep/water, dash/rush, fruit flight, and free flight.
- Reorganized Combat, Visuals, Player, VFX, Utilities, and Configs for easier navigation.
- Bumped the major version to 3.0.0.

### Removed
- Removed the legacy Fluent configuration managers. Existing Fluent configurations are not migrated to WindUI.

### Fixed
- Corrected WindUI subtab and section initialization so later tabs and configuration controls can be created.
- Fixed theme application errors when switching subtab visuals.

## [2.7.1]

### Improved
- Improved flight terrain and corridor handling, including smoother passage through non-collidable objects and open passages.
- Reduced unwanted altitude changes near terrain, players, and monsters.
- Improved flight stability while using skills and prioritized native fruit flight skills.
- Automated version synchronization in the build pipeline.

### Fixed
- Fixed ground-based skill casts accidentally triggering flight or leaving the character airborne.
- Fixed unwanted elevation near gates, doorways, trees, mushrooms, and stepped terrain.
- Fixed flight cancellation and physics issues when using certain skills.
- Fixed dash speed modifiers affecting non-dash skills.
- Fixed character orientation and movement after landing or canceling flight.
