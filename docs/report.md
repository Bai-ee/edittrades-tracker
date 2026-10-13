# EditTrades call tracker report

Generated 2026-10-13 17:57Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 16.4).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2 | 2 | 2 | 100% | +1.87R | +1.87R | +1.22R | 0 | 2 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 15.4).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 16.4).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 17.7).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −4.01% | −8.55% | 5 | 16 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 16.8).

| Equity now | Equity at start | Trades | Realized net | Kill/arm |
| --- | --- | --- | --- | --- |
| $520.99 | $523.01 | 0 | – | – |

Daily/weekly drawdown kill switch; Steady profile caps $150 size / 100x / $5 per trade / $25 per day / 1 open position.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Net-floor forward record (2.5R gross, net floor live), start 2026-09-27, ends 2026-10-11
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 14 / 14, plans scored 2 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +2.87R | 1 | 100% | 1 / 1 | 0 | +2.87R | 2026-10-13 17:57Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 2 | 2 | 100% | +2.69R | 2 / 0 | 0 | 0 | 0 | 2 / 0 | 1 | 1 | – | [2 SCORED · TOO FEW TO JUDGE] |
| WATCH | 1238 | 567 | 27.3% | +0.07R | 155 / 412 | 4 | 539 | 128 | 3 / 564 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 1884 | 536 | 78.4% | −0.02R | 420 / 116 | 2 | 260 | 1086 | 536 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-10-13 17:57Z | SOL | BAD | 3m | short | 107.12 / 107.57 / 106.31 | pending |
| 2026-10-13 17:37Z | BTC | WATCH | 5m | short | 83085.1 / 83229.2 / 82612.452 | open |
| 2026-10-13 17:27Z | ETH | WATCH | 3m | short | 2502.12 / 2507.7 / 2484.0408 | open |
| 2026-10-13 14:47Z | BTC | BAD | 1m | long | 83641.9 / 82788.75 / 83802.5 | open |
| 2026-10-13 14:07Z | SOL | WATCH | 3m | long | 107.32 / 106.53 / 108.663 | open |
| 2026-10-13 03:17Z | ETH | WATCH | 5m | long | 2493.49 / 2481.24 / 2545.43 | open |
| 2026-10-12 23:47Z | ETH | plan:conditional | 5m | short | 2454.17 / 2469.04 / 2388.99 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 755 | 245 | 192 | 52 | 2 | 78.7% | +0.04R | −0.29R | 0.32 | 6 | 23 |
| WATCH | 527 | 247 | 75 | 166 | 4 | 31.1% | +0.28R | −5.79R | 1.96 | 15 | 35 |
| GOOD | 1 | 1 | 1 | 0 | 0 | 100% | +2.87R | +2.53R | 1.9 | 0 | 89 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 522 | 243 | 73 | 165 | 4 | 30.7% | +0.26R | −5.88R | – | 15 | 35 |
| rr_below_min | 374 | 245 | 192 | 52 | 2 | 78.7% | +0.04R | −0.29R | 0.32 | 6 | 23 |
| chase | 233 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 148 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 5 | 4 | 2 | 1 | 0 | 66.7% | +1.63R | +1.34R | 1.96 | 1 | 57 |
| ready_flag_plan | 1 | 1 | 1 | 0 | 0 | 100% | +2.87R | +2.53R | 1.9 | 0 | 89 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 1 | 1 | 1 | 0 | 0 | 100% | +2.87R | +2.53R | 1.9 | 0 | 89 |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 2248 | 620 | 455 | 164 | 2 | 73.5% | −0.05R | −0.62R | 0.29 | 8 | 20 |
| WATCH | 1500 | 682 | 183 | 492 | 4 | 27.1% | +0.08R | −3.95R | 1.57 | 30 | 39 |
| GOOD | 7 | 7 | 3 | 4 | 0 | 42.9% | +0.60R | −1.65R | 1.25 | 3 | 4 |
| DATA_UNAVAILABLE | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 1486 | 672 | 181 | 485 | 4 | 27.2% | +0.08R | −3.95R | – | 30 | 39 |
| rr_below_min | 926 | 620 | 455 | 164 | 2 | 73.5% | −0.05R | −0.62R | 0.29 | 8 | 20 |
| chase | 682 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 640 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 14 | 10 | 2 | 7 | 0 | 22.2% | −0.12R | −3.88R | 1.57 | 7 | 57 |
| ready_flag_plan | 7 | 7 | 3 | 4 | 0 | 42.9% | +0.60R | −1.65R | 1.25 | 3 | 4 |
| missing_data:1m | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 1 | 1 | 1 | 0 | 0 | 100% | +2.51R | +1.22R | 0.53 | 0 | 11 |
| SOL | 1 | 1 | 1 | 0 | 0 | 100% | +2.87R | +2.53R | 1.9 | 0 | 89 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-10-13 | 143 | 1 | 55 | 87 | 1 | 1 | 1 | 0 | +2.87R |
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
| Live | 18 | 0.94 | 18 | 38.9% | +0.64R | −2.79R |
| NF | 1 | 0.05 | 1 | 100% | +2.87R | +2.53R |

n=18 over 19.25 d (engine 0, backfill 18). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 8670, gaps 33, DATA_UNAVAILABLE 3, mark drift |bps| median 1.4 / max 52.3, missing 1m candles 0.
