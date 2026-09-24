# EditTrades call tracker report

Generated 2026-09-24 16:37Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

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
| −1.00R | 1 | 0% | 1 / 1 | 1 | – | 2026-09-24 16:37Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 0% | −1.00R | 0 / 1 | 0 | 0 | 0 | 1 / 0 | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 45 | 21 | 23.8% | +0.05R | 5 / 16 | 3 | 14 | 7 | 0 / 21 | FILTER MAY BE BLOCKING WINNERS |
| BAD | 61 | 11 | 45.5% | −0.14R | 5 / 6 | 1 | 8 | 41 | 11 / 0 | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 16:37Z | BTC | WATCH | 5m | long | 84781.3 / 84455.4 / 86244.591 | pending |
| 2026-09-24 16:37Z | ETH | WATCH | 5m | long | 2697.99 / 2684.32 / 2750.8929 | pending |
| 2026-09-24 16:37Z | SOL | WATCH | 5m | long | 117.45 / 116.71 / 120.8022 | pending |
| 2026-09-24 16:27Z | SOL | BAD | 5m | long | 116.42 / 115.88 / 116.71 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 61 | 11 | 5 | 6 | 1 | 45.5% | −0.14R | −1.10R | 0.53 | 4 | 6 |
| WATCH | 45 | 21 | 5 | 16 | 3 | 23.8% | +0.05R | −1.16R | – | 7 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 45 | 21 | 5 | 16 | 3 | 23.8% | +0.05R | −1.16R | – | 7 | 23 |
| room_at_entry | 25 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 20 | 11 | 5 | 6 | 1 | 45.5% | −0.14R | −1.10R | 0.53 | 4 | 6 |
| chase | 16 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
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
| BAD | 61 | 11 | 5 | 6 | 1 | 45.5% | −0.14R | −1.10R | 0.53 | 4 | 6 |
| WATCH | 45 | 21 | 5 | 16 | 3 | 23.8% | +0.05R | −1.16R | – | 7 | 23 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 45 | 21 | 5 | 16 | 3 | 23.8% | +0.05R | −1.16R | – | 7 | 23 |
| room_at_entry | 25 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 20 | 11 | 5 | 6 | 1 | 45.5% | −0.14R | −1.10R | 0.53 | 4 | 6 |
| chase | 16 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| ready_flag_plan | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −4.04R | 0.07 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 | 103 | 1 | 42 | 60 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 240, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.9 / max 17.9, missing 1m candles 0.
