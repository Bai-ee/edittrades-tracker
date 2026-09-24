# EditTrades call tracker report

Generated 2026-09-24 19:47Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

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
| −1.00R | 1 | 0% | 1 / 1 | 1 | – | 2026-09-24 19:47Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 0% | −1.00R | 0 / 1 | 0 | 0 | 0 | 1 / 0 | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 52 | 27 | 18.5% | −0.18R | 5 / 22 | 4 | 14 | 7 | 0 / 27 | FILTER CONFIRMED |
| BAD | 81 | 16 | 56.3% | −0.10R | 9 / 7 | 3 | 11 | 51 | 16 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 19:47Z | ETH | BAD | 1m | long | 2695.55 / 2691.71 / 2697.99 | pending |
| 2026-09-24 19:47Z | SOL | WATCH | 3m | long | 117.63 / 117.24 / 118.4685 | pending |
| 2026-09-24 19:37Z | BTC | WATCH | 3m | long | 84650 / 84539.8 / 85045.618 | pending |
| 2026-09-24 19:37Z | ETH | BAD | 5m | long | 2691.71 / 2672.94 / 2697.99 | open |
| 2026-09-24 19:27Z | BTC | BAD | 3m | long | 84487 / 84200.8 / 84600 | open |
| 2026-09-24 18:27Z | ETH | WATCH | 5m | long | 2684.32 / 2669.97 / 2704.2665 | open |
| 2026-09-24 18:17Z | SOL | WATCH | 1m | long | 117.08 / 116.71 / 117.931 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 82 | 19 | 10 | 7 | 3 | 58.8% | +0.00R | −0.95R | 0.42 | 4 | 7 |
| WATCH | 55 | 31 | 5 | 24 | 4 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 55 | 31 | 5 | 24 | 4 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| room_at_entry | 34 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 31 | 19 | 10 | 7 | 3 | 58.8% | +0.00R | −0.95R | 0.42 | 4 | 7 |
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
| BAD | 82 | 19 | 10 | 7 | 3 | 58.8% | +0.00R | −0.95R | 0.42 | 4 | 7 |
| WATCH | 55 | 31 | 5 | 24 | 4 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 55 | 31 | 5 | 24 | 4 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| room_at_entry | 34 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 31 | 19 | 10 | 7 | 3 | 58.8% | +0.00R | −0.95R | 0.42 | 4 | 7 |
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
| 2026-09-24 | 134 | 1 | 52 | 81 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 303, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 2.1 / max 17.9, missing 1m candles 0.
