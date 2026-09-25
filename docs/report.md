# EditTrades call tracker report

Generated 2026-09-25 00:57Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

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
| −1.00R | 1 | 0% | 1 / 1 | 1 | – | 2026-09-25 00:57Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 0% | −1.00R | 0 / 1 | 0 | 0 | 0 | 1 / 0 | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 71 | 33 | 15.2% | −0.33R | 5 / 28 | 5 | 25 | 8 | 0 / 33 | FILTER CONFIRMED |
| BAD | 111 | 25 | 52% | −0.13R | 13 / 12 | 2 | 17 | 67 | 25 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 00:47Z | ETH | WATCH | 1m | short | 2687.2 / 2691.04 / 2682.0544 | pending |
| 2026-09-25 00:37Z | ETH | BAD | 3m | short | 2689.18 / 2693 / 2684.32 | open |
| 2026-09-25 00:35Z | BTC | WATCH | 5m | long | 84652 / 84523.7 / 85288.368 | open |
| 2026-09-25 00:17Z | ETH | BAD | 5m | long | 2692.7 / 2684.32 / 2697.99 | open |
| 2026-09-25 00:07Z | BTC | WATCH | 5m | long | 84479 / 84349.7 / 84981.977 | open |
| 2026-09-25 00:07Z | ETH | WATCH | 5m | long | 2692.7 / 2685.6 / 2710.024 | open |
| 2026-09-24 18:27Z | ETH | WATCH | 5m | long | 2684.32 / 2669.97 / 2704.2665 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 112 | 28 | 14 | 12 | 2 | 53.9% | −0.07R | −1.61R | 0.36 | 4 | 7 |
| WATCH | 74 | 39 | 5 | 30 | 5 | 14.3% | −0.37R | −1.48R | – | 18 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 74 | 39 | 5 | 30 | 5 | 14.3% | −0.37R | −1.48R | – | 18 | 23 |
| rr_below_min | 45 | 28 | 14 | 12 | 2 | 53.9% | −0.07R | −1.61R | 0.36 | 4 | 7 |
| room_at_entry | 42 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 25 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
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
| BAD | 112 | 28 | 14 | 12 | 2 | 53.9% | −0.07R | −1.61R | 0.36 | 4 | 7 |
| WATCH | 74 | 39 | 5 | 30 | 5 | 14.3% | −0.37R | −1.48R | – | 18 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 74 | 39 | 5 | 30 | 5 | 14.3% | −0.37R | −1.48R | – | 18 | 23 |
| rr_below_min | 45 | 28 | 14 | 12 | 2 | 53.9% | −0.07R | −1.61R | 0.36 | 4 | 7 |
| room_at_entry | 42 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 25 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| ready_flag_plan | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 | 11 | 0 | 6 | 5 | 0 | 0 | 0 | 0 | – |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 402, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.8 / max 17.9, missing 1m candles 0.
