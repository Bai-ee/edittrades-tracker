# EditTrades call tracker report

Generated 2026-09-24 08:37Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 4 forward paper record, start 2026-09-23, ends 2026-10-07
- Target: 14 days / >= 30 scored plans
- Progress: day 2 / 14, plans scored 0 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| [NO SCORED CALLS YET] | 0 | – | 0 / 0 | 0 | – | 2026-09-24 08:37Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 0 | 0 | – | – | 0 / 0 | 0 | 0 | 0 | 0 / 0 | [0 SCORED · TOO FEW TO JUDGE] |
| WATCH | 13 | 5 | 0% | −1.00R | 0 / 5 | 0 | 4 | 4 | 0 / 5 | FILTER CONFIRMED |
| BAD | 16 | 3 | 33.3% | −0.15R | 1 / 2 | 3 | 4 | 6 | 3 / 0 | [3 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 08:37Z | BTC | BAD | 1m | short | 83845.6 / 83955 / 83730.1 | pending |
| 2026-09-24 08:37Z | ETH | BAD | 1m | short | 2673.27 / 2677.65 / 2669.97 | pending |
| 2026-09-24 08:37Z | SOL | BAD | 1m | short | 114.35 / 114.71 / 114.3 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 16 | 3 | 1 | 2 | 3 | 33.3% | −0.15R | 0.18 | 2 | 78 |
| WATCH | 13 | 5 | 0 | 5 | 0 | 0% | −1.00R | – | 5 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 13 | 5 | 0 | 5 | 0 | 0% | −1.00R | – | 5 | – |
| rr_below_min | 10 | 3 | 1 | 2 | 3 | 33.3% | −0.15R | 0.18 | 2 | 78 |
| chase | 3 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |
| room_at_entry | 3 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |

Ready plans by symbol:

_none yet_


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 16 | 3 | 1 | 2 | 3 | 33.3% | −0.15R | 0.18 | 2 | 78 |
| WATCH | 13 | 5 | 0 | 5 | 0 | 0% | −1.00R | – | 5 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 13 | 5 | 0 | 5 | 0 | 0% | −1.00R | – | 5 | – |
| rr_below_min | 10 | 3 | 1 | 2 | 3 | 33.3% | −0.15R | 0.18 | 2 | 78 |
| chase | 3 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |
| room_at_entry | 3 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |

Ready plans by symbol:

_none yet_


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 | 25 | 0 | 10 | 15 | 0 | 0 | 0 | 0 | – |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 81, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.9 / max 11.2, missing 1m candles 0.
