<p align="center">
  <img src="https://atlasf1.app/atlas-logo.svg" alt="ATLAS" width="72" height="72">
</p>

<h1 align="center">ATLAS</h1>

<p align="center"><strong>Read the race like the pit wall.</strong><br>
A free Formula 1 desktop app for Windows: the official live timing while the session runs, and any lap since 2018 taken apart afterwards. Telemetry, sectors, braking, tyres and strategy, measured to the metre.</p>

<p align="center">
  <a href="https://github.com/matiennn33/atlas-releases/releases/latest/download/ATLAS-Setup.exe"><strong>⬇ Download for Windows</strong></a>
  &nbsp;·&nbsp; <a href="https://github.com/matiennn33/atlas-releases/releases/latest">Latest release</a>
  &nbsp;·&nbsp; <a href="CHANGELOG.md">Changelog</a>
  &nbsp;·&nbsp; <a href="https://atlasf1.app">atlasf1.app</a>
</p>

<p align="center">
  <img alt="Latest release" src="https://img.shields.io/github/v/release/matiennn33/atlas-releases?label=version&color=2448ff">
  <img alt="Downloads" src="https://img.shields.io/github/downloads/matiennn33/atlas-releases/total?color=2448ff">
  <img alt="Platform" src="https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20·%2064--bit-111">
  <img alt="Price" src="https://img.shields.io/badge/price-free-111">
  <img alt="Account" src="https://img.shields.io/badge/ATLAS%20account-none-111">
</p>

---

The TV shows you a few cars. ATLAS shows you every one of them: where they are, how far apart, on which tyres, how fast through each sector, and what race control has just decided. When the session is over, the same data stays on your computer, so you can put two laps on one rail and see exactly where the time was won.

**Free. No ATLAS account. No tracking. Everything is computed and stored on your own machine.**

## What you get

### During the session: your own pit wall
- **Official live timing.** Positions, gaps, intervals, lap and sector times, best sectors and mini-sectors, speed traps, pit stops, tyre ages. The same feed the teams' screens read, signed in with your own F1 TV subscription.
- **Every car on the track map.** Live positions on the official circuit outline, battles highlighted, DRS zones marked.
- **Race control, flags and safety car.** Decisions, investigations, penalties and track-limits strikes as they are published.
- **Team radio.** The radio messages as they come in, with transcripts written on your computer.
- **Onboard camera and broadcast** windows next to the data (F1 TV subscription).
- **Weather at the circuit.** Air and track temperature, wind, humidity, pressure, rain, plus the radar.
- **Strategy, tyres and energy.** Tyre degradation, pit windows, battery and power use per car.
- **Championship prediction and standings** updated lap by lap from the running order.
- **A race diary** that writes the session down as it happens: overtakes, stops, flags, fastest laps.
- **Panels you arrange.** Thirty-plus panels (timing, track map, race trace, race pace, lap times, driver focus, teammate comparison, position changes, gaps, finish-line speed, report and more) to float, minimise, maximise, pop out to a second screen, and save as your own layouts.

### After the session: any lap since 2018, taken apart
- **Analyze.** Tick two or more drivers, pick the laps, press Analyze. The lap opens chapter by chapter: lap time and the gap along the lap, the braking zones, the corners, the straights, the session context.
- **Telemetry channels.** Speed, throttle, brake, gear, RPM, DRS, battery state and ERS deployment, all drawn on one shared distance axis, so every trace lines up to the metre. Each corner and straight is annotated with who was fastest there and by how much.
- **Track dominance.** The circuit coloured by who was quicker in each stretch, with the sector and mini-sector times behind it.
- **Delta time, sectors and lap times.** Official sector times, speed-trap ledgers, ideal laps, lap-time evolution across the session.
- **g-g diagram, power phases, time attribution** and the other engines of the analysis workspace, each labelled by how it was obtained: measured, derived or estimated.
- **Race Story.** A whole race in one scroll, act by act: start, stints, undercuts, safety cars, the finish.
- **Race Start.** The first seconds of the race: reaction, traces, who gained and lost places off the line.
- **Long runs.** Practice sessions read as race simulations: run traces grouped by compound, fuel-corrected pace.
- **Race pace and tyre degradation.** Fuel-corrected field read for races and sprints, per-stint degradation per compound.
- **Replays.** Run any stored session again at up to ten times speed, on the layout you built, as if it were live.

