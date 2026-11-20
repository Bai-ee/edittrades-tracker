# EditTrades call tracker report

Generated 2026-11-20 17:18Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 54.3).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 42 | 39 | 11 | 28.2% | −0.13R | −1.21R | −0.48R | 18.44 | 39 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 53.4).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 54.3).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 55.7).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −33.90% | 11 | 54 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 54.8).

| Equity now | Equity at start | Trades | Realized net | Kill/arm |
| --- | --- | --- | --- | --- |
| $0.00 | $523.01 | 0 | – | – |

Daily/weekly drawdown kill switch; Steady profile caps $150 size / 100x / $5 per trade / $25 per day / 1 open position.

## Testing phase

_provisional; not evidence of an edge_

- Status: READY FOR REVIEW
- Phase: Net-floor forward record (2.5R gross, net floor live), start 2026-09-27, ends 2026-10-11
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 14 / 14, plans scored 39 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.73R | 15 | 40% | 17 / 17 | 4 | +3.32R | 2026-11-20 17:17Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 42 | 39 | 28.2% | +0.16R | 11 / 28 | 2 | 1 | 0 | 39 / 0 | 1 | 41 | – | WORKING |
| WATCH | 3962 | 1776 | 27.7% | +0.09R | 492 / 1284 | 3 | 1842 | 341 | 30 / 1746 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 5937 | 1738 | 72.2% | −0.03R | 1255 / 483 | 0 | 881 | 3318 | 1738 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-20 16:17Z | ETH | WATCH | 3m | short | 1637.33 / 1658.74 / 1529.2095 | open |
| 2026-11-20 16:07Z | BTC | plan:conditional | 3m | short | 59440 / 59743.9 / 56983.9 | pending |
| 2026-11-20 16:07Z | ETH | plan:conditional | 3m | short | 1646.99 / 1662.68 / 1545.81 | pending |
| 2026-11-20 16:07Z | ETH | WATCH | 3m | short | 1646.99 / 1662.68 / 1545.81 | open |
| 2026-11-20 16:07Z | ETH | plan:null | 3m | short | 1646.99 / 1662.68 / 1545.81 | open |
| 2026-11-20 15:57Z | ETH | WATCH | 1m | short | 1646.99 / 1662.68 / 1609.8047 | open |
| 2026-11-20 15:47Z | BTC | plan:ready | 3m | short | 60011 / 60379.6 / 57950.4 | open |
| 2026-11-20 15:47Z | BTC | GOOD | 3m | short | 60011 / 60379.6 / 57950.4 | open |
| 2026-11-20 15:47Z | ETH | plan:ready | 3m | short | 1669.43 / 1682.6 / 1578.06 | open |
| 2026-11-20 15:47Z | ETH | GOOD | 3m | short | 1669.43 / 1682.6 / 1578.06 | open |
| 2026-11-20 02:17Z | BTC | plan:conditional | 3m | short | 61353.2 / 61700 / 60034 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 687 | 210 | 124 | 86 | 0 | 59.1% | −0.07R | −0.38R | 0.48 | 7 | 20 |
| WATCH | 492 | 220 | 58 | 159 | 3 | 26.7% | −0.02R | −1.03R | 3.16 | 25 | 30 |
| GOOD | 17 | 17 | 6 | 9 | 2 | 40% | +0.73R | +0.50R | 2.97 | 4 | 244 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 473 | 210 | 55 | 153 | 2 | 26.4% | −0.04R | −1.08R | – | 25 | 28 |
| rr_below_min | 313 | 210 | 124 | 86 | 0 | 59.1% | −0.07R | −0.38R | 0.48 | 7 | 20 |
| room_at_entry | 189 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 185 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 19 | 10 | 3 | 6 | 1 | 33.3% | +0.26R | +0.03R | 3.16 | 5 | 114 |
| ready_flag_plan | 17 | 17 | 6 | 9 | 2 | 40% | +0.73R | +0.50R | 2.97 | 4 | 244 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 8 | 8 | 4 | 4 | 0 | 50% | +1.18R | +0.97R | 2.95 | 2 | 244 |
| BTC | 5 | 5 | 1 | 3 | 1 | 25% | +0.17R | −0.14R | 2.76 | 2 | 62 |
| ETH | 4 | 4 | 1 | 2 | 1 | 33.3% | +0.26R | +0.11R | 3.29 | 2 | 328 |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3161 | 936 | 642 | 292 | 0 | 68.7% | −0.02R | −0.35R | 0.47 | 7 | 23 |
| WATCH | 2149 | 946 | 269 | 669 | 3 | 28.7% | +0.13R | −2.57R | 2.66 | 25 | 35 |
| GOOD | 38 | 38 | 9 | 26 | 2 | 25.7% | +0.08R | −0.17R | 2.66 | 8 | 151 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2101 | 917 | 264 | 647 | 2 | 29% | +0.15R | −2.63R | – | 25 | 34 |
| rr_below_min | 1439 | 936 | 642 | 292 | 0 | 68.7% | −0.02R | −0.35R | 0.47 | 7 | 23 |
| chase | 925 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 795 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 48 | 29 | 5 | 22 | 1 | 18.5% | −0.27R | −0.53R | 2.66 | 8 | 80 |
| ready_flag_plan | 38 | 38 | 9 | 26 | 2 | 25.7% | +0.08R | −0.17R | 2.66 | 8 | 151 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 16 | 16 | 4 | 11 | 0 | 26.7% | +0.16R | −0.09R | 2.76 | 7 | 244 |
| ETH | 14 | 14 | 4 | 9 | 1 | 30.8% | +0.21R | −0.04R | 2.46 | 3 | 72 |
| BTC | 8 | 8 | 1 | 6 | 1 | 14.3% | −0.33R | −0.60R | 2.82 | 4 | 62 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-20 | 106 | 3 | 51 | 52 | 3 | 3 | 0 | 1 | −1.00R |
| 2026-11-19 | 191 | 0 | 73 | 118 | 0 | 0 | 0 | 0 | – |
| 2026-11-18 | 151 | 2 | 64 | 85 | 2 | 2 | 0 | 2 | −1.00R |
| 2026-11-17 | 170 | 0 | 67 | 103 | 0 | 0 | 0 | 0 | – |
| 2026-11-16 | 162 | 0 | 61 | 101 | 0 | 0 | 0 | 0 | – |
| 2026-11-15 | 169 | 3 | 70 | 96 | 4 | 4 | 1 | 3 | −0.13R |
| 2026-11-14 | 195 | 9 | 84 | 102 | 10 | 10 | 6 | 4 | +1.62R |
| 2026-11-13 | 197 | 5 | 85 | 107 | 5 | 5 | 2 | 3 | +0.68R |
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
| Live | 58 | 1.01 | 58 | 29.1% | +0.23R | −1.07R |
| NF | 40 | 0.7 | 40 | 24.3% | +0.03R | −0.23R |

n=58 over 57.22 d (engine 0, backfill 58). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 25308, gaps 48, DATA_UNAVAILABLE 6, mark drift |bps| median 3 / max 153.3, missing 1m candles 0.
