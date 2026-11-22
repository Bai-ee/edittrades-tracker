# EditTrades call tracker report

Generated 2026-11-22 02:38Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 55.7).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 50 | 47 | 14 | 29.8% | +0.08R | −1.20R | −0.33R | 18.44 | 47 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 54.8).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 55.7).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 57.1).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −36.34% | 11 | 56 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 56.2).

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
- Progress: day 14 / 14, plans scored 47 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.69R | 13 | 30.8% | 15 / 15 | 4 | +4.49R | 2026-11-22 02:37Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 50 | 47 | 29.8% | +0.35R | 14 / 33 | 2 | 1 | 0 | 47 / 0 | 1 | 49 | – | WORKING |
| WATCH | 4066 | 1832 | 28.1% | +0.10R | 515 / 1317 | 2 | 1886 | 346 | 37 / 1795 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 6073 | 1799 | 72.1% | −0.02R | 1297 / 502 | 6 | 904 | 3364 | 1799 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-22 02:37Z | SOL | WATCH | 1m | short | 69.66 / 69.76 / 69.06 | pending |
| 2026-11-22 02:27Z | ETH | WATCH | 1m | short | 1675.42 / 1678.01 / 1666.0183 | open |
| 2026-11-22 02:27Z | SOL | BAD | 3m | short | 70.12 / 70.41 / 69.99 | pending |
| 2026-11-21 19:57Z | ETH | BAD | 5m | long | 1684.28 / 1667.1 / 1693.95 | open |
| 2026-11-21 17:07Z | BTC | BAD | 3m | long | 60036.4 / 59424.03 / 60503 | open |
| 2026-11-21 17:07Z | ETH | BAD | 3m | long | 1683.91 / 1666.73 / 1695.1 | open |
| 2026-11-21 16:57Z | BTC | BAD | 3m | long | 59991 / 59379.09 / 60643.5 | open |
| 2026-11-21 16:47Z | ETH | BAD | 1m | long | 1681.32 / 1664.17 / 1689.91 | open |
| 2026-11-21 15:27Z | ETH | plan:ready | 3m | short | 1682.42 / 1694.44 / 1650.32 | open |
| 2026-11-21 15:27Z | ETH | GOOD | 3m | short | 1682.42 / 1694.44 / 1650.32 | open |
| 2026-11-21 14:37Z | BTC | plan:ready | 1m | short | 60182 / 60471.7 / 59405.9 | open |
| 2026-11-21 14:37Z | BTC | GOOD | 1m | short | 60182 / 60471.7 / 59405.9 | open |
| 2026-11-21 03:57Z | BTC | plan:conditional | 1m | short | 56638.4 / 56964.1 / 54794.7 | pending |
| 2026-11-21 03:57Z | SOL | plan:conditional | 1m | short | 65.96 / 66.52 / 63.61 | pending |
| 2026-11-21 03:47Z | BTC | plan:conditional | 1m | short | 56798.4 / 57379 / 55166.9 | pending |
| 2026-11-21 03:17Z | BTC | plan:conditional | 5m | short | 58487.2 / 58732.85 / 57868 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 683 | 217 | 135 | 77 | 6 | 63.7% | −0.01R | −0.32R | 0.46 | 7 | 21 |
| WATCH | 485 | 221 | 62 | 158 | 2 | 28.2% | +0.04R | −0.94R | 3.44 | 25 | 34 |
| GOOD | 15 | 15 | 4 | 9 | 2 | 30.8% | +0.69R | +0.46R | 2.71 | 4 | 181 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 470 | 210 | 60 | 149 | 2 | 28.7% | +0.04R | −0.98R | – | 25 | 33 |
| rr_below_min | 322 | 217 | 135 | 77 | 6 | 63.7% | −0.01R | −0.32R | 0.46 | 7 | 21 |
| room_at_entry | 189 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 172 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 15 | 11 | 2 | 9 | 0 | 18.2% | +0.02R | −0.19R | 3.44 | 7 | 436 |
| ready_flag_plan | 15 | 15 | 4 | 9 | 2 | 30.8% | +0.69R | +0.46R | 2.71 | 4 | 181 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BTC | 7 | 7 | 1 | 5 | 1 | 16.7% | +0.10R | −0.17R | 2.42 | 3 | 210 |
| ETH | 4 | 4 | 1 | 2 | 1 | 33.3% | +1.65R | +1.49R | 3.08 | 1 | 212 |
| SOL | 4 | 4 | 2 | 2 | 0 | 50% | +0.86R | +0.62R | 2.86 | 1 | 141 |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3147 | 961 | 651 | 303 | 6 | 68.2% | −0.01R | −0.33R | 0.49 | 7 | 24 |
| WATCH | 2161 | 961 | 279 | 676 | 2 | 29.2% | +0.15R | −2.50R | 2.68 | 25 | 32 |
| GOOD | 46 | 46 | 12 | 31 | 2 | 27.9% | +0.31R | +0.06R | 2.58 | 8 | 181 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2104 | 926 | 272 | 649 | 2 | 29.5% | +0.16R | −2.58R | – | 25 | 32 |
| rr_below_min | 1463 | 961 | 651 | 303 | 6 | 68.2% | −0.01R | −0.33R | 0.49 | 7 | 24 |
| chase | 918 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 764 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 57 | 35 | 7 | 27 | 0 | 20.6% | −0.09R | −0.34R | 2.68 | 8 | 114 |
| ready_flag_plan | 46 | 46 | 12 | 31 | 2 | 27.9% | +0.31R | +0.06R | 2.58 | 8 | 181 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 18 | 18 | 5 | 12 | 0 | 29.4% | +0.26R | +0.01R | 2.7 | 7 | 234 |
| ETH | 16 | 16 | 5 | 10 | 1 | 33.3% | +0.58R | +0.34R | 2.43 | 3 | 94 |
| BTC | 12 | 12 | 2 | 9 | 1 | 18.2% | +0.03R | −0.24R | 2.6 | 4 | 136 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-22 | 17 | 0 | 8 | 9 | 0 | 0 | 0 | 0 | – |
| 2026-11-21 | 189 | 6 | 75 | 108 | 7 | 7 | 1 | 4 | −0.21R |
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
| Live | 66 | 1.13 | 66 | 30.2% | +0.36R | −0.80R |
| NF | 48 | 0.82 | 48 | 26.7% | +0.26R | +0.01R |

n=66 over 58.61 d (engine 0, backfill 66). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 25920, gaps 48, DATA_UNAVAILABLE 6, mark drift |bps| median 3.1 / max 153.3, missing 1m candles 0.
