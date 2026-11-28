# Shuttle Fantasy data feed

Published every hour by the Shuttle Fantasy app's data job. Nobody edits it by hand, and each publish replaces the one before.

- `manifest.json`: what's here and when each part was imported. The app checks this first and downloads only the parts that are newer than its own copy.
- `results.json`: fantasy points per Tournament Week for every entry in the player pool, scored from real match results.
- `entries.json`: the player pool, with world ranks and prices.
  - Ranks update whenever the rankings do.
  - Prices change only when a Tournament Week locks.
  - Players who drop off the rankings list stay in the pool, marked `unlisted`.
- `calendar.json`: the Tournament Weeks and their deadlines. Deadlines are estimated from tournament dates.

Everything comes from English Wikipedia (CC BY-SA 4.0), which cites BWF. This feed is shared under the same licence.
