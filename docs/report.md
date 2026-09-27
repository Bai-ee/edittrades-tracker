# EditTrades call tracker report

Generated 2026-09-27 15:07Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 5 forward record (2.5R gross, net gate off), start 2026-09-24, ends 2026-10-08
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 4 / 14, plans scored 17 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.51R | 17 | 35.3% | 17 / 17 | 7 | +3.29R | 2026-09-27 15:07Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 17 | 17 | 35.3% | +0.51R | 6 / 11 | 0 | 0 | 0 | 17 / 0 | 15 | 6 | 4 | WORKING |
| WATCH | 279 | 114 | 26.3% | +0.13R | 30 / 84 | 3 | 142 | 20 | 6 / 108 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 392 | 96 | 44.8% | −0.24R | 43 / 53 | 0 | 47 | 249 | 96 / 0 | – | – | – | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-27 15:07Z | BTC | WATCH | 3m | short | 84415.4 / 84678 / 83790.412 | pending |
| 2026-09-27 14:57Z | ETH | WATCH | 1m | short | 2684.12 / 2689.22 / 2671.523 | open |
| 2026-09-27 14:57Z | SOL | WATCH | 1m | short | 121.64 / 122.08 / 120.8612 | open |
| 2026-09-27 01:07Z | BTC | plan:conditional | 1m | short | 84278.7 / 84297.2 / 84218.7 | pending |
| 2026-09-27 00:27Z | BTC | plan:conditional | 1m | short | 84244.8 / 84255.1 / 84200.8 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 393 | 97 | 44 | 53 | 0 | 45.4% | −0.22R | −2.11R | 0.4 | 8 | 12 |
| WATCH | 282 | 119 | 30 | 86 | 3 | 25.9% | +0.11R | −2.37R | 1.06 | 24 | 40 |
| GOOD | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 273 | 113 | 30 | 80 | 3 | 27.3% | +0.17R | −2.14R | – | 24 | 40 |
| rr_below_min | 144 | 97 | 44 | 53 | 0 | 45.4% | −0.22R | −2.11R | 0.4 | 8 | 12 |
| chase | 132 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 117 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 9 | 6 | 0 | 6 | 0 | 0% | −1.00R | −6.49R | 1.06 | 6 | – |
| ready_flag_plan | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 10 | 10 | 1 | 9 | 0 | 10% | −0.63R | −2.54R | 1.55 | 8 | 1 |
| ETH | 4 | 4 | 3 | 1 | 0 | 75% | +2.66R | −4.70R | 0.53 | 1 | 8 |
| BTC | 3 | 3 | 2 | 1 | 0 | 66.7% | +1.45R | −2.84R | 0.07 | 1 | 3 |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 393 | 97 | 44 | 53 | 0 | 45.4% | −0.22R | −2.11R | 0.4 | 8 | 12 |
| WATCH | 282 | 119 | 30 | 86 | 3 | 25.9% | +0.11R | −2.37R | 1.06 | 24 | 40 |
| GOOD | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 273 | 113 | 30 | 80 | 3 | 27.3% | +0.17R | −2.14R | – | 24 | 40 |
| rr_below_min | 144 | 97 | 44 | 53 | 0 | 45.4% | −0.22R | −2.11R | 0.4 | 8 | 12 |
| chase | 132 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 117 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 9 | 6 | 0 | 6 | 0 | 0% | −1.00R | −6.49R | 1.06 | 6 | – |
| ready_flag_plan | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 10 | 10 | 1 | 9 | 0 | 10% | −0.63R | −2.54R | 1.55 | 8 | 1 |
| ETH | 4 | 4 | 3 | 1 | 0 | 75% | +2.66R | −4.70R | 0.53 | 1 | 8 |
| BTC | 3 | 3 | 2 | 1 | 0 | 66.7% | +1.45R | −2.84R | 0.07 | 1 | 3 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-27 | 113 | 1 | 48 | 64 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-26 | 201 | 2 | 83 | 116 | 2 | 2 | 2 | 0 | +2.67R |
| 2026-09-25 | 191 | 2 | 83 | 106 | 2 | 2 | 0 | 2 | −1.00R |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Net floor · NF (live since 2026-09-27)

_provisional; not evidence of an edge_

| Rule | Calls | Calls / day | Fills | Win rate | Exp. (gross R) | Net exp. (dir-cost) |
| --- | --- | --- | --- | --- | --- | --- |
| Live | 17 | 5.43 | 17 | 35.3% | +0.51R | −3.10R |
| NF | 0 | 0 | 0 | – | – | – |

n=17 over 3.13 d (engine 0, backfill 17). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


## Data health

_provisional; not evidence of an edge_

Captures 1557, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.3 / max 20.1, missing 1m candles 0.
