# Aion 2 Progress Tracker

A single-page tracker for Aion 2 (Global). It runs locally on Windows: no install, no server, no account.

## Run it

1. Download the repo (**Code → Download ZIP**) and unzip it, or `git clone` it.
2. Double-click **`Start-Tracker.bat`**, or open `index.html` in Chrome, Edge or Firefox.
3. Pin the tab, or bookmark the file.

Progress is saved in your browser's local storage. Use **Settings → Export backup** now and then. Restore it with **Import backup**, which also moves your progress to another PC or browser.

## What's in it

| Tab | What it answers |
|---|---|
| **Roadmap** | *Where am I and what's next?* Eight breakpoints, each with one goal, a "done when" condition and a short checklist. Enter your item level and the tracker picks your current breakpoint. |
| **Today** | *What should I do right now?* Daily checklist, plus banked counters (Odyle Energy, Transcendence, Conquest, Nightmare, Shugo keys) sorted by which caps first. |
| **This week** | *What's left before Wednesday?* The weekly checklist, which clears itself at the weekly reset. |
| **Class notes** | Spiritmaster cheat sheet. |
| **Settings** | Server region (sets the reset time), subscription (Odyle cap 560 → 840), backup. |

### The breakpoints

| # | Target | Goal |
|---|---|---|
| 1 | Level 45 | Reach the cap fast with Odyle Energy saved |
| 2 | Item level 1,000 | Collect the one-time "free power", then unlock the Abyss |
| 3 | Item level 1,400 | Start the daily/weekly loop, then unlock Vakron & Urugugu |
| 4 | Item level 1,600 | Get item level 70 Unique gear, then unlock Transcendence |
| 5 | Item level 1,900 | Take Vakron to +10 and slot grey Arcana |
| 6 | Item level 2,100 | Get the green Bell + Mirror Arcana, then unlock Fire Temple |
| 7 | Item level 2,800 | Get item level 86 gear and Transcendence ★3/★4, then raid Ludra |
| 8 | Item level 4,500 | Clear Ludra weekly, then unlock Chalice of Muspel |

### How the counters work

Type the number you see in game and press **Set**. The tracker stores that value with a timestamp and works out the current value from the refill rate, so it keeps counting while the page is closed. Re-sync from the game whenever the number drifts.

Resets are at **09:00 server time** (NA East = New York, NA West = Los Angeles, EU = Berlin). The weekly reset is on **Wednesday**.

## Updating after a patch

All game numbers sit in one block at the top of the `<script>` in `index.html`: `BREAKPOINTS`, `COUNTERS`, `DAILY`, `WEEKLY` and `CLASS_NOTES`. Edit them there. Your saved progress is keyed by ids, so changing text or numbers won't wipe it.

## Changes from the original plan

- **Transcendence** refills +1 every 12 h and banks to 14. **Conquest** refills +1 every 8 h and banks to 21. They also share a 10-cube weekly limit. (The old plan had 2/day, banking to 4 and 14.)
- Resets are at 09:00 server time, and the weekly one is Wednesday.
- Added: Clash Rune at 1,000, Shugo keys (cap 14), 7 weekly Odyle crafts via Substance Morph, Abyss commander scrolls, and the 1,900 → 2,100 Arcana route (Bell of Vigor + Mirror of Magic).
- Muspel's Global entry gate is item level 4,500. Ludra is listed as 2,800, but some guides say 2,700, so check in game.
- The Android app spec was dropped in favour of a single local HTML file.

Numbers come from Global-client guides and community posts around launch (early Oct 2026). Sources include Stoopz's "Everything I Wish I Knew Before Playing AION 2", metabot.gg, mmoexp, game8 and aion2timers. Patches change these numbers, so treat them as a starting point.
