# RS Optimization v1.17.0 — Game Library & Automatic Performance Sessions

## Game Library

- Added a dedicated Game Library page under Gaming.
- Added local detection for FiveM, GTA V, Counter-Strike 2, Call of Duty / Warzone, Fortnite, VALORANT, League of Legends, Minecraft and Rocket League.
- Added Steam, Epic Games, Riot Client and known standalone-install detection.
- Added real Installed, Running and Not Detected states.
- Added Launch Through RS and manual library refresh.
- Added custom games: choose any game executable and give it an RS automatic profile. Removing a custom entry never deletes game files.
- Added favorites so important games remain at the top.

## RS Gaming Mode

- Added automatic game-start and game-exit detection.
- Added optional Auto Boost and Auto Restore controls.
- Added per-game Lite, Balanced, Performance, Competitive and Extreme modes.
- Modes now control the temporary Windows power plan and supported process priority instead of being cosmetic labels.
- The previous power plan is restored after the game closes and when RS closes during an active session.
- Security software, anti-cheat and protected Windows processes are never stopped automatically.
- Added notifications when Performance Mode starts and when the previous state is restored.

## Profiles, favorites and history

- Added validated profile Import and Export using the versioned `.rsprofiles.json` format.
- Added favorite optimizations throughout the utility pages.
- Added local game-session history with game, profile, duration and whether automatic boost was active.
- Session information remains stored locally in the RS application-data folder.

## Health and recovery

- Added a six-hour periodic PC health check.
- Added hardware-change detection with a recommendation to run Smart Scan again.
- Added Windows build-change detection after updates.
- Added detection for previously applied optimizations that Windows later reset.
- Added low-system-drive-space warnings.
- Added first-run onboarding that opens the real scan and recommendations flow.

## Benchmark sharing

- Added export of measured Before/After benchmark results as a 1200×675 PNG report.
- Reports include CPU throughput, memory bandwidth, latency, CPU/RAM load and packet loss.
- Missing measurements remain N/A; RS does not invent FPS or benchmark values.

## Optimization interface and tools

- Simplified utility pages into searchable cards with category tabs, selection switches and one Apply Selected action.
- Added real DNS benchmarking across six resolvers and the option to apply the fastest measured result to the active adapter.
- Added SSD Auto TRIM using the documented Windows `fsutil` control.
- Added a safe BIOS Advisor instead of automatic BIOS unlocking.
- Added Latency Lab with 11 existing, documented and reversible controls.

## Safety

- Existing backup, restore ledger, profile recovery and One-Click Restore remain intact.
- Changes stay reviewable before application.
- Auto Restore uses the power plan captured at game-session start.
- No automatic Defender, firewall, Windows Update or anti-cheat disabling was added.

## Validation

- Windows x64 Release build completed with 0 errors.
- All 58 functional checks passed.
- The existing non-blocking high-DPI manifest compiler warning remains unchanged.
