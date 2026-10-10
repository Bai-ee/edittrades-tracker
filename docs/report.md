# EditTrades call tracker report

Generated 2026-10-10 09:57Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 13).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 1 | 1 | 100% | +1.22R | +1.22R | – | 0 | 1 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 12.1).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 13).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 14.4).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −3.17% | −6.75% | 3 | 13 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 13.5).

| Equity now | Equity at start | Trades | Realized net | Kill/arm |
| --- | --- | --- | --- | --- |
| $521.34 | $523.01 | 0 | – | – |

Daily/weekly drawdown kill switch; Steady profile caps $150 size / 100x / $5 per trade / $25 per day / 1 open position.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Net-floor forward record (2.5R gross, net floor live), start 2026-09-27, ends 2026-10-11
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 14 / 14, plans scored 1 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| [NO SCORED CALLS YET] | 0 | – | 0 / 0 | 0 | – | 2026-10-10 09:57Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 100% | +2.51R | 1 / 0 | 0 | 0 | 0 | 1 / 0 | 1 | 0 | – | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 972 | 440 | 25.7% | −0.04R | 113 / 327 | 4 | 424 | 104 | 3 / 437 | – | – | – | FILTER CONFIRMED |
| BAD | 1493 | 420 | 78.8% | −0.01R | 331 / 89 | 8 | 200 | 865 | 420 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-10-10 09:47Z | BTC | WATCH | 3m | long | 82856.5 / 82810.4 / 83028.453 | pending |
| 2026-10-10 09:37Z | BTC | BAD | 3m | long | 82830.2 / 81985.33 / 82832.3 | open |
| 2026-10-10 09:27Z | ETH | BAD | 5m | long | 2495.35 / 2469.9 / 2497.02 | open |
| 2026-10-10 09:07Z | BTC | WATCH | 5m | long | 82800 / 82698.1 / 83027.237 | open |
| 2026-10-10 08:57Z | ETH | WATCH | 1m | long | 2493.56 / 2493.06 / 2496.76 | open |
| 2026-10-10 08:47Z | ETH | BAD | 1m | short | 2491.37 / 2501.83 / 2489.79 | open |
| 2026-10-10 07:07Z | ETH | BAD | 1m | short | 2491.24 / 2501.7 / 2488.99 | open |
| 2026-10-10 06:37Z | SOL | BAD | 3m | short | 109.76 / 110.22 / 109.46 | open |
| 2026-10-10 06:17Z | SOL | BAD | 1m | short | 109.79 / 110.25 / 109.46 | open |
| 2026-10-10 05:47Z | SOL | BAD | 5m | long | 110.14 / 109.02 / 110.6 | open |
| 2026-10-10 00:27Z | BTC | BAD | 1m | short | 82525.8 / 82872.41 / 82468.7 | open |
| 2026-10-10 00:17Z | ETH | WATCH | 5m | long | 2488.63 / 2482.59 / 2499.7436 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 780 | 242 | 184 | 50 | 8 | 78.6% | +0.01R | −0.31R | 0.31 | 6 | 23 |
| WATCH | 525 | 253 | 62 | 186 | 4 | 25% | −0.06R | −3.57R | 1.96 | 30 | 38 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 521 | 249 | 60 | 185 | 4 | 24.5% | −0.08R | −3.63R | – | 30 | 38 |
| rr_below_min | 356 | 242 | 184 | 50 | 8 | 78.6% | +0.01R | −0.31R | 0.31 | 6 | 23 |
| chase | 247 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 177 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 4 | 4 | 2 | 1 | 0 | 66.7% | +1.63R | +1.34R | 1.96 | 1 | 57 |

Ready plans by symbol:

