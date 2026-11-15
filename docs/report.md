# EditTrades call tracker report

Generated 2026-11-15 00:38Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 48.7).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 34 | 32 | 9 | 28.1% | −0.13R | −1.24R | −0.56R | 18.44 | 32 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 47.7).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 48.7).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 50).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −33.86% | 11 | 49 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 49.1).

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
- Progress: day 14 / 14, plans scored 32 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.50R | 20 | 35% | 21 / 21 | 6 | +3.30R | 2026-11-15 00:37Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 34 | 32 | 28.1% | +0.17R | 9 / 23 | 1 | 1 | 0 | 32 / 0 | 1 | 33 | – | WORKING |
| WATCH | 3578 | 1609 | 28% | +0.11R | 451 / 1158 | 3 | 1659 | 307 | 25 / 1584 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 5385 | 1583 | 73.3% | −0.02R | 1160 / 423 | 3 | 799 | 3000 | 1583 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-15 00:27Z | BTC | BAD | 5m | long | 64466.45 / 63808.89 / 64999.1 | pending |
| 2026-11-15 00:27Z | SOL | WATCH | 1m | short | 70.1 / 70.29 / 69.6592 | pending |
| 2026-11-15 00:17Z | BTC | BAD | 3m | long | 64169.3 / 63514.77 / 64999.1 | open |
| 2026-11-14 22:17Z | BTC | BAD | 5m | short | 64125.2 / 64999.1 / 62152.7 | open |
| 2026-11-14 22:17Z | ETH | plan:conditional | 5m | short | 1760.79 / 1793.42 / 1672.01 | pending |
| 2026-11-14 22:17Z | ETH | WATCH | 5m | short | 1760.79 / 1793.42 / 1672.01 | open |
| 2026-11-14 22:17Z | ETH | plan:null | 5m | short | 1760.79 / 1793.42 / 1672.01 | open |
| 2026-11-14 21:27Z | SOL | plan:ready | 5m | short | 70.09 / 70.84 / 67.64 | open |
| 2026-11-14 21:27Z | SOL | GOOD | 5m | short | 70.09 / 70.84 / 67.64 | open |
| 2026-11-14 21:17Z | SOL | WATCH | 5m | short | 70.09 / 70.84 / 67.6375 | open |
| 2026-11-14 20:37Z | ETH | plan:conditional | 3m | short | 1822.11 / 1829.76 / 1800.3 | pending |
| 2026-11-14 19:27Z | ETH | plan:conditional | 3m | short | 1826.08 / 1834.64 / 1804.58 | pending |
| 2026-11-14 18:57Z | SOL | plan:conditional | 3m | short | 72.34 / 72.8 / 71 | pending |
| 2026-11-14 16:17Z | SOL | plan:conditional | 5m | short | 73.34 / 74.1 / 70.93 | pending |
| 2026-11-14 03:37Z | ETH | plan:conditional | 3m | short | 1899.23 / 1916.13 / 1846.28 | pending |
| 2026-11-14 03:37Z | SOL | plan:conditional | 3m | short | 75.43 / 76.27 / 73.29 | pending |
| 2026-11-14 02:07Z | SOL | plan:conditional | 5m | short | 77.21 / 77.53 / 75.84 | pending |
| 2026-11-14 01:57Z | SOL | plan:conditional | 3m | short | 77.16 / 77.48 / 76.14 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 706 | 237 | 139 | 96 | 3 | 59.2% | −0.02R | −0.34R | 0.58 | 6 | 31 |
| WATCH | 519 | 238 | 68 | 168 | 3 | 28.8% | +0.13R | −4.51R | 2.27 | 15 | 27 |
| GOOD | 21 | 21 | 7 | 13 | 1 | 35% | +0.50R | +0.24R | 2.39 | 6 | 94 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 488 | 221 | 63 | 157 | 2 | 28.6% | +0.12R | −4.84R | – | 15 | 24 |
| rr_below_min | 362 | 237 | 139 | 96 | 3 | 59.2% | −0.02R | −0.34R | 0.58 | 6 | 31 |
| chase | 201 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 143 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 31 | 17 | 5 | 11 | 1 | 31.3% | +0.23R | −0.03R | 2.27 | 7 | 80 |
| ready_flag_plan | 21 | 21 | 7 | 13 | 1 | 35% | +0.50R | +0.24R | 2.39 | 6 | 94 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 9 | 9 | 2 | 6 | 1 | 25% | +0.21R | −0.04R | 2.58 | 3 | 490 |
| ETH | 8 | 8 | 4 | 4 | 0 | 50% | +0.96R | +0.70R | 2.09 | 3 | 72 |
| BTC | 4 | 4 | 1 | 3 | 0 | 25% | +0.17R | −0.11R | 2.55 | 3 | 62 |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3270 | 967 | 692 | 270 | 3 | 71.9% | −0.01R | −0.33R | 0.45 | 6 | 23 |
| WATCH | 2176 | 974 | 280 | 687 | 3 | 29% | +0.15R | −2.72R | 2.33 | 23 | 36 |
| GOOD | 30 | 30 | 7 | 21 | 1 | 25% | +0.07R | −0.19R | 2.5 | 8 | 94 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2135 | 950 | 275 | 670 | 2 | 29.1% | +0.16R | −2.77R | – | 23 | 36 |
| rr_below_min | 1471 | 967 | 692 | 270 | 3 | 71.9% | −0.01R | −0.33R | 0.45 | 6 | 23 |
| chase | 990 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 807 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 41 | 24 | 5 | 17 | 1 | 22.7% | −0.11R | −0.37R | 2.33 | 8 | 80 |
| ready_flag_plan | 30 | 30 | 7 | 21 | 1 | 25% | +0.07R | −0.19R | 2.5 | 8 | 94 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 14 | 14 | 2 | 10 | 1 | 16.7% | −0.19R | −0.46R | 2.65 | 7 | 490 |
| ETH | 11 | 11 | 4 | 7 | 0 | 36.4% | +0.43R | +0.16R | 2.16 | 3 | 72 |
| BTC | 5 | 5 | 1 | 4 | 0 | 20% | −0.06R | −0.32R | 2.86 | 4 | 62 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-15 | 5 | 0 | 2 | 3 | 0 | 0 | 0 | 0 | – |
| 2026-11-14 | 195 | 9 | 84 | 102 | 10 | 10 | 5 | 4 | +1.43R |
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
| Live | 50 | 0.97 | 50 | 29.2% | +0.24R | −1.21R |
| NF | 33 | 0.64 | 33 | 25.8% | +0.10R | −0.18R |

n=50 over 51.53 d (engine 0, backfill 50). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 22809, gaps 48, DATA_UNAVAILABLE 6, mark drift |bps| median 2.8 / max 153.3, missing 1m candles 0.
