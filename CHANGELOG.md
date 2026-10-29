# Changelog

All notable changes to the ATLAS desktop app. Versions are the installers published under [Releases](https://github.com/matiennn33/atlas-releases/releases); the app offers each new one at start-up.

| Version | Date | In one line |
|---|---|---|
| [0.1.6](#016--not-released-yet) | not released yet | Everything since 0.1.5: Pitwall keeps the whole race, Listen captions, season globe, drivers by face |
| [0.1.5](#015--2026-10-24) | 2026-10-24 | Maintenance build |
| [0.1.4](#014--2026-10-24) | 2026-10-24 | Speed-chart annotations lead with the fastest car; updates from 0.1.2 work again |
| [0.1.3](#013--2026-10-24) | 2026-10-24 | Releases go live only once every file is uploaded |
| [0.1.2](#012--2026-10-24) | 2026-10-24 | A download link that always points at the newest build |
| [0.1.1](#011--2026-10-24) | 2026-10-24 | Updates from inside the app, signed |
| [0.1.0](#010--2026-10-24) | 2026-10-24 | First public release |

---

## 0.1.6 — not released yet

Everything changed since 0.1.5. The installer is not built yet; when it is published, the app offers it at start-up as usual.

### Pit wall

- **The whole race, however late you join.** Opening the pit wall at lap 30, leaving it and coming back, or restarting the app mid-race used to give you a console that began wherever you arrived: no first pit stop, no early gaps. ATLAS now rebuilds the session from everything it has already recorded, so the gaps, stints, stops and lap markers start from lap 1.
- **Listen.** Captions for the onboard you are already watching (F1 TV in a browser, a broadcaster's onboard channel). ATLAS listens to your computer's own sound and writes the words down locally; nothing is sent anywhere and no stream is opened.
- **Season globe.** The pit wall opens on a rotating Earth with every round of the season. Drag it, press a venue, and its weekend opens.
- **Race calls.** Overtakes, stops and incidents appear as calls. The newest is a full card, older ones fold into a line you can reopen, and calls can be muted.
- **Pop-out windows that stay on top**, so the timing can sit over the broadcast on the same monitor.
- **Eleven panels rebuilt:** report, race control, investigations, track limits, energy, tyres, pit stops, race pace, degradation, lap times and race trace, each with driver faces and smooth reordering.
- **Timing boards** (speed traps, best sectors, finish line, championship) read as ranked lists with a gap bar per car; equal values share a place.
- Sector flags on the track map.

### Analyze

- **Results or best lap, Q1, Q2 or Q3.** The driver and lap picker splits a race into the official result and the best lap in the race, and qualifying into its three parts, with who was knocked out where.
- **Verdict on one sheet.** Thirteen reads in five groups, each with a dot per lap; the best is judged at the precision shown, so a tie no longer lights up as a win.
- **Telemetry probe deck.** A lap ribbon to scrub along and zoom into a sector, a ledger of every lap at the cursor, speed difference and combined-g traces, trace presets.
- **Gap trace.** The comparison summary draws each lap's cumulative gap to the fastest at every timing line.
- **Three or more laps at once.** Mini-sector ownership across the field, and a rival switch to duel any one car.
- **Driving style measured from zero**, a corner-by-corner ribbon, and redesigned energy and conditions reads.

### Everywhere else

- **Drivers by face and full name** across the app: results, standings, summaries, pickers, pit wall. The three-letter code stays only where space is tight.
- **Home page.** A night "stage" with the race week, a Continue strip back to what you were reading, the latest result replayed as cars crossing the finish line, the title fight with the points still on the table, earlier weekends and the news, with what is new since your last visit.
- **Race Story in six chapters** (who led, strategies, retirements) and the opening movers in Race Start.
- **A calmer look.** Neutral greys on deep black, no frosted glass, one blue accent; the motion stays.

---

## 0.1.5 — 2026-10-24

Maintenance build. Install it over any earlier version, or accept the update prompt from 0.1.1 or later; sessions and layouts stay.

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
