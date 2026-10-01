# EditTrades call tracker report

Generated 2026-10-01 13:07Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.


## Strategy scoreboard · each from its own start

_provisional; not evidence of an edge_


### Flag engine · net floor · LIVE · TRADABLE

Since 2026-09-27 (days live 4.2).

| Signals | Resolved | Wins | Win % | Net R mean | Net R median | Net R 90% LB | Max DD (R) | Toward 30 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 1 | 1 | 100% | +1.22R | +1.22R | – | 0 | 1 / 30 |

TP1 or stop from the flag plan’s own levels, stop floored at the net floor (max(0.5x ATR15m, 3x round-trip cost)), capped at 3% from entry.


### HTF-anchored entries · LIVE · TRADABLE

Since 2026-09-28 (days live 3.2).

[NO SIGNALS SINCE 2026-09-28]

TP1 or stop from the 1h swing (NF-floored, 3% scalp-capped); target from the last 1h impulse projected from that swing.


### RETEST 1H · PAPER

Since 2026-09-27 (days live 4.2).

[NO SIGNALS SINCE 2026-09-27]

A RETEST_1H_EXIT alert closes it on a structure break, else a 7-day hold cap.


### Spot EMA20 trend · PAPER

Since 2026-09-26 (days live 5.5).

| Paper equity | Buy & hold | Live flips | Days tracked |
| --- | --- | --- | --- |
| −1.09% | −1.39% | 0 | 4 |

Flips the coin to USDC when its daily close drops back below EMA20.


### Live wallet · Steady profile · WALLET

Since 2026-09-26 (days live 4.6).

| Equity now | Equity at start | Trades | Realized net | Kill/arm |
| --- | --- | --- | --- | --- |
| $522.42 | $523.01 | 0 | – | – |

Daily/weekly drawdown kill switch; Steady profile caps $150 size / 100x / $5 per trade / $25 per day / 1 open position.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Net-floor forward record (2.5R gross, net floor live), start 2026-09-27, ends 2026-10-11
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 5 / 14, plans scored 1 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +2.51R | 1 | 100% | 1 / 1 | 0 | +2.51R | 2026-10-01 13:07Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 1 | 1 | 100% | +2.51R | 1 / 0 | 0 | 0 | 0 | 1 / 0 | 1 | 0 | – | [1 SCORED · TOO FEW TO JUDGE] |
| WATCH | 308 | 142 | 24.7% | −0.05R | 35 / 107 | 0 | 130 | 36 | 0 / 142 | – | – | – | FILTER CONFIRMED |
| BAD | 486 | 121 | 81% | +0.01R | 98 / 23 | 0 | 53 | 312 | 121 / 0 | – | – | – | FILTER MAY BE BLOCKING WINNERS |
| DATA_UNAVAILABLE | 1 | 0 | – | – | 0 / 0 | 0 | 0 | 1 | 0 / 0 | – | – | – | [0 SCORED · TOO FEW TO JUDGE] |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

_none yet_


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 812 | 195 | 129 | 66 | 0 | 66.2% | −0.10R | −1.17R | 0.28 | 8 | 13 |
| WATCH | 539 | 236 | 60 | 175 | 0 | 25.5% | +0.04R | −2.02R | 1.06 | 24 | 41 |
| GOOD | 5 | 5 | 2 | 3 | 0 | 40% | +0.47R | −2.19R | 1.43 | 2 | 3 |
| DATA_UNAVAILABLE | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 530 | 230 | 60 | 169 | 0 | 26.2% | +0.06R | −1.90R | – | 24 | 41 |
| room_at_entry | 291 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 286 | 195 | 129 | 66 | 0 | 66.2% | −0.10R | −1.17R | 0.28 | 8 | 13 |
| chase | 235 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 9 | 6 | 0 | 6 | 0 | 0% | −1.00R | −6.49R | 1.06 | 6 | – |
| ready_flag_plan | 5 | 5 | 2 | 3 | 0 | 40% | +0.47R | −2.19R | 1.43 | 2 | 3 |
| missing_data:1m | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ETH | 1 | 1 | 1 | 0 | 0 | 100% | +2.51R | +1.22R | 0.53 | 0 | 11 |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 850 | 204 | 133 | 71 | 0 | 65.2% | −0.10R | −1.16R | 0.31 | 8 | 13 |
| WATCH | 570 | 251 | 63 | 187 | 0 | 25.2% | +0.02R | −1.98R | 1.06 | 24 | 40 |
| GOOD | 6 | 6 | 2 | 4 | 0 | 33.3% | +0.22R | −2.35R | 1.09 | 3 | 3 |
| DATA_UNAVAILABLE | 1 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 561 | 245 | 63 | 181 | 0 | 25.8% | +0.05R | −1.87R | – | 24 | 40 |
| room_at_entry | 304 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| rr_below_min | 302 | 204 | 133 | 71 | 0 | 65.2% | −0.10R | −1.16R | 0.31 | 8 | 13 |
| chase | 244 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 9 | 6 | 0 | 6 | 0 | 0% | −1.00R | −6.49R | 1.06 | 6 | – |
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
| 2026-10-01 | 100 | 0 | 38 | 62 | 0 | 0 | 0 | 0 | – |
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
| Live | 17 | 2.41 | 17 | 35.3% | +0.51R | −3.10R |
| NF | 0 | 0 | 0 | – | – | – |

n=17 over 7.05 d (engine 0, backfill 17). NF (live since 2026-09-27): the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Before 2026-09-27 (config 2026.09.24-5 and earlier) NF was a shadow comparator only, never traded; since config 2026.09.27-1 the floor is baked into the live plan itself, so Live IS the NF stop and the two columns converge going forward - historical divergence predates the cutover. Rows the engine could not source an NF verdict for are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation.


## RETEST 1H · paper

_provisional; not evidence of an edge_

[NO RETEST 1H SIGNALS YET]


## HTF ENTRY · live

_provisional; not evidence of an edge_

[NO HTF ENTRY SIGNALS YET]


## Data health

_provisional; not evidence of an edge_

Captures 3303, gaps 21, DATA_UNAVAILABLE 3, mark drift |bps| median 1.6 / max 26.2, missing 1m candles 0.
