# Changelog


### [Improvements & Fixes - v2.2.1]
- **Entity Tracker:** Implemented a robust hash-map `EntityTracker` module for high-performance entity and player monitoring.
- **ESP System & Silent Aim:** Decoupled the ESP rendering pipeline from targeting logic, ensuring stable and independent Silent Aim functionality.
- **Anti-Lava:** Added strict, safe neutralization for dangerous lava parts across map zones, including Prehistoric Island.
- **Server Browser:** Optimized server list fetching with batch-processing requests to prevent rate-limiting (`HTTP 429`).
- **Water Platform:** Optimized the `ManageWaterWalking` system using a persistent memory cache (`memoryWaterCache`) to significantly reduce lag and maintain smooth performance.
