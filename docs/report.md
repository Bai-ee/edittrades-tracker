# EditTrades call tracker report

Generated 2026-10-18 14:27Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 21.2).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 4 | 4 | 2 | 50% | +0.27R | −0.06R | −0.70R | 2.67 | 4 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 20.3).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 21.2).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 22.6).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −4.01% | −9.89% | 5 | 21 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 21.7).

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
- Progress: day 14 / 14, plans scored 4 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.29R | 3 | 33.3% | 3 / 3 | 2 | +2.87R | 2026-10-18 14:27Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 4 | 4 | 50% | +0.84R | 2 / 2 | 0 | 0 | 0 | 4 / 0 | 1 | 3 | – | [4 SCORED · TOO FEW TO JUDGE] |
| WATCH | 1591 | 730 | 27.4% | +0.07R | 200 / 530 | 1 | 694 | 166 | 3 / 727 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| BAD | 2421 | 700 | 75.7% | −0.04R | 530 / 170 | 2 | 328 | 1391 | 700 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-10-18 14:27Z | SOL | BAD | 5m | short | 102.55 / 103.14 / 101.7 | pending |
| 2026-10-18 14:17Z | BTC | BAD | 5m | short | 81290 / 81631.42 / 81119.1 | open |
| 2026-10-18 13:57Z | SOL | WATCH | 5m | short | 102.64 / 103.14 / 100.67 | open |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 797 | 237 | 166 | 69 | 2 | 70.6% | −0.08R | −0.41R | 0.33 | 6 | 15 |
| WATCH | 528 | 251 | 76 | 173 | 1 | 30.5% | +0.21R | −1.69R | – | 17 | 37 |
| GOOD | 3 | 3 | 1 | 2 | 0 | 33.3% | +0.29R | −0.04R | 2.14 | 2 | 89 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 527 | 251 | 76 | 173 | 1 | 30.5% | +0.21R | −1.69R | – | 17 | 37 |
| rr_below_min | 348 | 237 | 166 | 69 | 2 | 70.6% | −0.08R | −0.41R | 0.33 | 6 | 15 |
| chase | 250 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 199 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| ready_flag_plan | 3 | 3 | 1 | 2 | 0 | 33.3% | +0.29R | −0.04R | 2.14 | 2 | 89 |
| entry_condition | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 2 | 2 | 1 | 1 | 0 | 50% | +0.93R | +0.60R | 2.17 | 1 | 89 |
| ETH | 1 | 1 | 0 | 1 | 0 | 0% | −1.00R | −1.33R | 2.08 | 1 | – |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 2785 | 785 | 565 | 218 | 2 | 72.2% | −0.06R | −0.58R | 0.31 | 8 | 19 |
| WATCH | 1853 | 843 | 228 | 610 | 1 | 27.2% | +0.08R | −3.58R | 1.57 | 30 | 39 |
| GOOD | 9 | 9 | 3 | 6 | 0 | 33.3% | +0.24R | −1.58R | 1.54 | 3 | 4 |
| DATA_UNAVAILABLE | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 1839 | 833 | 226 | 603 | 1 | 27.3% | +0.08R | −3.57R | – | 30 | 39 |
| rr_below_min | 1158 | 785 | 565 | 218 | 2 | 72.2% | −0.06R | −0.58R | 0.31 | 8 | 19 |
| chase | 847 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 780 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 14 | 10 | 2 | 7 | 0 | 22.2% | −0.12R | −3.88R | 1.57 | 7 | 57 |
| ready_flag_plan | 9 | 9 | 3 | 6 | 0 | 33.3% | +0.24R | −1.58R | 1.54 | 3 | 4 |
| missing_data:1m | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 2 | 2 | 1 | 1 | 0 | 50% | +0.76R | −0.06R | 1.3 | 1 | 11 |
| SOL | 2 | 2 | 1 | 1 | 0 | 50% | +0.93R | +0.60R | 2.17 | 1 | 89 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-10-18 | 125 | 0 | 48 | 77 | 0 | 0 | 0 | 0 | – |
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
| Live | 20 | 0.83 | 20 | 35% | +0.48R | −2.64R |
| NF | 3 | 0.12 | 3 | 33.3% | +0.29R | −0.04R |

n=20 over 24.1 d (engine 0, backfill 20). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 10851, gaps 33, DATA_UNAVAILABLE 3, mark drift |bps| median 1.4 / max 52.3, missing 1m candles 0.
