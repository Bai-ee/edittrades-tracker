# EditTrades call tracker report

Generated 2026-09-28 09:47Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

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
| +0.51R | 17 | 35.3% | 17 / 17 | 7 | +3.29R | 2026-09-28 09:47Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 17 | 17 | 35.3% | +0.51R | 6 / 11 | 0 | 0 | 0 | 17 / 0 | 15 | 6 | 4 | WORKING |
| WATCH | 341 | 141 | 24.8% | +0.03R | 35 / 106 | 7 | 168 | 25 | 6 / 135 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 495 | 121 | 53.7% | −0.16R | 65 / 56 | 5 | 60 | 309 | 121 / 0 | – | – | – | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-28 09:47Z | BTC | BAD | 3m | short | 82674.3 / 83021.53 / 82288.1 | pending |
| 2026-09-28 09:47Z | SOL | BAD | 1m | short | 117.65 / 118.14 / 117.32 | pending |
| 2026-09-28 09:37Z | BTC | WATCH | 3m | short | 82674.3 / 82853.6 / 82258.324 | pending |
| 2026-09-28 09:17Z | BTC | BAD | 5m | short | 82801.8 / 83149.57 / 82293.1 | open |
| 2026-09-28 09:07Z | BTC | WATCH | 5m | short | 82801.8 / 82983 / 82292.628 | open |
| 2026-09-28 08:57Z | BTC | BAD | 1m | long | 82936 / 82090.05 / 83135.7 | open |
| 2026-09-28 08:37Z | BTC | BAD | 5m | short | 82895.3 / 83243.46 / 82517.2 | open |
| 2026-09-28 07:27Z | BTC | WATCH | 5m | short | 82950 / 83316.1 / 82122.614 | open |
| 2026-09-28 05:37Z | SOL | WATCH | 5m | short | 119 / 119.78 / 117.6272 | open |
| 2026-09-28 03:57Z | SOL | WATCH | 5m | short | 119.34 / 120.55 / 117.3556 | open |
| 2026-09-28 02:27Z | BTC | WATCH | 5m | short | 83501 / 83768.8 / 82076.304 | open |
| 2026-09-28 01:27Z | ETH | WATCH | 5m | short | 2670.12 / 2676.84 / 2634.0336 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 496 | 125 | 66 | 56 | 5 | 54.1% | −0.15R | −1.71R | 0.38 | 8 | 11 |
| WATCH | 344 | 150 | 35 | 108 | 7 | 24.5% | +0.01R | −2.26R | 1.06 | 24 | 39 |
| GOOD | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 335 | 144 | 35 | 102 | 7 | 25.6% | +0.06R | −2.08R | – | 24 | 39 |
| rr_below_min | 187 | 125 | 66 | 56 | 5 | 54.1% | −0.15R | −1.71R | 0.38 | 8 | 11 |
| room_at_entry | 157 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 152 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
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
| BAD | 496 | 125 | 66 | 56 | 5 | 54.1% | −0.15R | −1.71R | 0.38 | 8 | 11 |
| WATCH | 344 | 150 | 35 | 108 | 7 | 24.5% | +0.01R | −2.26R | 1.06 | 24 | 39 |
| GOOD | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 335 | 144 | 35 | 102 | 7 | 25.6% | +0.06R | −2.08R | – | 24 | 39 |
| rr_below_min | 187 | 125 | 66 | 56 | 5 | 54.1% | −0.15R | −1.71R | 0.38 | 8 | 11 |
| room_at_entry | 157 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 152 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
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
| 2026-09-28 | 83 | 0 | 33 | 50 | 0 | 0 | 0 | 0 | – |
| 2026-09-27 | 195 | 1 | 77 | 117 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-26 | 201 | 2 | 83 | 116 | 2 | 2 | 2 | 0 | +2.67R |
| 2026-09-25 | 191 | 2 | 83 | 106 | 2 | 2 | 0 | 2 | −1.00R |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Net floor · NF (live since 2026-09-27)

_provisional; not evidence of an edge_

| Rule | Calls | Calls / day | Fills | Win rate | Exp. (gross R) | Net exp. (dir-cost) |
| --- | --- | --- | --- | --- | --- | --- |
| Live | 17 | 4.35 | 17 | 35.3% | +0.51R | −3.10R |
| NF | 0 | 0 | 0 | – | – | – |

n=17 over 3.91 d (engine 0, backfill 17). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


## RETEST 1H · paper

_provisional; not evidence of an edge_

[NO RETEST 1H SIGNALS YET]


## HTF ENTRY · live

_provisional; not evidence of an edge_

[NO HTF ENTRY SIGNALS YET]


## Data health

_provisional; not evidence of an edge_

Captures 1905, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.4 / max 26.2, missing 1m candles 0.