_none yet_


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 1857 | 511 | 366 | 137 | 8 | 72.8% | −0.04R | −0.67R | 0.3 | 8 | 21 |
| WATCH | 1234 | 554 | 141 | 407 | 4 | 25.7% | −0.01R | −2.74R | 1.57 | 30 | 39 |
| GOOD | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |
| DATA_UNAVAILABLE | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 1221 | 544 | 139 | 400 | 4 | 25.8% | −0.00R | −2.73R | – | 30 | 39 |
| rr_below_min | 756 | 511 | 366 | 137 | 8 | 72.8% | −0.04R | −0.67R | 0.3 | 8 | 21 |
| room_at_entry | 551 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 550 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 13 | 10 | 2 | 7 | 0 | 22.2% | −0.12R | −3.88R | 1.57 | 7 | 57 |
| ready_flag_plan | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |
| missing_data:1m | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 1 | 1 | 1 | 0 | 0 | 100% | +2.51R | +1.22R | 0.53 | 0 | 11 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-10-10 | 70 | 0 | 31 | 39 | 0 | 0 | 0 | 0 | – |
| 2026-10-09 | 169 | 0 | 71 | 98 | 0 | 0 | 0 | 0 | – |
| 2026-10-08 | 187 | 0 | 78 | 109 | 0 | 0 | 0 | 0 | – |
| 2026-10-07 | 151 | 0 | 62 | 89 | 0 | 0 | 0 | 0 | – |
| 2026-10-06 | 192 | 0 | 78 | 114 | 0 | 0 | 0 | 0 | – |
| 2026-10-05 | 205 | 0 | 79 | 126 | 0 | 0 | 0 | 0 | – |
| 2026-10-04 | 206 | 0 | 78 | 128 | 0 | 0 | 0 | 0 | – |
| 2026-10-03 | 204 | 0 | 81 | 123 | 0 | 0 | 0 | 0 | – |
| 2026-10-02 | 201 | 0 | 75 | 126 | 0 | 0 | 0 | 0 | – |
| 2026-10-01 | 186 | 0 | 69 | 117 | 0 | 0 | 0 | 0 | – |
| 2026-09-30 | 190 | 0 | 71 | 119 | 0 | 0 | 0 | 0 | – |
| 2026-09-29 | 179 | 0 | 71 | 108 | 0 | 0 | 0 | 0 | – |
| 2026-09-28 | 195 | 0 | 79 | 115 | 0 | 0 | 0 | 0 | – |
| 2026-09-27 | 195 | 1 | 77 | 117 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-26 | 201 | 2 | 83 | 116 | 2 | 2 | 2 | 0 | +2.67R |
| 2026-09-25 | 191 | 2 | 83 | 106 | 2 | 2 | 0 | 2 | −1.00R |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Net floor · NF (live since 2026-09-27)

_provisional; not evidence of an edge_

| Rule | Calls | Calls / day | Fills | Win rate | Exp. (gross R) | Net exp. (dir-cost) |
| --- | --- | --- | --- | --- | --- | --- |
| Live | 17 | 1.07 | 17 | 35.3% | +0.51R | −3.10R |
| NF | 0 | 0 | 0 | – | – | – |

n=17 over 15.92 d (engine 0, backfill 17). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


## RETEST 1H · paper

_provisional; not evidence of an edge_

[NO RETEST 1H SIGNALS YET]


## HTF ENTRY · live

_provisional; not evidence of an edge_

| Calls | Resolved | Wins | Losses | Win rate | Gross R mean | Gross R median | Net R mean | Net R median | Net R 90% LB | Max DD (R) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | 0 | – | – | – | – | – | – | 0 |

0 resolved signal(s) scored so far. HTF-anchored entries ship live (docs/PROMPT_T20_HTF_ENTRY.md, owner decision 2026-09-27): direction from the 4h+1D EMA21/EMA200 stack, entry from a 1m/3m/5m flag reaching triggering, stop from the 1h swing (NF-floored, 3% scalp-capped), target from the last 1h impulse projected from that swing. Scored here from the 1-minute alert log, same math as RETEST_1H (mean/median/bootstrap 90% lower bound/max drawdown) for comparability — not a promotion gate; this class is already live.


## Data health

_provisional; not evidence of an edge_

Captures 7203, gaps 33, DATA_UNAVAILABLE 3, mark drift |bps| median 1.4 / max 52.3, missing 1m candles 0.
