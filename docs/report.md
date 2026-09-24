# EditTrades call tracker report

Generated 2026-09-24 20:17Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 5 forward record (net-gated rules), start 2026-09-24, ends 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 1 / 14, plans scored 1 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −1.00R | 1 | 0% | 1 / 1 | 1 | – | 2026-09-24 20:17Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 0% | −1.00R | 0 / 1 | 0 | 0 | 0 | 1 / 0 | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 52 | 27 | 18.5% | −0.18R | 5 / 22 | 2 | 16 | 7 | 0 / 27 | FILTER CONFIRMED |
| BAD | 87 | 19 | 52.6% | −0.17R | 10 / 9 | 3 | 11 | 54 | 19 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 20:17Z | BTC | BAD | 1m | short | 84284.3 / 84455.4 / 84200.8 | pending |
| 2026-09-24 20:17Z | ETH | BAD | 1m | short | 2690.19 / 2694.39 / 2684.32 | pending |
| 2026-09-24 20:17Z | SOL | BAD | 1m | short | 117.08 / 117.36 / 116.71 | pending |
| 2026-09-24 18:27Z | ETH | WATCH | 5m | long | 2684.32 / 2669.97 / 2704.2665 | open |
| 2026-09-24 18:17Z | SOL | WATCH | 1m | long | 117.08 / 116.71 / 117.931 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 88 | 20 | 11 | 9 | 3 | 55% | −0.08R | −1.00R | 0.42 | 4 | 7 |
| WATCH | 55 | 31 | 5 | 24 | 2 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 55 | 31 | 5 | 24 | 2 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| room_at_entry | 37 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 34 | 20 | 11 | 9 | 3 | 55% | −0.08R | −1.00R | 0.42 | 4 | 7 |
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
| BAD | 88 | 20 | 11 | 9 | 3 | 55% | −0.08R | −1.00R | 0.42 | 4 | 7 |
| WATCH | 55 | 31 | 5 | 24 | 2 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 55 | 31 | 5 | 24 | 2 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| room_at_entry | 37 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 34 | 20 | 11 | 9 | 3 | 55% | −0.08R | −1.00R | 0.42 | 4 | 7 |
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
| 2026-09-24 | 140 | 1 | 52 | 87 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 312, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 2.1 / max 17.9, missing 1m candles 0.
