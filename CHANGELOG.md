# Changelog

All notable changes to the ATLAS desktop app. Versions are the installers published under [Releases](https://github.com/matiennn33/atlas-releases/releases); the app offers each new one at start-up.

| Version | Date | In one line |
|---|---|---|
| [0.1.7](#017--2026-10-31) | 2026-10-31 | Long runs rebuilt, a strategy simulator that runs on real data, and a calmer Analyze header |
| [0.1.6](#016--2026-10-30) | 2026-10-30 | Everything since 0.1.5: Pitwall keeps the whole race, Listen captions, season globe, drivers by face |
| [0.1.5](#015--2026-10-24) | 2026-10-24 | Maintenance build |
| [0.1.4](#014--2026-10-24) | 2026-10-24 | Speed-chart annotations lead with the fastest car; updates from 0.1.2 work again |
| [0.1.3](#013--2026-10-24) | 2026-10-24 | Releases go live only once every file is uploaded |
| [0.1.2](#012--2026-10-24) | 2026-10-24 | A download link that always points at the newest build |
| [0.1.1](#011--2026-10-24) | 2026-10-24 | Updates from inside the app, signed |
| [0.1.0](#010--2026-10-24) | 2026-10-24 | First public release |

---

## 0.1.7 — 2026-10-31

Everything changed since 0.1.6. Install it over any earlier version, or accept the update prompt from 0.1.1 or later; sessions and layouts stay.

### Long runs and strategy

- **Strategy simulation you can trust.** The simulator used to price tyres from traffic laps and from different cars on different compounds, which produced a fake cliff and a 1.8 s gap between softs and mediums nobody had driven. It now fits each compound from steady laps only, compares cars with themselves, and only extrapolates to tyre ages that were actually run. A cliff is shown only if at least half the runs show it.
- **It runs when you arrive.** The race is simulated on open, so the chapter starts on an answer instead of an empty form. The race length is prefilled with the Grand Prix's own distance, and the button is always available (*Race again* draws a new set of races).
- **Inputs you can type into.** Values commit when you leave the field or press Enter; typing "71" no longer snaps to 10 on the way through "7".
- **Two reads.** The compounds (pace, wear, cliff, stint life) next to the stint model they imply, with the tyre age where the curves cross; and the race, with each plan drawn as its legs, its median finish against the quickest and the p10–p90 spread on one shared scale.
- **Race-pace order.** Each car's best run is put on the most-run compound, so the order across the field is comparable. It is labelled as modelled.
- **Traces without the noise.** Slow laps move to a "Slower" rail under the plot, each run gets a dashed trend, and the compound's typical lap is a hairline.
- **A fuller ledger.** Best lap, wear (trend, fuel-corrected), spread, and tyre-age span per run; chips and sentences use the driver's face and family name, and add the compound gap and drift.
- **Run plan.** Lap axis fixed (it was off by one lap); short runs are outlines, long runs solid with their lap count.
- **Across practice** is compact: one column per session, a spark per cell, a side-by-side delta and a rookie group.

### Analyze

- **The picker folds into the session header** once a session is open: the Grand Prix title is the switch, with Season, Round and Session menus beside it, and a *Download again* button. The "Session loaded" button and the pick-a-session eyebrow are gone.
- **Lap times.** The scale fits flying laps and slower laps sit on a rail below; a hollow dot marks a deleted lap, the session best is labelled once, and picked laps carry a ring and a code tag.
- **Lap tray.** Chips run fastest first with a delta on the others, and the bar is wider.
- **Gap builds through the lap.** The comparison summary is now a sector waterfall: one row per rival on a shared scale, green for time taken back, red for time lost, with a sentence on each.
- **Verdict.** New proofs for top speed, speed trap, the field spread and, in practice, laps run; the highlight only appears on hover or focus.
- **Page loading** shows a thin line under the masthead and an outline of the page instead of a blank screen.

### Pit wall

- **Race calls open on their own** and stay open, up to three at once, with entry, ageing and exit motion. A call that settles replaces the open one for the same driver ("Under investigation › Noted"), and the exit is now visible.
- **Timing summary** is one sentence: who leads by how much, how many cars are within a second, fastest lap, top speed, whether the pit lane is clear.
- **Driver versus.** The interval sits inside the gap meter, empty rows are hidden, and a rival who cannot be compared is struck through.
- **Track.** A short battle line on top, two-line sector cells, tag leader lines when labels pack, and corner numbers that follow the width.

### Everywhere else

- A dock and toolbar that lift as you scroll, a larger on-air dot, and a Ctrl K hint in the masthead.
- Mexico City added to the data: straight-mode figures and FP2 metadata.

---

## 0.1.6 — 2026-10-30

Everything changed since 0.1.5. Install it over any earlier version, or accept the update prompt from 0.1.1 or later; sessions and layouts stay.

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
