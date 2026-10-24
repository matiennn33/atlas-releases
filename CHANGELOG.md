# Changelog

All notable changes to the ATLAS desktop app. Versions are the installers published under [Releases](https://github.com/matiennn33/atlas-releases/releases); the app offers each new one at start-up.

## 0.1.4 — 2026-10-24

### Fixed
- **Analyze › Telemetry channels.** Each corner and straight annotation on the speed chart now leads with the driver who was fastest *at that point* and shows the others as deltas from it. Until now every block was headed by the selected driver, so a corner where another car carried more speed still read as the selected driver's number with a positive delta next to it.
- **Updating from 0.1.2.** The 0.1.3 release was missing its versioned installer file, so an app that accepted the 0.1.3 update got a download error. This release is complete; the update prompt works again.

## 0.1.3 — 2026-10-24

### Fixed
- A release is published only after every file is uploaded. A release became "latest" the moment it was created, and an app that checked for updates while the 300 MB installer was still uploading read the new version and then failed to download it.

## 0.1.2 — 2026-10-24

### Changed
- Every release also ships its installer as `ATLAS-Setup.exe`, without the version in the name, so the Download button on [atlasf1.app](https://atlasf1.app) always points at the newest build.

## 0.1.1 — 2026-10-24

### Added
- **Updates from inside the app.** ATLAS checks this repository at start-up and shows "ATLAS x.y.z is available" with *Download update* / *Later*. Nothing downloads on its own; once downloaded, *Restart and install* or let it install on the next quit.
- **Signed updates.** Each release is signed with ATLAS's own update key and the app installs an update only if the signature verifies for the announced version.

## 0.1.0 — 2026-10-24

First public release of ATLAS for Windows.

- **Pit wall.** Official live timing with your F1 TV sign-in, track map, race control, team radio with local transcripts, onboard and broadcast windows, weather and radar, strategy, tyres, energy, championship prediction, race diary, and thirty-plus panels to arrange, float, pop out and save as layouts.
- **Analyze.** Any lap since 2018 taken apart chapter by chapter: lap time and gap, braking zones, corners, straights, session context; telemetry channels on one shared axis; track dominance; delta time, sectors and lap times; g-g diagram, power phases and time attribution.
- **Race Story, Race Start, Long runs, Race pace and tyre degradation**, and replays of any stored session at up to ten times speed.
- **Season register since 2018, results since 1950, standings, head-to-head, driver and team pages, FIA documents, race-week briefing, news.** English and Italian, light and dark.
- Everything computed and stored on your own computer. No ATLAS account, no tracking.
