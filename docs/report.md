# EditTrades call tracker report

Generated 2026-11-21 03:28Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 54.8).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 44 | 43 | 13 | 30.2% | +0.11R | −1.20R | −0.31R | 18.44 | 43 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 53.8).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 54.8).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 56.1).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −38.03% | 11 | 55 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 55.2).

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
- Progress: day 14 / 14, plans scored 43 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +1.13R | 19 | 42.1% | 19 / 19 | 4 | +4.06R | 2026-11-21 03:27Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 44 | 43 | 30.2% | +0.39R | 13 / 30 | 0 | 1 | 0 | 43 / 0 | 1 | 43 | – | WORKING |
| WATCH | 3995 | 1790 | 27.7% | +0.09R | 496 / 1294 | 8 | 1855 | 342 | 33 / 1757 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 5973 | 1754 | 72.2% | −0.02R | 1266 / 488 | 2 | 886 | 3331 | 1754 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-21 03:27Z | BTC | WATCH | 5m | short | 58106.8 / 58396.9 / 57187.183 | pending |
| 2026-11-21 03:27Z | ETH | WATCH | 5m | short | 1604.33 / 1615.79 / 1578.7742 | pending |
| 2026-11-21 03:27Z | SOL | WATCH | 3m | short | 67.65 / 68.21 / 66.4516 | pending |
| 2026-11-21 03:17Z | BTC | plan:conditional | 5m | short | 58487.2 / 58732.85 / 57868 | pending |
| 2026-11-21 03:17Z | BTC | WATCH | 5m | short | 58487.2 / 58732.85 / 57868 | pending |
| 2026-11-21 03:17Z | BTC | plan:null | 5m | short | 58487.2 / 58732.85 / 57868 | pending |
| 2026-11-21 03:17Z | ETH | BAD | 5m | short | 1613.59 / 1622.13 / 1601.28 | pending |
| 2026-11-21 03:17Z | SOL | BAD | 5m | short | 68.36 / 68.66 / 67.63 | pending |
| 2026-11-21 03:07Z | ETH | WATCH | 3m | short | 1613.59 / 1620.41 / 1601.4504 | open |
| 2026-11-20 20:57Z | SOL | plan:conditional | 1m | short | 67.31 / 67.74 / 66.06 | pending |
| 2026-11-20 19:07Z | ETH | plan:conditional | 3m | short | 1614.48 / 1628.34 / 1579.58 | pending |
| 2026-11-20 18:17Z | BTC | plan:conditional | 3m | short | 58879.6 / 59126.89 / 58093.7 | pending |
| 2026-11-20 17:57Z | BTC | WATCH | 5m | short | 58814.1 / 59506.8 / 56659.803 | open |
| 2026-11-20 17:47Z | ETH | plan:conditional | 3m | short | 1625.08 / 1638.79 / 1590.71 | pending |
| 2026-11-20 16:17Z | ETH | WATCH | 3m | short | 1637.33 / 1658.74 / 1529.2095 | open |
| 2026-11-20 16:07Z | BTC | plan:conditional | 3m | short | 59440 / 59743.9 / 56983.9 | pending |
| 2026-11-20 16:07Z | ETH | plan:conditional | 3m | short | 1646.99 / 1662.68 / 1545.81 | pending |
| 2026-11-20 16:07Z | ETH | WATCH | 3m | short | 1646.99 / 1662.68 / 1545.81 | open |
| 2026-11-20 16:07Z | ETH | plan:null | 3m | short | 1646.99 / 1662.68 / 1545.81 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 676 | 207 | 123 | 84 | 2 | 59.4% | −0.04R | −0.35R | 0.52 | 7 | 18 |
| WATCH | 490 | 221 | 56 | 161 | 8 | 25.8% | −0.07R | −1.04R | 3.03 | 25 | 30 |
| GOOD | 19 | 19 | 8 | 11 | 0 | 42.1% | +1.13R | +0.91R | 2.9 | 4 | 223 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 470 | 209 | 53 | 153 | 6 | 25.7% | −0.07R | −1.08R | – | 25 | 28 |
| rr_below_min | 310 | 207 | 123 | 84 | 2 | 59.4% | −0.04R | −0.35R | 0.52 | 7 | 18 |
| room_at_entry | 188 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 178 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 20 | 12 | 3 | 8 | 2 | 27.3% | +0.03R | −0.20R | 3.03 | 8 | 114 |
| ready_flag_plan | 19 | 19 | 8 | 11 | 0 | 42.1% | +1.13R | +0.91R | 2.9 | 4 | 223 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 8 | 8 | 4 | 4 | 0 | 50% | +1.18R | +0.97R | 2.95 | 2 | 244 |
| BTC | 7 | 7 | 2 | 5 | 0 | 28.6% | +0.61R | +0.34R | 2.63 | 2 | 136 |
| ETH | 4 | 4 | 2 | 2 | 0 | 50% | +1.93R | +1.77R | 3.29 | 2 | 270 |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3153 | 939 | 643 | 294 | 2 | 68.6% | −0.02R | −0.34R | 0.49 | 7 | 23 |
| WATCH | 2157 | 950 | 268 | 673 | 8 | 28.5% | +0.12R | −2.58R | 2.61 | 25 | 33 |
| GOOD | 40 | 40 | 11 | 28 | 0 | 28.2% | +0.34R | +0.09R | 2.64 | 8 | 210 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2104 | 918 | 263 | 648 | 6 | 28.9% | +0.13R | −2.65R | – | 25 | 33 |
| rr_below_min | 1437 | 939 | 643 | 294 | 2 | 68.6% | −0.02R | −0.34R | 0.49 | 7 | 23 |
| chase | 922 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 792 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 53 | 32 | 5 | 25 | 2 | 16.7% | −0.35R | −0.60R | 2.61 | 8 | 80 |
| ready_flag_plan | 40 | 40 | 11 | 28 | 0 | 28.2% | +0.34R | +0.09R | 2.64 | 8 | 210 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 16 | 16 | 4 | 11 | 0 | 26.7% | +0.16R | −0.09R | 2.76 | 7 | 244 |
| ETH | 14 | 14 | 5 | 9 | 0 | 35.7% | +0.69R | +0.44R | 2.46 | 3 | 94 |
| BTC | 10 | 10 | 2 | 8 | 0 | 20% | +0.13R | −0.13R | 2.72 | 4 | 136 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-21 | 29 | 0 | 12 | 17 | 0 | 0 | 0 | 0 | – |
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
| Live | 60 | 1.04 | 60 | 30.5% | +0.39R | −0.84R |
| NF | 42 | 0.73 | 42 | 26.8% | +0.29R | +0.03R |

n=60 over 57.65 d (engine 0, backfill 60). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 25494, gaps 48, DATA_UNAVAILABLE 6, mark drift |bps| median 3 / max 153.3, missing 1m candles 0.
