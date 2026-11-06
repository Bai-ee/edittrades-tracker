# EditTrades call tracker report

Generated 2026-11-06 05:57Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 39.9).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 13 | 11 | 2 | 18.2% | −0.70R | −1.31R | −1.24R | 11.49 | 11 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 38.9).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 39.9).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 41.2).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −9.11% | −18.07% | 11 | 40 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 40.3).

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
- Progress: day 14 / 14, plans scored 11 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| −1.00R | 5 | 0% | 7 / 7 | 5 | – | 2026-11-06 05:57Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 13 | 11 | 18.2% | −0.33R | 2 / 9 | 2 | 0 | 0 | 11 / 0 | 1 | 12 | – | NOT WORKING YET |
| WATCH | 2933 | 1316 | 28.3% | +0.12R | 372 / 944 | 5 | 1345 | 267 | 9 / 1307 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 4490 | 1297 | 75.9% | −0.02R | 985 / 312 | 4 | 645 | 2544 | 1297 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-11-06 05:37Z | BTC | WATCH | 1m | long | 75583.9 / 75449.4 / 75800.445 | open |
| 2026-11-06 05:27Z | ETH | BAD | 5m | short | 2223.35 / 2233.37 / 2205.41 | open |
| 2026-11-06 05:17Z | BTC | BAD | 5m | short | 75583.9 / 75901.35 / 74957.2 | open |
| 2026-11-06 05:17Z | SOL | plan:ready | 5m | short | 89.2 / 89.57 / 88.01 | open |
| 2026-11-06 05:17Z | SOL | GOOD | 5m | short | 89.2 / 89.57 / 88.01 | open |
| 2026-11-05 22:07Z | ETH | plan:conditional | 5m | short | 2229.1 / 2241.53 / 2179.94 | pending |
| 2026-11-05 17:47Z | SOL | plan:conditional | 3m | short | 89.52 / 89.91 / 88.01 | pending |
| 2026-11-05 16:07Z | SOL | BAD | 5m | short | 90.39 / 91.54 / 88.01 | open |
| 2026-11-05 15:57Z | SOL | plan:ready | 3m | short | 90.39 / 91.54 / 85.04 | open |
| 2026-11-05 15:57Z | SOL | GOOD | 3m | short | 90.39 / 91.54 / 85.04 | open |
| 2026-11-05 15:47Z | BTC | plan:conditional | 1m | short | 76173.4 / 76596.2 / 74680 | pending |
| 2026-11-05 15:47Z | ETH | WATCH | 3m | short | 2256.13 / 2286.06 / 2131.3219 | open |
| 2026-11-05 15:37Z | BTC | WATCH | 3m | short | 76537.6 / 77577.8 / 73745.7 | open |
| 2026-11-05 15:37Z | BTC | plan:null | 3m | short | 76537.6 / 77577.8 / 73745.7 | open |
| 2026-11-05 15:37Z | SOL | WATCH | 3m | short | 90.55 / 92.2 / 85.4515 | open |
| 2026-11-05 15:27Z | SOL | BAD | 1m | short | 90.55 / 91.97 / 87.67 | open |
| 2026-11-05 15:17Z | ETH | WATCH | 1m | short | 2268.04 / 2307.45 / 2184.8849 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 749 | 228 | 171 | 53 | 4 | 76.3% | +0.06R | −0.27R | 0.48 | 4 | 29 |
| WATCH | 519 | 229 | 69 | 154 | 5 | 30.9% | +0.27R | −2.05R | 2.36 | 11 | 34 |
| GOOD | 7 | 7 | 0 | 5 | 2 | 0% | −1.00R | −1.27R | 2.85 | 5 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 512 | 224 | 69 | 150 | 4 | 31.5% | +0.30R | −2.06R | – | 11 | 34 |
| rr_below_min | 354 | 228 | 171 | 53 | 4 | 76.3% | +0.06R | −0.27R | 0.48 | 4 | 29 |
| chase | 226 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 169 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 7 | 5 | 0 | 4 | 1 | 0% | −1.00R | −1.28R | 2.36 | 4 | – |
| ready_flag_plan | 7 | 7 | 0 | 5 | 2 | 0% | −1.00R | −1.27R | 2.85 | 5 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 4 | 4 | 0 | 2 | 2 | 0% | −1.00R | −1.26R | 3 | 2 | – |
| ETH | 2 | 2 | 0 | 2 | 0 | 0% | −1.00R | −1.33R | 1.93 | 2 | – |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −1.15R | 4.07 | 1 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 3310 | 999 | 749 | 245 | 4 | 75.4% | −0.00R | −0.33R | 0.37 | 6 | 21 |
| WATCH | 2189 | 983 | 288 | 686 | 5 | 29.6% | +0.20R | −2.86R | 2.28 | 23 | 39 |
| GOOD | 12 | 12 | 1 | 9 | 2 | 10% | −0.61R | −0.90R | 2.61 | 9 | 89 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 2174 | 972 | 286 | 679 | 4 | 29.6% | +0.20R | −2.88R | – | 23 | 39 |
| rr_below_min | 1504 | 999 | 749 | 245 | 4 | 75.4% | −0.00R | −0.33R | 0.37 | 6 | 21 |
| chase | 993 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 811 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 15 | 11 | 2 | 7 | 1 | 22.2% | −0.12R | −0.41R | 2.28 | 6 | 57 |
| ready_flag_plan | 12 | 12 | 1 | 9 | 2 | 10% | −0.61R | −0.90R | 2.61 | 9 | 89 |
| invalid_levels | 2 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 7 | 7 | 1 | 4 | 2 | 20% | −0.23R | −0.53R | 2.6 | 4 | 89 |
| ETH | 4 | 4 | 0 | 4 | 0 | 0% | −1.00R | −1.29R | 2.28 | 4 | – |
| BTC | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −1.15R | 4.07 | 1 | – |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-11-06 | 49 | 1 | 18 | 30 | 1 | 1 | 0 | 0 | – |
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
| Live | 29 | 0.68 | 29 | 25.9% | +0.10R | −2.29R |
| NF | 12 | 0.28 | 12 | 10% | −0.61R | −0.90R |

n=29 over 42.75 d (engine 0, backfill 29). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 19143, gaps 36, DATA_UNAVAILABLE 6, mark drift |bps| median 2.5 / max 153.3, missing 1m candles 0.