### Around the championship
- **Season register.** Every weekend and session since 2018 with what you have already downloaded, one click from the analysis.
- **Grand Prix results back to 1950**, standings, head-to-head comparisons, driver profiles with teammate mirrors, team pages.
- **FIA documents.** Stewards' decisions and technical bulletins of the weekend, next to the standings.
- **Race-week briefing.** The next weekend is already on the clock when you open the app: schedule in your time zone, the circuit, the form.
- **News** from the paddock.
- **English and Italian.** Light and dark themes. Keyboard-first command palette.

## Install

1. **[Download `ATLAS-Setup.exe`](https://github.com/matiennn33/atlas-releases/releases/latest/download/ATLAS-Setup.exe)** (about 300 MB).
2. Run it. It installs for your user only, no administrator rights needed, and puts ATLAS in the Start menu and on the desktop.
3. If **Windows SmartScreen** stops the installer, choose **More info**, then **Run anyway**. The installer is not yet signed with a paid publisher certificate; the message says nothing else. Every release lists the installer's SHA-256 so you can check what you downloaded.
4. Open ATLAS, choose a weekend and a session. For live timing and for downloading a session you do not have yet, sign in with your F1 TV account under *Settings ▸ Live timing*: Formula 1 asks for that sign-in on its own feed.

### Requirements

| | |
|---|---|
| **System** | Windows 10 or 11, 64-bit. There is no macOS, Linux, phone or tablet version. |
| **Disk** | About 1 GB installed, plus the sessions you download (a race weekend with telemetry is a few hundred MB). |
| **Live timing and new sessions** | Your own active **F1 TV** subscription, signed in inside the app. Sessions already in your library replay and analyse without it. |
| **Network** | Only to Formula 1's live timing and archive, the Jolpica results archive, Open-Meteo weather and the FIA documents site, all from your computer. ATLAS has no servers of its own. |

### Updating

ATLAS checks this repository when it starts and tells you when a newer version is out. Nothing downloads without your say-so: choose *Download update*, then *Restart and install* when it is ready. Each update is signed and the app refuses one that does not verify. You can also run the newest installer over the old one; your sessions and layouts stay.

### Where your data lives

| | |
|---|---|
| App | `%LOCALAPPDATA%\Programs\ATLAS\` |
| Sessions, layouts, transcripts | `%APPDATA%\ATLAS Telemetry\atlas_data\` (*File ▸ Open Data Folder*) |
| Logs | `%APPDATA%\ATLAS Telemetry\logs\` (*File ▸ Open Logs Folder*) |

Uninstalling from Windows Settings removes the app and leaves your data folder in place, so a reinstall finds your library again.

## Questions

**Do I need F1 TV?**
For live timing, yes: ATLAS signs in with your own subscription, on your computer. Formula 1 also asks for an F1 TV sign-in to download a past session. Sessions already in your library replay without it, and the analysis is free.

**Where does the data come from?**
The official F1 live timing feed and its archive, read through [FastF1](https://github.com/theOehrly/Fast-F1), for every session since 2018. Results back to 1950 come from the [Jolpica](https://github.com/jolpica/jolpica-f1) archive. Weather comes from Open-Meteo.

**Does ATLAS send anything anywhere?**
No. There is no ATLAS account, no analytics and no telemetry about you. The app talks only to the data sources above, and your F1 TV sign-in stays on your machine.

**Is the source code here?**
No. This repository hosts the installers and the release notes. ATLAS is proprietary software, free to use; see the [terms](https://atlasf1.app/terms) and the [privacy policy](https://atlasf1.app/privacy).

**Something is wrong.**
Open an [issue](https://github.com/matiennn33/atlas-releases/issues) with what you did, what you expected and, if you can, the log from *File ▸ Open Logs Folder*.

## Verify a download

Each release lists the SHA-256 of its installer. In PowerShell:

```powershell
Get-FileHash .\ATLAS-Setup.exe -Algorithm SHA256
```

The hash must match the one in the release notes.

---

<sub>ATLAS is an independent project. It is unofficial and is not associated in any way with the Formula 1 companies, Formula One Licensing B.V., the FIA or any team. F1, FORMULA ONE, FORMULA 1, FIA FORMULA ONE WORLD CHAMPIONSHIP, GRAND PRIX and related marks are trademarks of Formula One Licensing B.V. ATLAS is not the ATLAS telemetry software by McLaren Applied.</sub>
