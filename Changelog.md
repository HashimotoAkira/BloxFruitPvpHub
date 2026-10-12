# Changelog

## [2.6.0]

### Added
- Added configurable M1 and skill rush movement modifiers.
- Added a switchable ESP rendering backend for Drawing API and ScreenGui, with reusable render-object pools.
- Added richer server-browser sorting, bounty filtering, and refresh behavior.
- Added aim lock support with the `B` key to pin the current target while fighting.
- Added sea-event targeting support for `Boat` and `SeaBeast` / `Leviathan` entities.
- Expanded combat and ESP detection to better categorize enemies in ocean events and sea zones.

### Improved
- Improved entity tracking and classification for players, monsters, boats, and sea beasts / Leviathan targets.
- Improved dash, flashstep, Geppo, jump, and flight controls, including movement adjustments for supported transformations.
- Improved the Monitor tab's live script/game uptime, FPS, ping, and memory reporting.
- Improved optional executor API lookup with environment fallbacks.
- Improved cleanup of hooks, tasks, connections, tracked entities, anti-stun helpers, and render resources.
- Improved entity tracking and target priority logic for sea mobs and boat-like objects.
- Refined combat and visuals filtering to reduce false positives and improve target selection.
- Optimized the script's internal targeting and rendering flow for smoother operation.


### Fixed
- Fixed anti-stun cleanup paths so temporary helper objects and converted forces can be restored when the feature stops or the script unloads.
- Fixed lifecycle cleanup to stop registered feature callbacks and release pooled ESP resources during a full unload.
- Fixed the fog-removal issue where full map fog could not be cleared correctly.
- Improved s
