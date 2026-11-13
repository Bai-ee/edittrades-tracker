# EditTrades call tracker report

Generated 2026-11-13 07:17Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 46.9).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 24 | 22 | 5 | 22.7% | −0.46R | −1.29R | −0.85R | 18.44 | 22 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 46).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 46.9).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 48.3).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −24.71% | 11 | 47 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 47.4).

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
- Progress: day 14 / 14, plans scored 22 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.19R | 10 | 30% | 11 / 11 | 6 | +2.97R | 2026-11-13 07:17Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 24 | 22 | 22.7% | −0.12R | 5 / 17 | 1 | 1 | 0 | 22 / 0 | 1 | 23 | – | NOT WORKING YET |
| WATCH | 3438 | 1539 | 27.8% | +0.10R | 428 / 1111 | 4 | 1596 | 299 | 18 / 1521 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 5214 | 1511 | 74.3% | −0.02R | 1122 / 389 | 3 | 773 | 2927 | 1511 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-13 07:17Z | SOL | WATCH | 1m | long | 80.57 / 80.25 / 81.3988 | pending |
| 2026-11-13 07:07Z | BTC | BAD | 5m | long | 68906.3 / 68203.46 / 70317.3 | pending |
| 2026-11-13 07:07Z | ETH | BAD | 5m | long | 1936.57 / 1916.82 / 1981.12 | pending |
| 2026-11-13 07:07Z | SOL | BAD | 3m | long | 79.97 / 79.15 / 80.37 | pending |
| 2026-11-13 06:37Z | SOL | WATCH | 1m | long | 79.76 / 79.53 / 80.7904 | open |
| 2026-11-13 05:17Z | BTC | plan:conditional | 5m | short | 68506 / 69069.7 / 66355 | pending |
| 2026-11-13 05:17Z | ETH | plan:conditional | 3m | short | 1923.1 / 1931.18 / 1892.52 | pending |
| 2026-11-13 04:07Z | BTC | plan:conditional | 5m | short | 68896 / 69421 / 66856.7 | pending |
| 2026-11-13 04:07Z | BTC | WATCH | 5m | short | 68896 / 69421 / 66856.7 | open |
| 2026-11-13 04:07Z | BTC | plan:null | 5m | short | 68896 / 69421 / 66856.7 | open |
| 2026-11-13 04:07Z | ETH | plan:conditional | 5m | short | 1944.86 / 1963.84 / 1877.8 | pending |
| 2026-11-13 04:07Z | SOL | plan:conditional | 5m | short | 78.62 / 79.48 / 75.88 | pending |
| 2026-11-13 03:57Z | BTC | plan:ready | 3m | short | 68896 / 69421 / 67163.6 | open |
| 2026-11-13 03:57Z | BTC | GOOD | 3m | short | 68896 / 69421 / 67163.6 | open |
| 2026-11-13 03:57Z | SOL | plan:conditional | 3m | short | 78.62 / 79.48 / 76.31 | pending |
| 2026-11-13 03:47Z | ETH | WATCH | 3m | short | 1948.67 / 1963.84 / 1889.8104 | open |
| 2026-11-13 02:37Z | BTC | plan:conditional | 3m | short | 70437.3 / 70733.14 / 69603.6 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 720 | 209 | 135 | 74 | 3 | 64.6% | −0.05R | −0.38R | 0.51 | 6 | 29 |
| WATCH | 501 | 224 | 56 | 165 | 4 | 25.3% | −0.01R | −5.78R | 2.41 | 15 | 30 |
| GOOD | 11 | 11 | 3 | 7 | 1 | 30% | +0.19R | −0.10R | 2.16 | 6 | 50 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 485 | 214 | 54 | 158 | 3 | 25.5% | −0.01R | −6.01R | – | 15 | 28 |
| rr_below_min | 338 | 209 | 135 | 74 | 3 | 64.6% | −0.05R | −0.38R | 0.51 | 6 | 29 |
| chase | 216 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 166 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 16 | 10 | 2 | 7 | 1 | 22.2% | −0.08R | −0.33R | 2.41 | 3 | 59 |
| ready_flag_plan | 11 | 11 | 3 | 7 | 1 | 30% | +0.19R | −0.10R | 2.16 | 6 | 50 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 7 | 7 | 3 | 4 | 0 | 42.9% | +0.70R | +0.42R | 2.05 | 3 | 50 |
| BTC | 2 | 2 | 0 | 1 | 1 | 0% | −1.00R | −1.30R | 2.36 | 1 | – |
| SOL | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.31R | 2.34 | 2 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3268 | 959 | 689 | 267 | 3 | 72.1% | −0.02R | −0.35R | 0.42 | 6 | 22 |
| WATCH | 2155 | 960 | 270 | 682 | 4 | 28.4% | +0.13R | −2.80R | 2.43 | 23 | 40 |
| GOOD | 22 | 22 | 3 | 17 | 1 | 15% | −0.40R | −0.69R | 2.42 | 10 | 50 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2129 | 943 | 268 | 669 | 3 | 28.6% | +0.14R | −2.84R | – | 23 | 40 |
| rr_below_min | 1467 | 959 | 689 | 267 | 3 | 72.1% | −0.02R | −0.35R | 0.42 | 6 | 22 |
| chase | 984 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 815 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 26 | 17 | 2 | 13 | 1 | 13.3% | −0.45R | −0.71R | 2.43 | 8 | 59 |
| ready_flag_plan | 22 | 22 | 3 | 17 | 1 | 15% | −0.40R | −0.69R | 2.42 | 10 | 50 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 11 | 11 | 3 | 8 | 0 | 27.3% | +0.08R | −0.20R | 2.13 | 4 | 50 |
| SOL | 8 | 8 | 0 | 7 | 0 | 0% | −1.00R | −1.31R | 2.62 | 7 | – |
| BTC | 3 | 3 | 0 | 2 | 1 | 0% | −1.00R | −1.23R | 2.93 | 2 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-13 | 76 | 4 | 31 | 41 | 4 | 4 | 2 | 1 | +1.79R |
| 2026-11-12 | 138 | 1 | 53 | 84 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-11-11 | 154 | 0 | 62 | 92 | 0 | 0 | 0 | 0 | – |
| 2026-11-10 | 186 | 2 | 76 | 108 | 2 | 2 | 0 | 2 | −1.00R |
| 2026-11-09 | 195 | 4 | 81 | 110 | 4 | 4 | 1 | 3 | −0.12R |
| 2026-11-08 | 179 | 0 | 78 | 101 | 0 | 0 | 0 | 0 | – |
| 2026-11-07 | 198 | 0 | 76 | 122 | 0 | 0 | 0 | 0 | – |
| 2026-11-06 | 163 | 1 | 66 | 96 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-11-05 | 197 | 3 | 84 | 110 | 3 | 3 | 0 | 2 | −1.00R |
| 2026-11-04 | 189 | 0 | 72 | 117 | 0 | 0 | 0 | 0 | – |
| 2026-11-03 | 198 | 0 | 76 | 122 | 0 | 0 | 0 | 0 | – |
| 2026-11-02 | 165 | 0 | 67 | 98 | 0 | 0 | 0 | 0 | – |
| 2026-11-01 | 172 | 0 | 72 | 100 | 0 | 0 | 0 | 0 | – |
| 2026-10-31 | 178 | 0 | 75 | 103 | 0 | 0 | 0 | 0 | – |
| 2026-10-30 | 170 | 4 | 73 | 93 | 4 | 4 | 0 | 4 | −1.00R |
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
| Live | 40 | 0.8 | 40 | 26.3% | +0.09R | −1.69R |
| NF | 23 | 0.46 | 23 | 19.1% | −0.25R | −0.54R |

n=40 over 49.81 d (engine 0, backfill 40). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 22044, gaps 48, DATA_UNAVAILABLE 6, mark drift |bps| median 2.7 / max 153.3, missing 1m candles 0.
