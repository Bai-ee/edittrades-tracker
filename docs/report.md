# EditTrades call tracker report

Generated 2026-10-08 23:47Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 11.6).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 1 | 1 | 100% | +1.22R | +1.22R | – | 0 | 1 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 10.6).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 0 | – | – | – | – | 0 | 0 / 30 |

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 11.6).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 13).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −3.17% | −3.37% | 3 | 11 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 12.1).

| Equity now | Equity at start | Trades | Realized net | Kill/arm |
| --- | --- | --- | --- | --- |
| $521.30 | $523.01 | 0 | – | – |

Daily/weekly drawdown kill switch; Steady profile caps $150 size / 100x / $5 per trade / $25 per day / 1 open position.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Net-floor forward record (2.5R gross, net floor live), start 2026-09-27, ends 2026-10-11
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 12 / 14, plans scored 1 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| [NO SCORED CALLS YET] | 0 | – | 0 / 0 | 0 | – | 2026-10-08 23:47Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 100% | +2.51R | 1 / 0 | 0 | 0 | 0 | 1 / 0 | 1 | 0 | – | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 868 | 395 | 26.1% | −0.04R | 103 / 292 | 5 | 371 | 97 | 3 / 392 | – | – | – | FILTER CONFIRMED |
| BAD | 1356 | 368 | 77.5% | −0.03R | 285 / 83 | 11 | 173 | 804 | 368 / 0 | – | – | – | FILTER CONFIRMED |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-10-08 23:47Z | ETH | BAD | 1m | short | 2473.89 / 2484.28 / 2465.94 | pending |
| 2026-10-08 23:07Z | BTC | WATCH | 1m | short | 81809.4 / 81870 / 81676.686 | open |
| 2026-10-08 22:47Z | BTC | BAD | 5m | long | 81788.9 / 80954.65 / 81915 | open |
| 2026-10-08 21:47Z | ETH | BAD | 3m | long | 2475.41 / 2450.16 / 2486.77 | open |
| 2026-10-08 21:47Z | SOL | BAD | 3m | long | 110.1 / 108.98 / 111.1 | open |
| 2026-10-08 21:17Z | ETH | WATCH | 5m | long | 2474.19 / 2466.84 / 2498.739 | open |
| 2026-10-08 21:17Z | SOL | BAD | 3m | long | 109.86 / 108.74 / 110.78 | open |
| 2026-10-08 20:57Z | ETH | BAD | 5m | long | 2469.33 / 2444.14 / 2498.82 | open |
| 2026-10-08 20:57Z | SOL | BAD | 5m | long | 109.51 / 108.39 / 111.35 | open |
| 2026-10-08 20:47Z | ETH | BAD | 3m | long | 2469.33 / 2444.14 / 2489.21 | open |
| 2026-10-08 20:37Z | SOL | WATCH | 5m | long | 109.44 / 109.12 / 111.28 | open |
| 2026-10-08 20:27Z | SOL | plan:conditional | 5m | long | 109.31 / 108.2 / 112.36 | pending |
| 2026-10-08 20:27Z | SOL | WATCH | 5m | long | 109.31 / 108.2 / 112.36 | open |
| 2026-10-08 20:27Z | SOL | plan:null | 5m | long | 109.31 / 108.2 / 112.36 | open |
| 2026-10-08 20:17Z | SOL | BAD | 3m | long | 109.35 / 108.23 / 111.07 | open |
| 2026-10-08 20:07Z | BTC | BAD | 3m | long | 81754.4 / 80920.51 / 81915 | open |
| 2026-10-08 18:47Z | BTC | WATCH | 3m | long | 81492.7 / 81278.6 / 82522.521 | open |
| 2026-10-08 18:37Z | BTC | BAD | 1m | long | 81402.8 / 80572.49 / 81915 | open |
| 2026-10-08 17:07Z | SOL | plan:conditional | 1m | short | 107.39 / 107.84 / 105.87 | pending |
| 2026-10-08 13:47Z | SOL | plan:conditional | 5m | short | 111.99 / 112.8 / 109.95 | pending |
| 2026-10-08 13:07Z | SOL | plan:conditional | 3m | short | 112.27 / 112.74 / 110.98 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 815 | 246 | 179 | 57 | 11 | 75.9% | −0.04R | −0.37R | 0.32 | 6 | 22 |
| WATCH | 530 | 251 | 66 | 179 | 5 | 26.9% | −0.03R | −3.52R | 1.96 | 30 | 39 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 526 | 247 | 64 | 178 | 4 | 26.5% | −0.05R | −3.58R | – | 30 | 39 |
| rr_below_min | 360 | 246 | 179 | 57 | 11 | 75.9% | −0.04R | −0.37R | 0.32 | 6 | 22 |
| chase | 263 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| room_at_entry | 192 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 4 | 4 | 2 | 1 | 1 | 66.7% | +1.63R | +1.34R | 1.96 | 1 | 57 |

Ready plans by symbol:

_none yet_


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 1720 | 461 | 320 | 131 | 11 | 71% | −0.07R | −0.73R | 0.32 | 8 | 18 |
| WATCH | 1130 | 510 | 131 | 372 | 5 | 26% | −0.01R | −2.75R | 1.57 | 30 | 39 |
| GOOD | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |
| DATA_UNAVAILABLE | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 1117 | 500 | 129 | 365 | 4 | 26.1% | −0.00R | −2.73R | – | 30 | 39 |
| rr_below_min | 680 | 461 | 320 | 131 | 11 | 71% | −0.07R | −0.73R | 0.32 | 8 | 18 |
| room_at_entry | 523 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 517 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 13 | 10 | 2 | 7 | 1 | 22.2% | −0.12R | −3.88R | 1.57 | 7 | 57 |
| ready_flag_plan | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |
| missing_data:1m | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 1 | 1 | 1 | 0 | 0 | 100% | +2.51R | +1.22R | 0.53 | 0 | 11 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-10-08 | 185 | 0 | 76 | 109 | 0 | 0 | 0 | 0 | – |
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
| Live | 17 | 1.17 | 17 | 35.3% | +0.51R | −3.10R |
| NF | 0 | 0 | 0 | – | – | – |

n=17 over 14.49 d (engine 0, backfill 17). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


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

Captures 6570, gaps 33, DATA_UNAVAILABLE 3, mark drift |bps| median 1.4 / max 52.3, missing 1m candles 0.
