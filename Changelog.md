# Changelog

## [2.7.1]

### Improved
- **Flight Elevation & Corridor Awareness**:
  - Non-collidable parts (such as decorative foliage, pass-through gates, and transparent boundaries) are now ignored during flight raycasting, allowing smooth pass-through without unnecessary elevation.
  - Flight altitude lowered to tightly skim the terrain (just inches above the grass) for a realistic, close-to-ground gliding feel.
  - Flight now distinguishes between solid terrain steps and open passages (such as archways, gates, doorways, bridges, and tree canopies), allowing you to fly straight through openings without being forced onto the roof.
  - Ground detection now intelligently filters out other players and monsters, preventing erratic height bounces or sudden flight cancellation when flying over enemies.
  - Normal third-person downward camera pitch will no longer press your character down into rising ground or steps.
  - Active forward flight no longer accidentally cancels when brushing against ledges or elevated terrain.
  - Boats remain fully solid, allowing seamless landing and hovering on player and enemy vessels.
  - Completely eliminated mid-air freezing and stuttering when activating skills during flight.
  - Native fruit flight skills (F) now take full priority and operate smoothly without interference.
- **Build Pipeline**:
  - Automated version synchronization for new releases.

### Fixed
- Fixed an issue where casting skills with velocity while on the ground would mistakenly trigger flight or leave the character floating.
- Fixed character getting pulled onto the roof when flying through arched gates, doorways, or under small trees and mushrooms.
- Fixed character getting pressed down against stepped ledges or scraping against inclined terrain during flight.
- Fixed an issue where casting certain skills could cancel flight or cause physics lag.
- Fixed dash speed multiplier applying to non-dash skills (such as hovering or ground-slam attacks).
- Fixed character getting stuck or facing the wrong direction after landing or canceling flight.

