# EditTrades call tracker report

Generated 2026-09-28 07:27Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 5 forward record (2.5R gross, net gate off), start 2026-09-24, ends 2026-10-08
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 5 / 14, plans scored 17 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.51R | 17 | 35.3% | 17 / 17 | 7 | +3.29R | 2026-09-28 07:27Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 17 | 17 | 35.3% | +0.51R | 6 / 11 | 0 | 0 | 0 | 17 / 0 | 15 | 6 | 4 | WORKING |
| WATCH | 333 | 136 | 24.3% | +0.02R | 33 / 103 | 6 | 166 | 25 | 6 / 130 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 482 | 117 | 52.1% | −0.18R | 61 / 56 | 2 | 60 | 303 | 117 / 0 | – | – | – | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-28 07:27Z | BTC | WATCH | 5m | short | 82950 / 83316.1 / 82122.614 | pending |
| 2026-09-28 07:27Z | ETH | BAD | 3m | short | 2645.35 / 2656.46 / 2641.99 | pending |
| 2026-09-28 07:17Z | BTC | BAD | 1m | short | 83084.9 / 83433.86 / 82912.9 | open |
| 2026-09-28 05:37Z | SOL | WATCH | 5m | short | 119 / 119.78 / 117.6272 | open |
| 2026-09-28 03:57Z | SOL | WATCH | 5m | short | 119.34 / 120.55 / 117.3556 | open |
| 2026-09-28 02:27Z | BTC | WATCH | 5m | short | 83501 / 83768.8 / 82076.304 | open |
| 2026-09-28 02:27Z | SOL | WATCH | 5m | short | 120.23 / 121.81 / 117.7336 | open |
| 2026-09-28 01:27Z | ETH | WATCH | 5m | short | 2670.12 / 2676.84 / 2634.0336 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 483 | 119 | 62 | 56 | 2 | 52.5% | −0.17R | −1.77R | 0.36 | 8 | 12 |
| WATCH | 336 | 144 | 33 | 105 | 6 | 23.9% | +0.01R | −2.33R | 1.06 | 24 | 39 |
| GOOD | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 327 | 138 | 33 | 99 | 6 | 25% | +0.05R | −2.14R | – | 24 | 39 |
| rr_below_min | 180 | 119 | 62 | 56 | 2 | 52.5% | −0.17R | −1.77R | 0.36 | 8 | 12 |
| room_at_entry | 152 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 151 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
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
| BAD | 483 | 119 | 62 | 56 | 2 | 52.5% | −0.17R | −1.77R | 0.36 | 8 | 12 |
| WATCH | 336 | 144 | 33 | 105 | 6 | 23.9% | +0.01R | −2.33R | 1.06 | 24 | 39 |
| GOOD | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 327 | 138 | 33 | 99 | 6 | 25% | +0.05R | −2.14R | – | 24 | 39 |
| rr_below_min | 180 | 119 | 62 | 56 | 2 | 52.5% | −0.17R | −1.77R | 0.36 | 8 | 12 |
| room_at_entry | 152 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 151 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
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
| 2026-09-28 | 62 | 0 | 25 | 37 | 0 | 0 | 0 | 0 | – |
| 2026-09-27 | 195 | 1 | 77 | 117 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-26 | 201 | 2 | 83 | 116 | 2 | 2 | 2 | 0 | +2.67R |
| 2026-09-25 | 191 | 2 | 83 | 106 | 2 | 2 | 0 | 2 | −1.00R |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Net floor · NF (live since 2026-09-27)

_provisional; not evidence of an edge_

| Rule | Calls | Calls / day | Fills | Win rate | Exp. (gross R) | Net exp. (dir-cost) |
| --- | --- | --- | --- | --- | --- | --- |
| Live | 17 | 4.46 | 17 | 35.3% | +0.51R | −3.10R |
| NF | 0 | 0 | 0 | – | – | – |

n=17 over 3.81 d (engine 0, backfill 17). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


## RETEST 1H · paper

_provisional; not evidence of an edge_

[NO RETEST 1H SIGNALS YET]


## Data health

_provisional; not evidence of an edge_

Captures 1863, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.4 / max 26.2, missing 1m candles 0.
