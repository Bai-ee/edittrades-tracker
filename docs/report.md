# EditTrades call tracker report

Generated 2026-09-24 07:57Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

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
| [NO SCORED CALLS YET] | 0 | – | 0 / 0 | 0 | – | 2026-09-24 07:57Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 0 | 0 | – | – | 0 / 0 | 0 | 0 | 0 | 0 / 0 | [0 SCORED · TOO FEW TO JUDGE] |
| WATCH | 10 | 5 | 0% | −1.00R | 0 / 5 | 0 | 4 | 1 | 0 / 5 | FILTER CONFIRMED |
| BAD | 10 | 2 | 50% | +0.28R | 1 / 1 | 1 | 2 | 5 | 2 / 0 | [2 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 07:57Z | ETH | BAD | 1m | long | 2697.45 / 2693.33 / 2703 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 10 | 2 | 1 | 1 | 1 | 50% | +0.28R | 0.21 | 1 | 78 |
| WATCH | 10 | 5 | 0 | 5 | 0 | 0% | −1.00R | – | 5 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 10 | 5 | 0 | 5 | 0 | 0% | −1.00R | – | 5 | – |
| rr_below_min | 5 | 2 | 1 | 1 | 1 | 50% | +0.28R | 0.21 | 1 | 78 |
| chase | 3 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |
| room_at_entry | 2 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |

Ready plans by symbol:

_none yet_


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 10 | 2 | 1 | 1 | 1 | 50% | +0.28R | 0.21 | 1 | 78 |
| WATCH | 10 | 5 | 0 | 5 | 0 | 0% | −1.00R | – | 5 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 10 | 5 | 0 | 5 | 0 | 0% | −1.00R | – | 5 | – |
| rr_below_min | 5 | 2 | 1 | 1 | 1 | 50% | +0.28R | 0.21 | 1 | 78 |
| chase | 3 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |
| room_at_entry | 2 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |

Ready plans by symbol:

_none yet_


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 | 16 | 0 | 7 | 9 | 0 | 0 | 0 | 0 | – |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 69, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.9 / max 11.2, missing 1m candles 0.
