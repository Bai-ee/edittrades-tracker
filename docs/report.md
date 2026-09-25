# EditTrades call tracker report

Generated 2026-09-25 12:57Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 5 forward record (2.5R gross, net gate off), start 2026-09-24, ends 2026-10-08
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 2 / 14, plans scored 1 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −1.00R | 1 | 0% | 1 / 1 | 1 | – | 2026-09-25 12:57Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 0% | −1.00R | 0 / 1 | 0 | 0 | 0 | 1 / 0 | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 111 | 46 | 17.4% | −0.31R | 8 / 38 | 2 | 53 | 10 | 0 / 46 | FILTER CONFIRMED |
| BAD | 166 | 41 | 46.3% | −0.24R | 19 / 22 | 0 | 22 | 103 | 41 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 12:47Z | SOL | WATCH | 5m | long | 120.97 / 119.86 / 124.3222 | pending |
| 2026-09-25 12:37Z | SOL | plan:conditional | 1m | long | 120.56 / 119.88 / 122.57 | pending |
| 2026-09-25 12:37Z | SOL | WATCH | 1m | long | 120.56 / 119.88 / 122.57 | open |
| 2026-09-25 12:37Z | SOL | plan:null | 1m | long | 120.56 / 119.88 / 122.57 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 167 | 42 | 20 | 22 | 0 | 47.6% | −0.20R | −1.58R | 0.28 | 6 | 9 |
| WATCH | 114 | 49 | 8 | 40 | 2 | 16.7% | −0.34R | −1.46R | 1.47 | 24 | 38 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 113 | 48 | 8 | 40 | 1 | 16.7% | −0.34R | −1.46R | – | 24 | 38 |
| rr_below_min | 64 | 42 | 20 | 22 | 0 | 47.6% | −0.20R | −1.58R | 0.28 | 6 | 9 |
| room_at_entry | 56 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 47 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 1 | 1 | 0 | 0 | 1 | – | – | – | 1.47 | 0 | – |
| ready_flag_plan | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 167 | 42 | 20 | 22 | 0 | 47.6% | −0.20R | −1.58R | 0.28 | 6 | 9 |
| WATCH | 114 | 49 | 8 | 40 | 2 | 16.7% | −0.34R | −1.46R | 1.47 | 24 | 38 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 113 | 48 | 8 | 40 | 1 | 16.7% | −0.34R | −1.46R | – | 24 | 38 |
| rr_below_min | 64 | 42 | 20 | 22 | 0 | 47.6% | −0.20R | −1.58R | 0.28 | 6 | 9 |
| room_at_entry | 56 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 47 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 1 | 1 | 0 | 0 | 1 | – | – | – | 1.47 | 0 | – |
| ready_flag_plan | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 | 106 | 0 | 46 | 60 | 0 | 0 | 0 | 0 | – |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 621, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.8 / max 20.1, missing 1m candles 0.
