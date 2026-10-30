# EditTrades call tracker report

Generated 2026-10-30 10:07Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 33).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 8 | 6 | 2 | 33.3% | −0.23R | −1.24R | −0.88R | 5.15 | 6 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 32.1).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 33).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 34.4).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −4.72% | −15.41% | 7 | 33 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 33.5).

| Equity now | Equity at start | Trades | Realized net | Kill/arm |
| --- | --- | --- | --- | --- |
| $0.00 | $523.01 | 0 | – | – |

Daily/weekly drawdown kill switch; Steady profile caps $150 size / 100x / $5 per trade / $25 per day / 1 open position.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Net-floor forward record (2.5R gross, net floor live), start 2026-09-27, ends 2026-10-11
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 14 / 14, plans scored 6 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −1.00R | 2 | 0% | 4 / 4 | 2 | – | 2026-10-30 10:07Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 8 | 6 | 33.3% | +0.23R | 2 / 4 | 2 | 0 | 0 | 6 / 0 | 1 | 7 | – | WORKING |
| WATCH | 2429 | 1096 | 27.7% | +0.09R | 303 / 793 | 7 | 1094 | 232 | 5 / 1091 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 3758 | 1079 | 75.8% | −0.03R | 818 / 261 | 3 | 521 | 2155 | 1079 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-10-30 09:54Z | SOL | WATCH | 3m | short | 96.57 / 97 / 95.7014 | open |
| 2026-10-30 09:37Z | SOL | BAD | 5m | short | 96.86 / 97.43 / 96.03 | open |
| 2026-10-30 09:17Z | ETH | plan:ready | 5m | short | 2221.13 / 2230.46 / 2191.49 | open |
| 2026-10-30 09:17Z | ETH | GOOD | 5m | short | 2221.13 / 2230.46 / 2191.49 | open |
| 2026-10-30 09:07Z | ETH | WATCH | 5m | short | 2221.13 / 2230.19 / 2191.5038 | open |
| 2026-10-30 08:57Z | ETH | plan:conditional | 5m | short | 2222.42 / 2232.39 / 2190.12 | pending |
| 2026-10-30 08:57Z | ETH | WATCH | 5m | short | 2222.42 / 2232.39 / 2190.12 | open |
| 2026-10-30 08:57Z | ETH | plan:null | 5m | short | 2222.42 / 2232.39 / 2190.12 | open |
| 2026-10-30 08:47Z | ETH | plan:ready | 3m | short | 2222.96 / 2232.3 / 2198.43 | open |
| 2026-10-30 08:47Z | ETH | GOOD | 3m | short | 2222.96 / 2232.3 / 2198.43 | open |
| 2026-10-30 08:27Z | BTC | WATCH | 3m | short | 77843.4 / 78095.8 / 77260.356 | open |
| 2026-10-30 08:27Z | ETH | WATCH | 3m | short | 2222.62 / 2232.39 / 2194.1893 | open |
| 2026-10-30 08:17Z | BTC | BAD | 1m | long | 77979.4 / 77184.01 / 78120.3 | open |
| 2026-10-30 08:17Z | ETH | plan:conditional | 3m | short | 2228.67 / 2238.03 / 2204.39 | pending |
| 2026-10-30 08:17Z | ETH | WATCH | 3m | short | 2228.67 / 2238.03 / 2204.39 | open |
| 2026-10-30 08:17Z | ETH | plan:null | 3m | short | 2228.67 / 2238.03 / 2204.39 | open |
| 2026-10-30 07:57Z | ETH | WATCH | 1m | short | 2227.29 / 2232.46 / 2207.644 | open |
| 2026-10-30 07:57Z | SOL | BAD | 1m | short | 97.03 / 97.44 / 96.03 | open |
| 2026-10-30 01:37Z | BTC | plan:conditional | 5m | short | 76809.6 / 77178 / 74957.2 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 797 | 231 | 167 | 61 | 3 | 73.3% | −0.03R | −0.36R | 0.4 | 4 | 20 |
| WATCH | 503 | 221 | 66 | 148 | 7 | 30.8% | +0.24R | −1.94R | 2.35 | 12 | 35 |
| GOOD | 4 | 4 | 0 | 2 | 2 | 0% | −1.00R | −1.24R | 2.22 | 2 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 498 | 217 | 66 | 146 | 5 | 31.1% | +0.25R | −1.95R | – | 12 | 35 |
| rr_below_min | 343 | 231 | 167 | 61 | 3 | 73.3% | −0.03R | −0.36R | 0.4 | 4 | 20 |
| chase | 244 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 208 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 5 | 4 | 0 | 2 | 2 | 0% | −1.00R | −1.31R | 2.35 | 2 | – |
| ready_flag_plan | 4 | 4 | 0 | 2 | 2 | 0% | −1.00R | −1.24R | 2.22 | 2 | – |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 3 | 3 | 0 | 1 | 2 | 0% | −1.00R | −1.15R | 2.34 | 1 | – |
| SOL | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −1.34R | 1.86 | 1 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3400 | 981 | 737 | 240 | 3 | 75.4% | −0.04R | −0.36R | 0.32 | 6 | 19 |
| WATCH | 2200 | 994 | 277 | 707 | 7 | 28.2% | +0.11R | −3.28R | 2.15 | 30 | 40 |
| GOOD | 7 | 7 | 1 | 4 | 2 | 20% | −0.23R | −0.52R | 2.19 | 4 | 89 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2190 | 986 | 275 | 704 | 5 | 28.1% | +0.11R | −3.30R | – | 30 | 40 |
| rr_below_min | 1464 | 981 | 737 | 240 | 3 | 75.4% | −0.04R | −0.36R | 0.32 | 6 | 19 |
| chase | 1034 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 900 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 10 | 8 | 2 | 3 | 2 | 40% | +0.58R | +0.28R | 2.15 | 2 | 57 |
| ready_flag_plan | 7 | 7 | 1 | 4 | 2 | 20% | −0.23R | −0.52R | 2.19 | 4 | 89 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 4 | 4 | 0 | 2 | 2 | 0% | −1.00R | −1.24R | 2.28 | 2 | – |
| SOL | 3 | 3 | 1 | 2 | 0 | 33.3% | +0.29R | −0.05R | 2.07 | 2 | 89 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-10-30 | 77 | 3 | 33 | 41 | 3 | 3 | 0 | 1 | −1.00R |
| 2026-10-29 | 222 | 0 | 81 | 141 | 0 | 0 | 0 | 0 | – |
| 2026-10-28 | 198 | 0 | 78 | 120 | 0 | 0 | 0 | 0 | – |
| 2026-10-27 | 181 | 0 | 70 | 111 | 0 | 0 | 0 | 0 | – |
| 2026-10-26 | 185 | 0 | 70 | 115 | 0 | 0 | 0 | 0 | – |
| 2026-10-25 | 190 | 1 | 71 | 118 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-10-24 | 158 | 0 | 65 | 93 | 0 | 0 | 0 | 0 | – |
| 2026-10-23 | 168 | 0 | 64 | 104 | 0 | 0 | 0 | 0 | – |
| 2026-10-22 | 180 | 0 | 70 | 110 | 0 | 0 | 0 | 0 | – |
| 2026-10-21 | 177 | 0 | 65 | 112 | 0 | 0 | 0 | 0 | – |
| 2026-10-20 | 181 | 0 | 69 | 112 | 0 | 0 | 0 | 0 | – |
| 2026-10-19 | 185 | 0 | 72 | 113 | 0 | 0 | 0 | 0 | – |
| 2026-10-18 | 202 | 0 | 78 | 124 | 0 | 0 | 0 | 0 | – |
| 2026-10-17 | 176 | 0 | 67 | 109 | 0 | 0 | 0 | 0 | – |
| 2026-10-16 | 194 | 0 | 74 | 120 | 0 | 0 | 0 | 0 | – |
| 2026-10-15 | 178 | 1 | 73 | 104 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-10-14 | 171 | 1 | 69 | 101 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-10-13 | 191 | 1 | 77 | 113 | 1 | 1 | 1 | 0 | +2.87R |
| 2026-10-12 | 218 | 0 | 91 | 127 | 0 | 0 | 0 | 0 | – |
| 2026-10-11 | 196 | 0 | 78 | 118 | 0 | 0 | 0 | 0 | – |
| 2026-10-10 | 171 | 0 | 73 | 98 | 0 | 0 | 0 | 0 | – |
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
| Live | 24 | 0.67 | 24 | 31.8% | +0.34R | −2.52R |
| NF | 7 | 0.19 | 7 | 20% | −0.23R | −0.52R |

n=24 over 35.92 d (engine 0, backfill 24). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 16128, gaps 33, DATA_UNAVAILABLE 6, mark drift |bps| median 2 / max 153.3, missing 1m candles 0.
