# EditTrades call tracker report

Generated 2026-09-25 06:27Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

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
| −1.00R | 1 | 0% | 1 / 1 | 1 | – | 2026-09-25 06:27Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 0% | −1.00R | 0 / 1 | 0 | 0 | 0 | 1 / 0 | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 85 | 38 | 13.2% | −0.42R | 5 / 33 | 4 | 35 | 8 | 0 / 38 | FILTER CONFIRMED |
| BAD | 136 | 35 | 42.9% | −0.30R | 15 / 20 | 4 | 17 | 80 | 35 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 06:27Z | BTC | WATCH | 5m | long | 84278.7 / 84113.5 / 84519.892 | pending |
| 2026-09-25 06:27Z | ETH | BAD | 5m | short | 2677.65 / 2684.32 / 2672.94 | pending |
| 2026-09-25 06:27Z | SOL | WATCH | 5m | short | 116.28 / 116.86 / 115.0794 | pending |
| 2026-09-25 06:17Z | BTC | BAD | 3m | short | 84113.5 / 84278.7 / 83938.8 | open |
| 2026-09-25 06:17Z | ETH | BAD | 3m | short | 2674.83 / 2680.01 / 2672.94 | pending |
| 2026-09-25 04:27Z | BTC | BAD | 5m | short | 84113.5 / 84375.4 / 83938.5 | open |
| 2026-09-25 02:40Z | BTC | WATCH | 5m | short | 84375.3 / 84609.7 / 83936.972 | open |
| 2026-09-24 18:27Z | ETH | WATCH | 5m | long | 2684.32 / 2669.97 / 2704.2665 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 137 | 38 | 16 | 20 | 4 | 44.4% | −0.25R | −1.74R | 0.29 | 6 | 8 |
| WATCH | 88 | 42 | 5 | 35 | 4 | 12.5% | −0.45R | −1.64R | – | 23 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 88 | 42 | 5 | 35 | 4 | 12.5% | −0.45R | −1.64R | – | 23 | 23 |
| rr_below_min | 57 | 38 | 16 | 20 | 4 | 44.4% | −0.25R | −1.74R | 0.29 | 6 | 8 |
| room_at_entry | 47 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 33 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
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
| BAD | 137 | 38 | 16 | 20 | 4 | 44.4% | −0.25R | −1.74R | 0.29 | 6 | 8 |
| WATCH | 88 | 42 | 5 | 35 | 4 | 12.5% | −0.45R | −1.64R | – | 23 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 88 | 42 | 5 | 35 | 4 | 12.5% | −0.45R | −1.64R | – | 23 | 23 |
| rr_below_min | 57 | 38 | 16 | 20 | 4 | 44.4% | −0.25R | −1.74R | 0.29 | 6 | 8 |
| room_at_entry | 47 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 33 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| ready_flag_plan | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −3.13R | 0.07 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-25 | 50 | 0 | 20 | 30 | 0 | 0 | 0 | 0 | – |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 501, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.8 / max 17.9, missing 1m candles 0.
