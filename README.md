# bolt-bowl-data

The weekly team-strength file for the Bolt Bowl game's Quick Game. Bolt Bowl is a parody robot football game.
It is not connected to or approved by any sports league or team.

`team-strength.json` is the file the game downloads, about once a week. It is updated every Tuesday. It holds
only plain facts: each team's wins, losses, ties and points for and against this season and last season, and
this week's pairings, all written with the game's own parody team ids. No team names, logos or scores of single
games.

```json
{
  "format": 1,
  "season": 2026,
  "phase": "regular",
  "week": 7,
  "updated": "2026-10-20",
  "source": "weekly",
  "credit": "https://github.com/tuckerfam5/bolt-bowl-data#credit",
  "records": { "detroit-li-ions": {"w": 5, "l": 1, "t": 0, "pf": 172, "pa": 110} },
  "lastSeason": { "detroit-li-ions": {"w": 13, "l": 4, "t": 0, "pf": 480, "pa": 340} },
  "games": [ {"date": "2026-10-25", "home": "detroit-li-ions", "away": "green-bay-packet-loss"} ]
}
```

- `phase` is `regular`, `playoffs` (with `round` 1 to 4) or `offseason`.
- `records` counts regular-season games only. `games` is the coming week; teams on a bye are not in it.

## Credit

Results and schedules come from the nflverse schedules data by Lee Sharpe
(https://github.com/nflverse/nflverse-data/releases/tag/schedules), shared under
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Changed: only win, loss, tie and point totals and one
week's pairings are kept, under Bolt Bowl's own team ids. This file is shared under the same license.
