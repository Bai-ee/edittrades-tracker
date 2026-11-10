# EditTrades call tracker report

Generated 2026-11-10 02:47Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 43.7).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 17 | 16 | 3 | 18.8% | −0.68R | −1.32R | −1.07R | 14.57 | 16 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 42.8).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 43.7).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 45.1).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −20.38% | 11 | 44 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 44.2).

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
- Progress: day 14 / 14, plans scored 16 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −0.50R | 7 | 14.3% | 8 / 8 | 3 | +2.53R | 2026-11-10 02:47Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 17 | 16 | 18.8% | −0.32R | 3 / 13 | 0 | 1 | 0 | 16 / 0 | 1 | 16 | – | NOT WORKING YET |
| WATCH | 3227 | 1439 | 27.9% | +0.11R | 401 / 1038 | 4 | 1500 | 284 | 14 / 1425 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 4908 | 1414 | 75.3% | −0.02R | 1064 / 350 | 5 | 716 | 2773 | 1414 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-10 02:47Z | SOL | WATCH | 3m | short | 85.78 / 85.92 / 85.0996 | pending |
| 2026-11-10 02:37Z | BTC | BAD | 5m | short | 74834.9 / 75149.21 / 74718.2 | pending |
| 2026-11-10 02:37Z | ETH | BAD | 3m | short | 2117.29 / 2126.18 / 2115.4 | open |
| 2026-11-10 02:37Z | SOL | BAD | 1m | short | 85.81 / 86.17 / 85.62 | open |
| 2026-11-10 01:57Z | BTC | WATCH | 5m | short | 74878.2 / 75152.47 / 74387.2567 | open |
| 2026-11-10 01:57Z | ETH | WATCH | 5m | short | 2121.58 / 2130.04 / 2106.8596 | open |
| 2026-11-10 01:57Z | SOL | WATCH | 5m | short | 86.22 / 86.45 / 85.7002 | open |
| 2026-11-10 00:07Z | BTC | BAD | 5m | long | 75216.45 / 74449.24 / 75402.8 | open |
| 2026-11-10 00:07Z | ETH | BAD | 3m | long | 2130.94 / 2109.2 / 2137.04 | open |
| 2026-11-09 06:57Z | SOL | plan:conditional | 5m | short | 86.05 / 86.41 / 84.59 | pending |
| 2026-11-09 06:47Z | SOL | plan:conditional | 3m | short | 86.02 / 86.38 / 84.95 | pending |
| 2026-11-09 06:27Z | SOL | plan:conditional | 3m | short | 86.39 / 86.75 / 85.47 | pending |
| 2026-11-09 05:17Z | ETH | plan:conditional | 5m | short | 2134.74 / 2143.87 / 2111.61 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 790 | 220 | 148 | 66 | 5 | 69.2% | −0.06R | −0.38R | 0.5 | 6 | 20 |
| WATCH | 538 | 231 | 65 | 159 | 4 | 29% | +0.16R | −5.77R | 2.18 | 10 | 34 |
| GOOD | 8 | 8 | 1 | 6 | 0 | 14.3% | −0.50R | −0.79R | 2.63 | 3 | 94 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 527 | 224 | 64 | 154 | 4 | 29.4% | +0.18R | −5.91R | – | 10 | 34 |
| rr_below_min | 355 | 220 | 148 | 66 | 5 | 69.2% | −0.06R | −0.38R | 0.5 | 6 | 20 |
| chase | 238 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 197 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 11 | 7 | 1 | 5 | 0 | 16.7% | −0.41R | −0.71R | 2.18 | 3 | 80 |
| ready_flag_plan | 8 | 8 | 1 | 6 | 0 | 14.3% | −0.50R | −0.79R | 2.63 | 3 | 94 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 4 | 4 | 0 | 3 | 0 | 0% | −1.00R | −1.31R | 2.8 | 3 | – |
| ETH | 3 | 3 | 1 | 2 | 0 | 33.3% | +0.18R | −0.15R | 1.93 | 2 | 94 |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −1.15R | 4.07 | 1 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3338 | 970 | 711 | 252 | 5 | 73.8% | −0.03R | −0.35R | 0.38 | 6 | 19 |
| WATCH | 2203 | 988 | 284 | 695 | 4 | 29% | +0.18R | −3.55R | 2.3 | 23 | 39 |
| GOOD | 16 | 16 | 2 | 13 | 0 | 13.3% | −0.51R | −0.80R | 2.45 | 10 | 92 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2185 | 976 | 283 | 685 | 4 | 29.2% | +0.19R | −3.58R | – | 23 | 39 |
| rr_below_min | 1474 | 970 | 711 | 252 | 5 | 73.8% | −0.03R | −0.35R | 0.38 | 6 | 19 |
| chase | 1015 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 847 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 18 | 12 | 1 | 10 | 0 | 9.1% | −0.68R | −0.97R | 2.3 | 8 | 80 |
| ready_flag_plan | 16 | 16 | 2 | 13 | 0 | 13.3% | −0.51R | −0.80R | 2.45 | 10 | 92 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 8 | 8 | 1 | 6 | 0 | 14.3% | −0.45R | −0.75R | 2.54 | 6 | 89 |
| ETH | 7 | 7 | 1 | 6 | 0 | 14.3% | −0.50R | −0.80R | 2.13 | 4 | 94 |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −1.15R | 4.07 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-10 | 30 | 0 | 11 | 19 | 0 | 0 | 0 | 0 | – |
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
| Live | 33 | 0.71 | 33 | 25% | +0.03R | −2.02R |
| NF | 16 | 0.34 | 16 | 13.3% | −0.51R | −0.80R |

n=33 over 46.62 d (engine 0, backfill 33). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 20835, gaps 39, DATA_UNAVAILABLE 6, mark drift |bps| median 2.6 / max 153.3, missing 1m candles 0.
