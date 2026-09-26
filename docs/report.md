# EditTrades call tracker report

Generated 2026-09-26 04:57Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 5 forward record (2.5R gross, net gate off), start 2026-09-24, ends 2026-10-08
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 3 / 14, plans scored 4 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −0.05R | 4 | 25% | 4 / 4 | 3 | +2.79R | 2026-09-26 04:57Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 4 | 4 | 25% | −0.05R | 1 / 3 | 0 | 0 | 0 | 4 / 0 | [4 SCORED · TOO FEW TO JUDGE] |
| WATCH | 166 | 66 | 18.2% | −0.27R | 12 / 54 | 7 | 79 | 14 | 4 / 62 | FILTER CONFIRMED |
| BAD | 234 | 55 | 40% | −0.35R | 22 / 33 | 3 | 31 | 145 | 55 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-26 04:57Z | BTC | WATCH | 1m | long | 83979.6 / 83967.8 / 84119.43 | pending |
| 2026-09-26 04:57Z | ETH | WATCH | 3m | long | 2690.87 / 2688.33 / 2694.6292 | pending |
| 2026-09-26 04:57Z | SOL | WATCH | 5m | short | 120.39 / 120.84 / 118.968 | pending |
| 2026-09-26 04:34Z | BTC | BAD | 5m | short | 83925.2 / 84050.3 / 83828.5 | open |
| 2026-09-26 04:34Z | SOL | BAD | 5m | short | 120.56 / 121.06 / 119.97 | open |
| 2026-09-26 04:27Z | BTC | WATCH | 5m | short | 83925.2 / 84050.3 / 83711.279 | open |
| 2026-09-26 03:32Z | SOL | WATCH | 3m | short | 120.69 / 121.06 / 119.2692 | open |
| 2026-09-25 22:47Z | SOL | plan:conditional | 1m | long | 122.37 / 122.2 / 122.83 | pending |
| 2026-09-25 22:27Z | BTC | plan:conditional | 1m | long | 83949.3 / 83924.2 / 84042.1 | pending |
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
| BAD | 235 | 59 | 23 | 33 | 3 | 41.1% | −0.32R | −1.95R | 0.4 | 8 | 9 |
| WATCH | 169 | 72 | 12 | 56 | 7 | 17.7% | −0.30R | −1.85R | 1.06 | 24 | 38 |
| GOOD | 4 | 4 | 1 | 3 | 0 | 25% | −0.05R | −1.85R | 1.01 | 3 | 2 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 163 | 68 | 12 | 52 | 7 | 18.8% | −0.25R | −1.67R | – | 24 | 38 |
| rr_below_min | 90 | 59 | 23 | 33 | 3 | 41.1% | −0.32R | −1.95R | 0.4 | 8 | 9 |
| room_at_entry | 79 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 66 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 6 | 4 | 0 | 4 | 0 | 0% | −1.00R | −4.78R | 1.06 | 4 | – |
| ready_flag_plan | 4 | 4 | 1 | 3 | 0 | 25% | −0.05R | −1.85R | 1.01 | 3 | 2 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 2 | 2 | 1 | 1 | 0 | 50% | +0.89R | −2.05R | 0.07 | 1 | 2 |
| SOL | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.66R | 1.49 | 2 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 235 | 59 | 23 | 33 | 3 | 41.1% | −0.32R | −1.95R | 0.4 | 8 | 9 |
| WATCH | 169 | 72 | 12 | 56 | 7 | 17.7% | −0.30R | −1.85R | 1.06 | 24 | 38 |
| GOOD | 4 | 4 | 1 | 3 | 0 | 25% | −0.05R | −1.85R | 1.01 | 3 | 2 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 163 | 68 | 12 | 52 | 7 | 18.8% | −0.25R | −1.67R | – | 24 | 38 |
| rr_below_min | 90 | 59 | 23 | 33 | 3 | 41.1% | −0.32R | −1.95R | 0.4 | 8 | 9 |
| room_at_entry | 79 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 66 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 6 | 4 | 0 | 4 | 0 | 0% | −1.00R | −4.78R | 1.06 | 4 | – |
| ready_flag_plan | 4 | 4 | 1 | 3 | 0 | 25% | −0.05R | −1.85R | 1.01 | 3 | 2 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 2 | 2 | 1 | 1 | 0 | 50% | +0.89R | −2.05R | 0.07 | 1 | 2 |
| SOL | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.66R | 1.49 | 2 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-26 | 41 | 1 | 18 | 22 | 1 | 1 | 1 | 0 | +2.79R |
| 2026-09-25 | 191 | 2 | 83 | 106 | 2 | 2 | 0 | 2 | −1.00R |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 921, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.7 / max 20.1, missing 1m candles 0.
