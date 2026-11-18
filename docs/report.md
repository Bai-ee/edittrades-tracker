# EditTrades call tracker report

Generated 2026-11-18 21:08Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 52.5).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 39 | 37 | 11 | 29.7% | −0.07R | −1.21R | −0.46R | 18.44 | 37 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 51.5).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 52.5).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 53.9).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −31.39% | 11 | 52 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 53).

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
- Progress: day 14 / 14, plans scored 37 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.81R | 19 | 42.1% | 20 / 20 | 3 | +3.29R | 2026-11-18 21:07Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 39 | 37 | 29.7% | +0.22R | 11 / 26 | 1 | 1 | 0 | 37 / 0 | 1 | 38 | – | WORKING |
| WATCH | 3828 | 1727 | 28% | +0.10R | 483 / 1244 | 2 | 1776 | 323 | 28 / 1699 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 5752 | 1692 | 72.6% | −0.02R | 1229 / 463 | 4 | 855 | 3201 | 1692 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-18 21:07Z | SOL | WATCH | 5m | short | 72.69 / 73.2 / 71.3793 | pending |
| 2026-11-18 20:57Z | ETH | WATCH | 1m | long | 1751.68 / 1749.54 / 1758.1 | open |
| 2026-11-18 20:57Z | SOL | BAD | 1m | long | 72.98 / 72.24 / 73.2 | open |
| 2026-11-18 20:47Z | SOL | BAD | 1m | long | 72.98 / 72.24 / 73.2 | open |
| 2026-11-18 20:37Z | BTC | BAD | 5m | short | 62532.4 / 62795.04 / 62212.7 | open |
| 2026-11-18 20:27Z | BTC | BAD | 3m | short | 62532.4 / 62795.04 / 62212.7 | open |
| 2026-11-18 19:47Z | BTC | plan:ready | 5m | short | 62707.6 / 62970.97 / 61948.2 | open |
| 2026-11-18 19:47Z | BTC | GOOD | 5m | short | 62707.6 / 62970.97 / 61948.2 | open |
| 2026-11-18 16:47Z | ETH | plan:conditional | 3m | short | 1742.43 / 1755.31 / 1707.72 | pending |
| 2026-11-18 16:27Z | BTC | plan:conditional | 5m | short | 62906.8 / 63242.6 / 61761.2 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 663 | 221 | 125 | 92 | 4 | 57.6% | −0.03R | −0.34R | 0.59 | 7 | 23 |
| WATCH | 477 | 232 | 67 | 164 | 2 | 29% | +0.08R | −0.88R | 2.51 | 25 | 27 |
| GOOD | 20 | 20 | 8 | 11 | 1 | 42.1% | +0.81R | +0.57R | 2.42 | 3 | 193 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 451 | 218 | 63 | 154 | 2 | 29% | +0.08R | −0.94R | – | 25 | 27 |
| rr_below_min | 330 | 221 | 125 | 92 | 4 | 57.6% | −0.03R | −0.34R | 0.59 | 7 | 23 |
| chase | 178 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 155 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 26 | 14 | 4 | 10 | 0 | 28.6% | +0.15R | −0.08R | 2.51 | 7 | 76 |
| ready_flag_plan | 20 | 20 | 8 | 11 | 1 | 42.1% | +0.81R | +0.57R | 2.42 | 3 | 193 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 8 | 8 | 4 | 4 | 0 | 50% | +1.18R | +0.96R | 2.54 | 2 | 244 |
| BTC | 6 | 6 | 1 | 4 | 1 | 20% | −0.06R | −0.34R | 2.36 | 3 | 62 |
| ETH | 6 | 6 | 3 | 3 | 0 | 50% | +1.03R | +0.82R | 2.33 | 2 | 50 |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3187 | 957 | 664 | 287 | 4 | 69.8% | −0.02R | −0.34R | 0.47 | 7 | 23 |
| WATCH | 2144 | 950 | 275 | 669 | 2 | 29.1% | +0.15R | −2.58R | 2.41 | 25 | 35 |
| GOOD | 35 | 35 | 9 | 24 | 1 | 27.3% | +0.15R | −0.11R | 2.45 | 8 | 151 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2099 | 924 | 270 | 649 | 2 | 29.4% | +0.16R | −2.63R | – | 25 | 34 |
| rr_below_min | 1457 | 957 | 664 | 287 | 4 | 69.8% | −0.02R | −0.34R | 0.47 | 7 | 23 |
| chase | 932 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 796 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 45 | 26 | 5 | 20 | 0 | 20% | −0.21R | −0.47R | 2.41 | 8 | 80 |
| ready_flag_plan | 35 | 35 | 9 | 24 | 1 | 27.3% | +0.15R | −0.11R | 2.45 | 8 | 151 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 15 | 15 | 4 | 10 | 0 | 28.6% | +0.25R | −0.01R | 2.59 | 7 | 244 |
| ETH | 13 | 13 | 4 | 9 | 0 | 30.8% | +0.21R | −0.04R | 2.21 | 3 | 72 |
| BTC | 7 | 7 | 1 | 5 | 1 | 16.7% | −0.22R | −0.48R | 2.6 | 4 | 62 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-18 | 126 | 2 | 54 | 70 | 2 | 2 | 0 | 1 | −1.00R |
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
| Live | 55 | 0.99 | 55 | 30.2% | +0.27R | −1.07R |
| NF | 37 | 0.67 | 37 | 25.7% | +0.09R | −0.17R |

n=55 over 55.38 d (engine 0, backfill 55). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 24498, gaps 48, DATA_UNAVAILABLE 6, mark drift |bps| median 3 / max 153.3, missing 1m candles 0.
