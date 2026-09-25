# EditTrades call tracker report

Generated 2026-09-25 22:17Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 5 forward record (2.5R gross, net gate off), start 2026-09-24, ends 2026-10-08
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 2 / 14, plans scored 3 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −1.00R | 3 | 0% | 3 / 3 | 3 | – | 2026-09-25 22:17Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 3 | 3 | 0% | −1.00R | 0 / 3 | 0 | 0 | 0 | 3 / 0 | [3 SCORED · TOO FEW TO JUDGE] |
| WATCH | 140 | 56 | 17.9% | −0.28R | 10 / 46 | 2 | 70 | 12 | 2 / 54 | FILTER CONFIRMED |
| BAD | 205 | 51 | 41.2% | −0.34R | 21 / 30 | 1 | 27 | 126 | 51 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 18:07Z | SOL | WATCH | 5m | long | 121.53 / 119.88 / 124.368 | open |
| 2026-09-25 17:57Z | SOL | plan:conditional | 1m | short | 120.72 / 121 / 120.02 | pending |
| 2026-09-25 16:37Z | SOL | BAD | 5m | long | 121.06 / 119.97 / 123.18 | open |
| 2026-09-25 15:21Z | SOL | plan:conditional | 3m | long | 120.83 / 119.97 / 123.45 | pending |
| 2026-09-25 13:57Z | ETH | WATCH | 3m | short | 2680.35 / 2706.39 / 2637.9048 | open |
| 2026-09-25 12:37Z | SOL | plan:conditional | 1m | long | 120.56 / 119.88 / 122.57 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 206 | 53 | 22 | 30 | 1 | 42.3% | −0.30R | −1.79R | 0.39 | 8 | 9 |
| WATCH | 143 | 60 | 10 | 48 | 2 | 17.2% | −0.31R | −1.32R | 1.55 | 24 | 38 |
| GOOD | 3 | 3 | 0 | 3 | 0 | 0% | −1.00R | −2.15R | 1.01 | 3 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 139 | 58 | 10 | 46 | 2 | 17.9% | −0.28R | −1.31R | – | 24 | 38 |
| rr_below_min | 80 | 53 | 22 | 30 | 1 | 42.3% | −0.30R | −1.79R | 0.39 | 8 | 9 |
| room_at_entry | 72 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 54 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 4 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.65R | 1.55 | 2 | – |
| ready_flag_plan | 3 | 3 | 0 | 3 | 0 | 0% | −1.00R | −2.15R | 1.01 | 3 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.66R | 1.49 | 2 | – |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 206 | 53 | 22 | 30 | 1 | 42.3% | −0.30R | −1.79R | 0.39 | 8 | 9 |
| WATCH | 143 | 60 | 10 | 48 | 2 | 17.2% | −0.31R | −1.32R | 1.55 | 24 | 38 |
| GOOD | 3 | 3 | 0 | 3 | 0 | 0% | −1.00R | −2.15R | 1.01 | 3 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 139 | 58 | 10 | 46 | 2 | 17.9% | −0.28R | −1.31R | – | 24 | 38 |
| rr_below_min | 80 | 53 | 22 | 30 | 1 | 42.3% | −0.30R | −1.79R | 0.39 | 8 | 9 |
| room_at_entry | 72 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 54 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 4 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.65R | 1.55 | 2 | – |
| ready_flag_plan | 3 | 3 | 0 | 3 | 0 | 0% | −1.00R | −2.15R | 1.01 | 3 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.66R | 1.49 | 2 | – |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 | 176 | 2 | 75 | 99 | 2 | 2 | 0 | 2 | −1.00R |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 795, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.9 / max 20.1, missing 1m candles 0.
