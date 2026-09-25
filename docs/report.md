# EditTrades call tracker report

Generated 2026-09-25 09:57Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

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
| −1.00R | 1 | 0% | 1 / 1 | 1 | – | 2026-09-25 09:57Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 0% | −1.00R | 0 / 1 | 0 | 0 | 0 | 1 / 0 | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 101 | 43 | 14% | −0.42R | 6 / 37 | 5 | 44 | 9 | 0 / 43 | FILTER CONFIRMED |
| BAD | 156 | 40 | 47.5% | −0.22R | 19 / 21 | 1 | 21 | 94 | 40 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 09:57Z | BTC | WATCH | 5m | long | 84781.3 / 84479 / 85648.901 | pending |
| 2026-09-25 09:57Z | ETH | WATCH | 5m | long | 2712.13 / 2700.28 / 2758.7005 | pending |
| 2026-09-25 09:57Z | SOL | WATCH | 5m | long | 118.68 / 118.06 / 121.3088 | pending |
| 2026-09-25 09:47Z | SOL | plan:null | 5m | long | 117.72 / 117.32 / 119.08 | pending |
| 2026-09-25 09:37Z | BTC | BAD | 5m | long | 84667 / 84479 / 84861.8 | open |
| 2026-09-25 09:27Z | BTC | WATCH | 3m | long | 84771.3 / 84458.5 / 85409.412 | open |
| 2026-09-25 09:17Z | ETH | WATCH | 5m | long | 2696.26 / 2684.55 / 2724.7153 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 157 | 42 | 20 | 21 | 1 | 48.8% | −0.18R | −1.56R | 0.28 | 6 | 9 |
| WATCH | 104 | 47 | 6 | 39 | 5 | 13.3% | −0.45R | −1.60R | – | 24 | 29 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 104 | 47 | 6 | 39 | 5 | 13.3% | −0.45R | −1.60R | – | 24 | 29 |
| rr_below_min | 63 | 42 | 20 | 21 | 1 | 48.8% | −0.18R | −1.56R | 0.28 | 6 | 9 |
| room_at_entry | 51 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 43 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
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
| BAD | 157 | 42 | 20 | 21 | 1 | 48.8% | −0.18R | −1.56R | 0.28 | 6 | 9 |
| WATCH | 104 | 47 | 6 | 39 | 5 | 13.3% | −0.45R | −1.60R | – | 24 | 29 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 104 | 47 | 6 | 39 | 5 | 13.3% | −0.45R | −1.60R | – | 24 | 29 |
| rr_below_min | 63 | 42 | 20 | 21 | 1 | 48.8% | −0.18R | −1.56R | 0.28 | 6 | 9 |
| room_at_entry | 51 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 43 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| ready_flag_plan | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 | 86 | 0 | 36 | 50 | 0 | 0 | 0 | 0 | – |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 564, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.8 / max 20.1, missing 1m candles 0.
