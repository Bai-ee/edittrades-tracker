# EditTrades call tracker report

Generated 2026-09-24 10:47Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 4 forward paper record, start 2026-09-23, ends 2026-10-07
- Target: 14 days / >= 30 scored plans
- Progress: day 2 / 14, plans scored 0 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| [NO SCORED CALLS YET] | 0 | – | 0 / 0 | 0 | – | 2026-09-24 10:47Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 0 | 0 | – | – | 0 / 0 | 0 | 0 | 0 | 0 / 0 | [0 SCORED · TOO FEW TO JUDGE] |
| WATCH | 23 | 8 | 37.5% | +0.48R | 3 / 5 | 4 | 7 | 4 | 0 / 8 | FILTER MAY BE BLOCKING WINNERS |
| BAD | 29 | 6 | 66.7% | +0.36R | 4 / 2 | 3 | 5 | 15 | 6 / 0 | FILTER MAY BE BLOCKING WINNERS |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 10:47Z | BTC | BAD | 3m | long | 83293.1 / 83147.2 / 83501 | pending |
| 2026-09-24 09:47Z | BTC | BAD | 5m | short | 83279.8 / 83715.2 / 82288.1 | open |
| 2026-09-24 09:47Z | ETH | WATCH | 3m | short | 2638.22 / 2651.27 / 2591.8925 | open |
| 2026-09-24 09:37Z | BTC | BAD | 3m | short | 83310.5 / 83715.2 / 82288.1 | open |
| 2026-09-24 09:07Z | BTC | WATCH | 3m | short | 83358.9 / 83715.2 / 81994.271 | open |
| 2026-09-24 09:07Z | ETH | WATCH | 3m | short | 2659.36 / 2672.94 / 2615.904 | open |
| 2026-09-24 08:47Z | BTC | WATCH | 1m | short | 83655.6 / 83860.7 / 82816.741 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 29 | 8 | 4 | 2 | 3 | 66.7% | +0.36R | 0.68 | 2 | 6 |
| WATCH | 23 | 12 | 3 | 5 | 4 | 37.5% | +0.48R | – | 5 | 35 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 23 | 12 | 3 | 5 | 4 | 37.5% | +0.48R | – | 5 | 35 |
| rr_below_min | 14 | 8 | 4 | 2 | 3 | 66.7% | +0.36R | 0.68 | 2 | 6 |
| room_at_entry | 8 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |
| chase | 7 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |

Ready plans by symbol:

_none yet_


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 29 | 8 | 4 | 2 | 3 | 66.7% | +0.36R | 0.68 | 2 | 6 |
| WATCH | 23 | 12 | 3 | 5 | 4 | 37.5% | +0.48R | – | 5 | 35 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 23 | 12 | 3 | 5 | 4 | 37.5% | +0.48R | – | 5 | 35 |
| rr_below_min | 14 | 8 | 4 | 2 | 3 | 66.7% | +0.36R | 0.68 | 2 | 6 |
| room_at_entry | 8 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |
| chase | 7 | 0 | 0 | 0 | 0 | – | – | – | 0 | – |

Ready plans by symbol:

_none yet_


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-24 | 48 | 0 | 20 | 28 | 0 | 0 | 0 | 0 | – |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Data health

_provisional; not evidence of an edge_

Captures 123, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 2.1 / max 13, missing 1m candles 0.
