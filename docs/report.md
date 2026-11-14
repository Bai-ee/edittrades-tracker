# EditTrades call tracker report

Generated 2026-11-14 20:48Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 48.5).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 32 | 30 | 7 | 23.3% | −0.34R | −1.27R | −0.75R | 18.44 | 30 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 47.5).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 48.5).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 49.9).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −28.02% | 11 | 48 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 48.9).

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
- Progress: day 14 / 14, plans scored 30 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.20R | 18 | 27.8% | 19 / 19 | 6 | +3.32R | 2026-11-14 20:47Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 32 | 30 | 23.3% | −0.03R | 7 / 23 | 1 | 1 | 0 | 30 / 0 | 1 | 31 | – | NOT WORKING YET |
| WATCH | 3568 | 1601 | 27.8% | +0.10R | 445 / 1156 | 6 | 1656 | 305 | 23 / 1578 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 5374 | 1579 | 73.3% | −0.02R | 1157 / 422 | 2 | 799 | 2994 | 1579 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-14 20:47Z | ETH | WATCH | 3m | short | 1817.24 / 1825.39 / 1793.0345 | pending |
| 2026-11-14 20:47Z | SOL | WATCH | 3m | short | 71.37 / 71.84 / 70.1292 | pending |
| 2026-11-14 20:37Z | ETH | plan:conditional | 3m | short | 1822.11 / 1829.76 / 1800.3 | pending |
| 2026-11-14 20:37Z | ETH | WATCH | 3m | short | 1822.11 / 1829.76 / 1800.3 | open |
| 2026-11-14 20:37Z | ETH | plan:null | 3m | short | 1822.11 / 1829.76 / 1800.3 | open |
| 2026-11-14 20:37Z | SOL | BAD | 3m | short | 71.57 / 72.06 / 70.55 | open |
| 2026-11-14 20:27Z | ETH | WATCH | 3m | short | 1818.69 / 1826.67 / 1796.9046 | open |
| 2026-11-14 19:27Z | ETH | plan:conditional | 3m | short | 1826.08 / 1834.64 / 1804.58 | pending |
| 2026-11-14 19:07Z | SOL | BAD | 5m | short | 72.25 / 72.8 / 71.04 | open |
| 2026-11-14 18:57Z | SOL | plan:conditional | 3m | short | 72.34 / 72.8 / 71 | pending |
| 2026-11-14 18:57Z | SOL | WATCH | 3m | short | 72.34 / 72.8 / 71 | open |
| 2026-11-14 18:57Z | SOL | plan:null | 3m | short | 72.34 / 72.8 / 71 | open |
| 2026-11-14 16:17Z | SOL | plan:conditional | 5m | short | 73.34 / 74.1 / 70.93 | pending |
| 2026-11-14 15:57Z | SOL | WATCH | 5m | short | 73.34 / 74.1 / 70.9308 | open |
| 2026-11-14 15:37Z | ETH | plan:ready | 5m | short | 1838.07 / 1862.07 / 1773.1 | open |
| 2026-11-14 15:27Z | ETH | plan:ready | 5m | short | 1838.78 / 1862.07 / 1773.81 | open |
| 2026-11-14 15:27Z | ETH | GOOD | 5m | short | 1838.78 / 1862.07 / 1773.81 | open |
| 2026-11-14 15:27Z | ETH | plan:null | 3m | short | 1838.78 / 1862.07 / 1780.52 | open |
| 2026-11-14 15:20Z | ETH | plan:conditional | 5m | short | 1838.78 / 1862.07 / 1773.81 | open |
| 2026-11-14 03:37Z | ETH | plan:conditional | 3m | short | 1899.23 / 1916.13 / 1846.28 | pending |
| 2026-11-14 03:37Z | SOL | plan:conditional | 3m | short | 75.43 / 76.27 / 73.29 | pending |
| 2026-11-14 02:07Z | SOL | plan:conditional | 5m | short | 77.21 / 77.53 / 75.84 | pending |
| 2026-11-14 01:57Z | SOL | plan:conditional | 3m | short | 77.16 / 77.48 / 76.14 | pending |
| 2026-11-13 22:17Z | SOL | plan:conditional | 1m | short | 78.08 / 78.41 / 77.26 | pending |
| 2026-11-13 21:57Z | SOL | plan:conditional | 5m | short | 79.04 / 79.5 / 77.51 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 717 | 239 | 139 | 98 | 2 | 58.7% | −0.04R | −0.37R | 0.58 | 6 | 31 |
| WATCH | 525 | 243 | 65 | 174 | 6 | 27.2% | +0.07R | −4.64R | 2.26 | 15 | 27 |
| GOOD | 19 | 19 | 5 | 13 | 1 | 27.8% | +0.20R | −0.07R | 2.36 | 6 | 94 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 495 | 227 | 62 | 163 | 4 | 27.6% | +0.09R | −4.90R | – | 15 | 25 |
| rr_below_min | 367 | 239 | 139 | 98 | 2 | 58.7% | −0.04R | −0.37R | 0.58 | 6 | 31 |
| chase | 204 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 146 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 30 | 16 | 3 | 11 | 2 | 21.4% | −0.15R | −0.41R | 2.26 | 7 | 80 |
| ready_flag_plan | 19 | 19 | 5 | 13 | 1 | 27.8% | +0.20R | −0.07R | 2.36 | 6 | 94 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 8 | 8 | 3 | 4 | 1 | 42.9% | +0.70R | +0.42R | 2.09 | 3 | 50 |
| SOL | 8 | 8 | 2 | 6 | 0 | 25% | +0.21R | −0.04R | 2.56 | 3 | 490 |
| BTC | 3 | 3 | 0 | 3 | 0 | 0% | −1.00R | −1.27R | 2.54 | 3 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3274 | 964 | 690 | 269 | 2 | 72% | −0.01R | −0.34R | 0.45 | 6 | 23 |
| WATCH | 2176 | 971 | 274 | 688 | 6 | 28.5% | +0.14R | −2.77R | 2.32 | 23 | 37 |
| GOOD | 28 | 28 | 5 | 21 | 1 | 19.2% | −0.17R | −0.44R | 2.49 | 8 | 94 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2136 | 948 | 271 | 671 | 4 | 28.8% | +0.15R | −2.81R | – | 23 | 36 |
| rr_below_min | 1468 | 964 | 690 | 269 | 2 | 72% | −0.01R | −0.34R | 0.45 | 6 | 23 |
| chase | 989 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 815 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 40 | 23 | 3 | 17 | 2 | 15% | −0.41R | −0.67R | 2.32 | 8 | 80 |
| ready_flag_plan | 28 | 28 | 5 | 21 | 1 | 19.2% | −0.17R | −0.44R | 2.49 | 8 | 94 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 13 | 13 | 2 | 10 | 0 | 16.7% | −0.19R | −0.46R | 2.64 | 7 | 490 |
| ETH | 11 | 11 | 3 | 7 | 1 | 30% | +0.19R | −0.09R | 2.16 | 3 | 50 |
| BTC | 4 | 4 | 0 | 4 | 0 | 0% | −1.00R | −1.24R | 2.92 | 4 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-14 | 177 | 7 | 76 | 94 | 8 | 8 | 2 | 4 | +0.62R |
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
| Live | 48 | 0.93 | 48 | 26.1% | +0.11R | −1.40R |
| NF | 31 | 0.6 | 31 | 20.7% | −0.12R | −0.40R |

n=48 over 51.37 d (engine 0, backfill 48). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 22737, gaps 48, DATA_UNAVAILABLE 6, mark drift |bps| median 2.8 / max 153.3, missing 1m candles 0.
