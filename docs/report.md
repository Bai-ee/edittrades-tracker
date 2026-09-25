# EditTrades call tracker report

Generated 2026-09-25 16:27Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 5 forward record (2.5R gross, net gate off), start 2026-09-24, ends 2026-10-08
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 2 / 14, plans scored 2 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −1.00R | 2 | 0% | 2 / 2 | 2 | – | 2026-09-25 16:27Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 2 | 2 | 0% | −1.00R | 0 / 2 | 0 | 0 | 0 | 2 / 0 | [2 SCORED · TOO FEW TO JUDGE] |
| WATCH | 124 | 52 | 17.3% | −0.30R | 9 / 43 | 3 | 59 | 10 | 2 / 50 | FILTER CONFIRMED |
| BAD | 184 | 44 | 43.2% | −0.29R | 19 / 25 | 2 | 25 | 113 | 44 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 16:27Z | BTC | WATCH | 3m | long | 84075.9 / 83920.1 / 84820.624 | pending |
| 2026-09-25 16:17Z | BTC | BAD | 1m | long | 84042.1 / 83919.9 / 84075.9 | open |
| 2026-09-25 16:17Z | SOL | BAD | 1m | long | 120.85 / 120.45 / 121.06 | pending |
| 2026-09-25 15:21Z | SOL | plan:conditional | 3m | long | 120.83 / 119.97 / 123.45 | pending |
| 2026-09-25 14:07Z | BTC | WATCH | 3m | short | 83587.3 / 84113.5 / 82545.424 | open |
| 2026-09-25 13:57Z | ETH | WATCH | 3m | short | 2680.35 / 2706.39 / 2637.9048 | open |
| 2026-09-25 12:37Z | SOL | plan:conditional | 1m | long | 120.56 / 119.88 / 122.57 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 185 | 46 | 20 | 25 | 2 | 44.4% | −0.25R | −1.64R | 0.33 | 6 | 9 |
| WATCH | 127 | 56 | 9 | 45 | 3 | 16.7% | −0.33R | −1.38R | 1.55 | 24 | 41 |
| GOOD | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −2.41R | 0.85 | 2 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 124 | 54 | 9 | 43 | 3 | 17.3% | −0.30R | −1.37R | – | 24 | 41 |
| rr_below_min | 72 | 46 | 20 | 25 | 2 | 44.4% | −0.25R | −1.64R | 0.33 | 6 | 9 |
| room_at_entry | 64 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 49 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 3 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.65R | 1.55 | 2 | – |
| ready_flag_plan | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −2.41R | 0.85 | 2 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |
| SOL | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −1.69R | 1.63 | 1 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 185 | 46 | 20 | 25 | 2 | 44.4% | −0.25R | −1.64R | 0.33 | 6 | 9 |
| WATCH | 127 | 56 | 9 | 45 | 3 | 16.7% | −0.33R | −1.38R | 1.55 | 24 | 41 |
| GOOD | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −2.41R | 0.85 | 2 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 124 | 54 | 9 | 43 | 3 | 17.3% | −0.30R | −1.37R | – | 24 | 41 |
| rr_below_min | 72 | 46 | 20 | 25 | 2 | 44.4% | −0.25R | −1.64R | 0.33 | 6 | 9 |
| room_at_entry | 64 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 49 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 3 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.65R | 1.55 | 2 | – |
| ready_flag_plan | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −2.41R | 0.85 | 2 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |
| SOL | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −1.69R | 1.63 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 | 138 | 1 | 59 | 78 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 687, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 2 / max 20.1, missing 1m candles 0.
