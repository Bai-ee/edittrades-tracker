# EditTrades call tracker report

Generated 2026-11-14 01:37Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 47.7).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 25 | 24 | 5 | 20.8% | −0.52R | −1.29R | −0.91R | 18.44 | 24 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 46.7).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 47.7).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 49.1).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −28.02% | 11 | 48 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 48.1).

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
- Progress: day 14 / 14, plans scored 24 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −0.01R | 12 | 25% | 12 / 12 | 6 | +2.97R | 2026-11-14 01:37Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 25 | 24 | 20.8% | −0.20R | 5 / 19 | 0 | 1 | 0 | 24 / 0 | 1 | 24 | – | NOT WORKING YET |
| WATCH | 3498 | 1565 | 27.7% | +0.10R | 434 / 1131 | 5 | 1626 | 302 | 22 / 1543 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 5289 | 1536 | 74.1% | −0.02R | 1138 / 398 | 10 | 781 | 2962 | 1536 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-14 01:37Z | BTC | WATCH | 1m | long | 68269.2 / 68199 / 68460.846 | pending |
| 2026-11-14 01:37Z | ETH | WATCH | 5m | long | 1932.37 / 1925.04 / 1952.894 | pending |
| 2026-11-14 01:37Z | SOL | WATCH | 3m | short | 77.2 / 77.5 / 75.931 | pending |
| 2026-11-14 01:27Z | BTC | BAD | 1m | long | 68230.7 / 67534.75 / 68354.4 | open |
| 2026-11-14 01:27Z | ETH | BAD | 1m | long | 1928.73 / 1909.06 / 1932.28 | open |
| 2026-11-14 01:27Z | SOL | BAD | 5m | short | 77.54 / 78.07 / 76.45 | pending |
| 2026-11-14 01:17Z | BTC | BAD | 1m | short | 68161 / 68447.28 / 67967.1 | open |
| 2026-11-14 01:17Z | SOL | BAD | 1m | short | 77.3 / 77.62 / 76.51 | open |
| 2026-11-14 01:07Z | ETH | BAD | 1m | short | 1927.64 / 1935.74 / 1920.03 | open |
| 2026-11-14 00:17Z | ETH | BAD | 5m | long | 1928.11 / 1908.44 / 1944.06 | open |
| 2026-11-13 23:07Z | BTC | WATCH | 5m | short | 67944.5 / 68460 / 66892.88 | open |
| 2026-11-13 22:57Z | BTC | BAD | 1m | long | 68367 / 67669.66 / 68460 | open |
| 2026-11-13 22:47Z | BTC | WATCH | 5m | short | 68166.3 / 68460 / 67111.917 | open |
| 2026-11-13 22:37Z | BTC | BAD | 1m | long | 68269.3 / 67572.95 / 68460 | open |
| 2026-11-13 22:17Z | SOL | plan:conditional | 1m | short | 78.08 / 78.41 / 77.26 | pending |
| 2026-11-13 21:57Z | SOL | plan:conditional | 5m | short | 79.04 / 79.5 / 77.51 | pending |
| 2026-11-13 21:47Z | ETH | plan:null | 3m | short | 1927.04 / 1935.13 / 1901.78 | open |
| 2026-11-13 21:37Z | ETH | BAD | 1m | short | 1926.83 / 1934.92 / 1912.7 | open |
| 2026-11-13 15:37Z | ETH | plan:conditional | 1m | short | 1919.88 / 1927.94 / 1894.25 | pending |
| 2026-11-13 15:37Z | SOL | plan:conditional | 1m | short | 79.29 / 79.62 / 78.29 | pending |
| 2026-11-13 15:27Z | ETH | plan:conditional | 3m | short | 1933.05 / 1945.87 / 1894.13 | pending |
| 2026-11-13 05:17Z | BTC | plan:conditional | 5m | short | 68506 / 69069.7 / 66355 | pending |
| 2026-11-13 05:17Z | ETH | plan:conditional | 3m | short | 1923.1 / 1931.18 / 1892.52 | pending |
| 2026-11-13 04:07Z | BTC | plan:conditional | 5m | short | 68896 / 69421 / 66856.7 | pending |
| 2026-11-13 04:07Z | ETH | plan:conditional | 5m | short | 1944.86 / 1963.84 / 1877.8 | pending |
| 2026-11-13 04:07Z | SOL | plan:conditional | 5m | short | 78.62 / 79.48 / 75.88 | pending |
| 2026-11-13 03:57Z | SOL | plan:conditional | 3m | short | 78.62 / 79.48 / 76.31 | pending |
| 2026-11-13 02:37Z | BTC | plan:conditional | 3m | short | 70437.3 / 70733.14 / 69603.6 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 725 | 222 | 136 | 77 | 10 | 63.9% | −0.04R | −0.37R | 0.55 | 6 | 31 |
| WATCH | 514 | 230 | 59 | 169 | 5 | 25.9% | +0.03R | −5.57R | 2.3 | 15 | 29 |
| GOOD | 12 | 12 | 3 | 9 | 0 | 25% | −0.01R | −0.29R | 2.14 | 6 | 50 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 493 | 217 | 57 | 158 | 5 | 26.5% | +0.05R | −5.86R | – | 15 | 28 |
| rr_below_min | 348 | 222 | 136 | 77 | 10 | 63.9% | −0.04R | −0.37R | 0.55 | 6 | 31 |
| chase | 221 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 156 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 21 | 13 | 2 | 11 | 0 | 15.4% | −0.36R | −0.63R | 2.3 | 7 | 59 |
| ready_flag_plan | 12 | 12 | 3 | 9 | 0 | 25% | −0.01R | −0.29R | 2.14 | 6 | 50 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 7 | 7 | 3 | 4 | 0 | 42.9% | +0.70R | +0.42R | 2.05 | 3 | 50 |
| SOL | 3 | 3 | 0 | 3 | 0 | 0% | −1.00R | −1.32R | 2.22 | 3 | – |
| BTC | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.24R | 2.36 | 2 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3273 | 963 | 691 | 260 | 10 | 72.7% | −0.02R | −0.34R | 0.43 | 6 | 22 |
| WATCH | 2165 | 956 | 269 | 680 | 5 | 28.4% | +0.13R | −2.80R | 2.36 | 23 | 38 |
| GOOD | 22 | 22 | 3 | 18 | 0 | 14.3% | −0.43R | −0.71R | 2.4 | 9 | 50 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2134 | 936 | 267 | 663 | 5 | 28.7% | +0.14R | −2.84R | – | 23 | 36 |
| rr_below_min | 1469 | 963 | 691 | 260 | 10 | 72.7% | −0.02R | −0.34R | 0.43 | 6 | 22 |
| chase | 987 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 815 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 31 | 20 | 2 | 17 | 0 | 10.5% | −0.56R | −0.84R | 2.36 | 8 | 59 |
| ready_flag_plan | 22 | 22 | 3 | 18 | 0 | 14.3% | −0.43R | −0.71R | 2.4 | 9 | 50 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 11 | 11 | 3 | 8 | 0 | 27.3% | +0.08R | −0.20R | 2.13 | 4 | 50 |
| SOL | 8 | 8 | 0 | 7 | 0 | 0% | −1.00R | −1.31R | 2.56 | 7 | – |
| BTC | 3 | 3 | 0 | 3 | 0 | 0% | −1.00R | −1.21R | 2.93 | 3 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-14 | 15 | 0 | 6 | 9 | 0 | 0 | 0 | 0 | – |
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
| Live | 41 | 0.81 | 41 | 25% | +0.04R | −1.66R |
| NF | 24 | 0.47 | 24 | 17.4% | −0.31R | −0.60R |

n=41 over 50.57 d (engine 0, backfill 41). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 22380, gaps 48, DATA_UNAVAILABLE 6, mark drift |bps| median 2.8 / max 153.3, missing 1m candles 0.
