# EditTrades call tracker report

Generated 2026-09-24 18:27Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 4 forward paper record, start 2026-09-23, ends 2026-10-07
- Target: 14 days / >= 30 scored plans
- Progress: day 2 / 14, plans scored 1 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −1.00R | 1 | 0% | 1 / 1 | 1 | – | 2026-09-24 18:27Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 0% | −1.00R | 0 / 1 | 0 | 0 | 0 | 1 / 0 | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 51 | 26 | 19.2% | −0.15R | 5 / 21 | 4 | 14 | 7 | 0 / 26 | FILTER CONFIRMED |
| BAD | 72 | 14 | 57.1% | −0.03R | 8 / 6 | 1 | 9 | 48 | 14 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 18:27Z | BTC | BAD | 1m | long | 84378.8 / 84304.1 / 84455.4 | pending |
| 2026-09-24 18:27Z | ETH | WATCH | 5m | long | 2684.32 / 2669.97 / 2704.2665 | pending |
| 2026-09-24 18:17Z | SOL | WATCH | 1m | long | 117.08 / 116.71 / 117.931 | open |
| 2026-09-24 17:07Z | BTC | WATCH | 1m | short | 84356.2 / 84540.4 / 83801.758 | open |
| 2026-09-24 17:07Z | ETH | WATCH | 1m | short | 2681.71 / 2690.19 / 2658.5596 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 72 | 14 | 8 | 6 | 1 | 57.1% | −0.03R | −0.91R | 0.47 | 4 | 7 |
| WATCH | 51 | 29 | 5 | 21 | 4 | 19.2% | −0.15R | −1.21R | – | 9 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 51 | 29 | 5 | 21 | 4 | 19.2% | −0.15R | −1.21R | – | 9 | 23 |
| room_at_entry | 31 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 24 | 14 | 8 | 6 | 1 | 57.1% | −0.03R | −0.91R | 0.47 | 4 | 7 |
| chase | 17 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| ready_flag_plan | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 72 | 14 | 8 | 6 | 1 | 57.1% | −0.03R | −0.91R | 0.47 | 4 | 7 |
| WATCH | 51 | 29 | 5 | 21 | 4 | 19.2% | −0.15R | −1.21R | – | 9 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 51 | 29 | 5 | 21 | 4 | 19.2% | −0.15R | −1.21R | – | 9 | 23 |
| room_at_entry | 31 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 24 | 14 | 8 | 6 | 1 | 57.1% | −0.03R | −0.91R | 0.47 | 4 | 7 |
| chase | 17 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| ready_flag_plan | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 | 120 | 1 | 48 | 71 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 273, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 2.1 / max 17.9, missing 1m candles 0.
