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
| **Roadmap** | *Where am I and what's next?* Each breakpoint has with one goal, a "done when" condition and a short checklist. Every task has a short plain-English explanation under it. Enter your item level and the tracker picks your current breakpoint. |
| **Today** | *What should I do right now?* Daily checklist, plus banked counters (Odyle Energy, Transcendence, Conquest, Nightmare, Shugo keys) sorted by which caps first. |
| **This week** | *What's left before Wednesday?* The weekly checklist, which clears itself at the weekly reset. |
| **Glossary** | Plain-English meanings of game terms (Sealed Dungeon, Daevanion Crystal, Arcana and more), with a search box. |
| **Class notes** | Spiritmaster: skill levels, specialty order, stigmas (with early/mid/late levels), two macro setups, gear/stat/Arcana priorities, PvP and how to reset skills. |
| **Settings** | Server region (sets the reset time) and backup. |

### The breakpoints

These follow the Roadmap tab of the community sheet. Item levels marked ~ are its estimates.

| # | Target | Goal |
|---|---|---|
| 1 | Level 45 | Main Story, plus Sealed Dungeons, Regional quests, feathers and Strongholds along the way |
| 2 | Item level 1,000 | Use up the free power, then go into the Abyss |
| 3 | ~1,400 | Get all gear to +10 with Manastones, which is enough for Vakron Sky Island |
| 4 | 1,600 | Farm the full Vakron set, which opens Deus ★1 |
| 5 | ~1,920 | Collect every green Arcana card from Deus ★1 |
| 6 | ~2,190 | Collect every blue card from Deus ★2 and get main skills to 16 |
| 7 | ~2,560 | Get accessories from Kromede, and armor and Guard from Ferocious Horn Den |
| 8 | Ludra prep | Get yellow cards from Deus ★3/★4 and the Ludra enhancement targets (+17/+16/+15) |

### How the counters work

Type the number you see in game and press **Set**. The tracker stores that value with a timestamp and works out the current value from the refill rate, so it keeps counting while the page is closed. Re-sync from the game whenever the number drifts.

Resets are at **09:00 server time** (NA East = New York, NA West = Los Angeles, EU = Berlin). The weekly reset is on **Wednesday**.

## Updating after a patch

All game numbers sit in one block at the top of the `<script>` in `index.html`: `BREAKPOINTS`, `COUNTERS`, `DAILY`, `WEEKLY` and `CLASS_NOTES`. Edit them there. Your saved progress is keyed by ids, so changing text or numbers won't wipe it.

## Sources

- **Main source:** the [Aion 2 community spreadsheet](https://docs.google.com/spreadsheets/d/1lbHaVairHaz26M8XGNF9CBWqiiHHBM6CylTwNKnlOug/htmlview), using its Roadmap, DailyWeeklies and Spirit Master tabs. The roadmap is credited to Divided.
- [SIRIN's Global Spiritmaster guide](https://docs.google.com/document/d/16RBdqrTCKJ4TZJNEkYri9hLYcMv-Hle2pW6HXSNCX7c/edit?tab=t.0), linked from the sheet and updated 21 Sep 2026. Skills, specialties, stigmas, macros and stats come from it.
- [TheWhelps – 1400 To 2100 Guide, Road To 3 Star Conquest](https://www.youtube.com/watch?v=u3Wb6tH0mZs) is linked on breakpoint 3. Its 1,400 → 2,100 tips come from written guides that cover the same route, because the video's transcript couldn't be fetched.
- Gaps (refill rates, reset times, the raid gates) are filled from Global guides from early Oct 2026: metabot.gg, aion2timers, mmoexp and game8.

Patches change these numbers, so treat them as a starting point.
