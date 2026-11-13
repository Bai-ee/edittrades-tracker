# EditTrades call tracker report

Generated 2026-11-13 00:17Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 46.6).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 20 | 19 | 3 | 15.8% | −0.77R | −1.31R | −1.11R | 18.44 | 19 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 45.7).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 46.6).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 48).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −24.71% | 11 | 47 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 47.1).

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
- Progress: day 14 / 14, plans scored 19 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −0.56R | 8 | 12.5% | 8 / 8 | 6 | +2.53R | 2026-11-13 00:17Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 20 | 19 | 15.8% | −0.43R | 3 / 16 | 0 | 1 | 0 | 19 / 0 | 1 | 19 | – | NOT WORKING YET |
| WATCH | 3410 | 1519 | 27.7% | +0.09R | 420 / 1099 | 5 | 1588 | 298 | 14 / 1505 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 5174 | 1496 | 74.6% | −0.02R | 1116 / 380 | 12 | 758 | 2908 | 1496 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-13 00:17Z | ETH | WATCH | 3m | short | 2013 / 2017.19 / 2002.9859 | pending |
| 2026-11-13 00:07Z | BTC | WATCH | 3m | long | 71422.1 / 71322.7 / 71631.834 | pending |
| 2026-11-13 00:07Z | ETH | BAD | 5m | long | 2016.5 / 1995.93 / 2024.91 | pending |
| 2026-11-13 00:07Z | SOL | WATCH | 5m | long | 81.66 / 81.48 / 82.1604 | pending |
| 2026-11-12 23:57Z | BTC | BAD | 1m | long | 71341.5 / 70613.82 / 71680.7 | open |
| 2026-11-12 23:57Z | ETH | BAD | 3m | long | 2016.59 / 1996.02 / 2024.91 | open |
| 2026-11-12 23:57Z | SOL | BAD | 1m | long | 81.64 / 80.81 / 81.83 | open |
| 2026-11-12 23:37Z | SOL | WATCH | 3m | long | 81.64 / 81.45 / 82.1397 | open |
| 2026-11-12 21:27Z | SOL | BAD | 1m | long | 81.46 / 80.63 / 81.9 | open |
| 2026-11-12 20:37Z | BTC | BAD | 5m | short | 71396.1 / 71695.96 / 70745.1 | open |
| 2026-11-12 20:17Z | ETH | BAD | 3m | long | 2016.62 / 1996.05 / 2024.91 | open |
| 2026-11-12 20:07Z | BTC | WATCH | 5m | short | 71462.8 / 71668 / 70812.316 | open |
| 2026-11-12 19:42Z | BTC | BAD | 5m | short | 71506 / 71806.33 / 70946.1 | open |
| 2026-11-12 19:37Z | BTC | BAD | 3m | short | 71506 / 71806.33 / 70946.1 | open |
| 2026-11-12 17:57Z | ETH | BAD | 3m | long | 2012.94 / 1992.41 / 2029.36 | open |
| 2026-11-12 16:17Z | ETH | BAD | 5m | long | 2012.17 / 1991.65 / 2033.49 | open |
| 2026-11-12 13:27Z | ETH | BAD | 5m | short | 2010.92 / 2033.49 / 1971.31 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 711 | 218 | 137 | 70 | 12 | 66.2% | −0.06R | −0.39R | 0.49 | 6 | 27 |
| WATCH | 494 | 209 | 49 | 158 | 5 | 23.7% | −0.08R | −6.24R | 2.06 | 13 | 29 |
| GOOD | 8 | 8 | 1 | 7 | 0 | 12.5% | −0.56R | −0.87R | 2.08 | 6 | 94 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 485 | 204 | 48 | 154 | 5 | 23.8% | −0.08R | −6.38R | – | 13 | 28 |
| rr_below_min | 335 | 218 | 137 | 70 | 12 | 66.2% | −0.06R | −0.39R | 0.49 | 6 | 27 |
| chase | 208 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 168 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 9 | 5 | 1 | 4 | 0 | 20% | −0.29R | −0.60R | 2.06 | 2 | 80 |
| ready_flag_plan | 8 | 8 | 1 | 7 | 0 | 12.5% | −0.56R | −0.87R | 2.08 | 6 | 94 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 4 | 4 | 1 | 3 | 0 | 25% | −0.12R | −0.42R | 1.94 | 3 | 94 |
| SOL | 3 | 3 | 0 | 3 | 0 | 0% | −1.00R | −1.32R | 2.27 | 3 | – |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −1.30R | 2.09 | 1 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3262 | 965 | 692 | 259 | 12 | 72.8% | −0.02R | −0.35R | 0.41 | 6 | 21 |
| WATCH | 2149 | 946 | 264 | 675 | 5 | 28.1% | +0.12R | −2.85R | 2.3 | 23 | 40 |
| GOOD | 18 | 18 | 1 | 16 | 0 | 5.9% | −0.79R | −1.08R | 2.44 | 10 | 94 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2130 | 934 | 263 | 665 | 5 | 28.3% | +0.13R | −2.87R | – | 23 | 39 |
| rr_below_min | 1458 | 965 | 692 | 259 | 12 | 72.8% | −0.02R | −0.35R | 0.41 | 6 | 21 |
| chase | 978 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 824 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 19 | 12 | 1 | 10 | 0 | 9.1% | −0.68R | −0.97R | 2.3 | 8 | 80 |
| ready_flag_plan | 18 | 18 | 1 | 16 | 0 | 5.9% | −0.79R | −1.08R | 2.44 | 10 | 94 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 8 | 8 | 1 | 7 | 0 | 12.5% | −0.56R | −0.85R | 2.11 | 4 | 94 |
| SOL | 8 | 8 | 0 | 7 | 0 | 0% | −1.00R | −1.31R | 2.62 | 7 | – |
| BTC | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.23R | 3.08 | 2 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-13 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |
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
| Live | 36 | 0.73 | 36 | 22.9% | −0.05R | −1.96R |
| NF | 19 | 0.38 | 19 | 11.1% | −0.59R | −0.88R |

n=36 over 49.51 d (engine 0, backfill 36). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 21915, gaps 48, DATA_UNAVAILABLE 6, mark drift |bps| median 2.7 / max 153.3, missing 1m candles 0.
