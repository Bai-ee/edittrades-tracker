# EditTrades call tracker report

Generated 2026-09-24 19:17Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

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
| −1.00R | 1 | 0% | 1 / 1 | 1 | – | 2026-09-24 19:17Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 0% | −1.00R | 0 / 1 | 0 | 0 | 0 | 1 / 0 | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 50 | 27 | 18.5% | −0.18R | 5 / 22 | 3 | 13 | 7 | 0 / 27 | FILTER CONFIRMED |
| BAD | 76 | 15 | 53.3% | −0.17R | 8 / 7 | 3 | 9 | 49 | 15 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 19:17Z | BTC | BAD | 1m | long | 84487 / 84375.3 / 84600 | pending |
| 2026-09-24 19:17Z | ETH | BAD | 1m | long | 2690.06 / 2686.59 / 2690.19 | pending |
| 2026-09-24 19:17Z | SOL | BAD | 1m | long | 117.42 / 117.23 / 117.62 | pending |
| 2026-09-24 19:07Z | ETH | WATCH | 1m | short | 2681.74 / 2684.4 / 2667.4026 | pending |
| 2026-09-24 18:27Z | ETH | WATCH | 5m | long | 2684.32 / 2669.97 / 2704.2665 | open |
| 2026-09-24 18:17Z | SOL | WATCH | 1m | long | 117.08 / 116.71 / 117.931 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 77 | 16 | 9 | 7 | 3 | 56.3% | −0.06R | −0.99R | 0.42 | 4 | 6 |
| WATCH | 53 | 31 | 5 | 24 | 3 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 53 | 31 | 5 | 24 | 3 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| room_at_entry | 32 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 28 | 16 | 9 | 7 | 3 | 56.3% | −0.06R | −0.99R | 0.42 | 4 | 6 |
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
| BAD | 77 | 16 | 9 | 7 | 3 | 56.3% | −0.06R | −0.99R | 0.42 | 4 | 6 |
| WATCH | 53 | 31 | 5 | 24 | 3 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 53 | 31 | 5 | 24 | 3 | 17.2% | −0.24R | −1.28R | – | 12 | 23 |
| room_at_entry | 32 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 28 | 16 | 9 | 7 | 3 | 56.3% | −0.06R | −0.99R | 0.42 | 4 | 6 |
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
| 2026-09-24 | 127 | 1 | 50 | 76 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 291, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 2.2 / max 17.9, missing 1m candles 0.
