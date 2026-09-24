# EditTrades call tracker report

Generated 2026-09-24 12:27Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

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
| −1.00R | 1 | 0% | 1 / 1 | 1 | – | 2026-09-24 12:27Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 0% | −1.00R | 0 / 1 | 0 | 0 | 0 | 1 / 0 | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 28 | 12 | 25% | −0.01R | 3 / 9 | 3 | 9 | 4 | 0 / 12 | FILTER CONFIRMED |
| BAD | 36 | 6 | 66.7% | +0.36R | 4 / 2 | 3 | 7 | 20 | 6 / 0 | FILTER MAY BE BLOCKING WINNERS |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 11:07Z | ETH | BAD | 3m | long | 2651.27 / 2641.76 / 2660.36 | open |
| 2026-09-24 09:47Z | BTC | BAD | 5m | short | 83279.8 / 83715.2 / 82288.1 | open |
| 2026-09-24 09:37Z | BTC | BAD | 3m | short | 83310.5 / 83715.2 / 82288.1 | open |
| 2026-09-24 09:07Z | BTC | WATCH | 3m | short | 83358.9 / 83715.2 / 81994.271 | open |
| 2026-09-24 09:07Z | ETH | WATCH | 3m | short | 2659.36 / 2672.94 / 2615.904 | open |
| 2026-09-24 08:47Z | BTC | WATCH | 1m | short | 83655.6 / 83860.7 / 82816.741 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 36 | 9 | 4 | 2 | 3 | 66.7% | +0.36R | 0.61 | 2 | 6 |
| WATCH | 28 | 15 | 3 | 9 | 3 | 25% | −0.01R | – | 5 | 35 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 28 | 15 | 3 | 9 | 3 | 25% | −0.01R | – | 5 | 35 |
| rr_below_min | 16 | 9 | 4 | 2 | 3 | 66.7% | +0.36R | 0.61 | 2 | 6 |
| room_at_entry | 13 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |
| chase | 7 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |
| ready_flag_plan | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | 0.07 | 1 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | 0.07 | 1 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 36 | 9 | 4 | 2 | 3 | 66.7% | +0.36R | 0.61 | 2 | 6 |
| WATCH | 28 | 15 | 3 | 9 | 3 | 25% | −0.01R | – | 5 | 35 |
| GOOD | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | 0.07 | 1 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 28 | 15 | 3 | 9 | 3 | 25% | −0.01R | – | 5 | 35 |
| rr_below_min | 16 | 9 | 4 | 2 | 3 | 66.7% | +0.36R | 0.61 | 2 | 6 |
| room_at_entry | 13 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |
| chase | 7 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |
| ready_flag_plan | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | 0.07 | 1 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | 0.07 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 | 61 | 1 | 25 | 35 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 153, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.8 / max 13, missing 1m candles 0.
