# EditTrades call tracker report

Generated 2026-11-22 06:18Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 55.9).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 53 | 51 | 16 | 31.4% | +0.12R | −1.20R | −0.27R | 18.44 | 51 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 54.9).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 55.9).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 57.3).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −36.34% | 11 | 56 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 56.3).

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
- Progress: day 14 / 14, plans scored 51 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.61R | 16 | 31.3% | 17 / 17 | 4 | +4.17R | 2026-11-22 06:17Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 53 | 51 | 31.4% | +0.39R | 16 / 35 | 1 | 1 | 0 | 51 / 0 | 1 | 52 | – | WORKING |
| WATCH | 4080 | 1841 | 28.1% | +0.11R | 518 / 1323 | 2 | 1890 | 347 | 37 / 1804 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 6091 | 1807 | 71.9% | −0.02R | 1299 / 508 | 0 | 911 | 3373 | 1807 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-22 06:17Z | BTC | WATCH | 1m | long | 59100 / 58947.9 / 59458.956 | pending |
| 2026-11-22 05:57Z | ETH | WATCH | 1m | long | 1655.21 / 1652.4 / 1665.9161 | open |
| 2026-11-22 03:17Z | ETH | plan:ready | 5m | short | 1663.69 / 1670.76 / 1640.58 | open |
| 2026-11-22 03:17Z | ETH | GOOD | 5m | short | 1663.69 / 1670.76 / 1640.58 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 691 | 219 | 136 | 83 | 0 | 62.1% | −0.03R | −0.34R | 0.46 | 9 | 21 |
| WATCH | 490 | 227 | 64 | 162 | 2 | 28.3% | +0.07R | −0.90R | 3.44 | 25 | 37 |
| GOOD | 17 | 17 | 5 | 11 | 1 | 31.3% | +0.61R | +0.37R | 2.66 | 4 | 212 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 475 | 216 | 62 | 153 | 2 | 28.8% | +0.07R | −0.94R | – | 25 | 34 |
| rr_below_min | 328 | 219 | 136 | 83 | 0 | 62.1% | −0.03R | −0.34R | 0.46 | 9 | 21 |
| room_at_entry | 188 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 175 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| ready_flag_plan | 17 | 17 | 5 | 11 | 1 | 31.3% | +0.61R | +0.37R | 2.66 | 4 | 212 |
| entry_condition | 15 | 11 | 2 | 9 | 0 | 18.2% | +0.02R | −0.19R | 3.44 | 7 | 436 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 7 | 7 | 2 | 5 | 0 | 28.6% | +0.47R | +0.20R | 2.42 | 3 | 466 |
| ETH | 7 | 7 | 2 | 4 | 1 | 33.3% | +0.93R | +0.71R | 2.65 | 2 | 522 |
| SOL | 3 | 3 | 1 | 2 | 0 | 33.3% | +0.32R | +0.09R | 3.22 | 1 | 131 |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3144 | 960 | 650 | 308 | 0 | 67.9% | −0.01R | −0.33R | 0.49 | 9 | 24 |
| WATCH | 2163 | 967 | 281 | 680 | 2 | 29.2% | +0.16R | −2.48R | 2.68 | 25 | 32 |
| GOOD | 49 | 49 | 14 | 33 | 1 | 29.8% | +0.35R | +0.10R | 2.55 | 8 | 211 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2106 | 932 | 274 | 653 | 2 | 29.6% | +0.17R | −2.55R | – | 25 | 32 |
| rr_below_min | 1464 | 960 | 650 | 308 | 0 | 67.9% | −0.01R | −0.33R | 0.49 | 9 | 24 |
| chase | 919 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 759 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 57 | 35 | 7 | 27 | 0 | 20.6% | −0.09R | −0.34R | 2.68 | 8 | 114 |
| ready_flag_plan | 49 | 49 | 14 | 33 | 1 | 29.8% | +0.35R | +0.10R | 2.55 | 8 | 211 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 19 | 19 | 6 | 12 | 1 | 33.3% | +0.52R | +0.27R | 2.37 | 3 | 153 |
| SOL | 18 | 18 | 5 | 12 | 0 | 29.4% | +0.26R | +0.01R | 2.7 | 7 | 234 |
| BTC | 12 | 12 | 3 | 9 | 0 | 25% | +0.25R | −0.02R | 2.6 | 4 | 210 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-22 | 52 | 3 | 22 | 27 | 3 | 3 | 0 | 2 | −1.00R |
| 2026-11-21 | 189 | 6 | 75 | 108 | 7 | 7 | 3 | 4 | +0.61R |
| 2026-11-20 | 148 | 5 | 72 | 71 | 5 | 5 | 2 | 3 | +1.91R |
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
| Live | 69 | 1.17 | 69 | 31.3% | +0.39R | −0.72R |
| NF | 51 | 0.87 | 51 | 28.6% | +0.31R | +0.05R |

n=69 over 58.76 d (engine 0, backfill 69). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 25989, gaps 48, DATA_UNAVAILABLE 6, mark drift |bps| median 3.1 / max 153.3, missing 1m candles 0.
