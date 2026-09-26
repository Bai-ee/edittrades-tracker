# EditTrades call tracker report

Generated 2026-09-26 20:37Z. R is gross, before fees and slippage. Not evidence of an edge. Scores the engine's calls against later closed candles.

## Testing phase

_provisional; not evidence of an edge_

- Status: RUNNING
- Phase: Phase 5 forward record (2.5R gross, net gate off), start 2026-09-24, ends 2026-10-08
- Thresholds frozen until 2026-10-08
- Target: 14 days / >= 30 scored plans
- Progress: day 3 / 14, plans scored 14 / 30
- Frozen during the window: no threshold tuning

## Summary

_provisional; not evidence of an edge_

| Expectancy 7d | Scored 7d | Win rate 7d | Fills 7d | Losing streak 7d | Avg win R 7d | Last capture |
| --- | --- | --- | --- | --- | --- | --- |
| +0.32R | 14 | 28.6% | 14 / 14 | 7 | +3.61R | 2026-09-26 20:37Z |


## Class check

_provisional; not evidence of an edge_

| Class | Calls | Scored | Win rate | Exp. (gross R) | TP1 / Stop | Open | Not filled | No levels | Levels from (plan / candidate) | Calls (1-min log) | Of which captured | Median GOOD window (min) | Verdict |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| GOOD | 14 | 14 | 28.6% | +0.32R | 4 / 10 | 0 | 0 | 0 | 14 / 0 | 12 | 5 | 4 | WORKING |
| WATCH | 220 | 88 | 19.3% | −0.13R | 17 / 71 | 6 | 109 | 17 | 4 / 84 | – | – | – | FILTER CONFIRMED |
| BAD | 309 | 72 | 41.7% | −0.28R | 30 / 42 | 1 | 41 | 195 | 72 / 0 | – | – | – | FILTER CONFIRMED |


WATCH and BAD are scored as if taken: entry at the flag breakout, stop at invalidation, TP1 at the measured move. Counterfactual only: never counted in the 30-plan target or the expectancy above.


GOOD calls come from the engine's 1-minute alert log since 2026-09-25; before that from 10-minute captures.


## Open calls

_provisional; not evidence of an edge_

| Called | Symbol | Call | TF | Dir | Entry / stop / TP1 | Status |
| --- | --- | --- | --- | --- | --- | --- |
| 2026-09-26 20:37Z | BTC | WATCH | 1m | long | 84080.7 / 84062.5 / 84185.35 | pending |
| 2026-09-26 20:37Z | ETH | WATCH | 1m | long | 2683.76 / 2683.09 / 2686.6879 | pending |
| 2026-09-26 20:27Z | ETH | BAD | 1m | long | 2682.71 / 2681.64 / 2684.32 | pending |
| 2026-09-26 20:27Z | SOL | WATCH | 5m | short | 120.72 / 121.26 / 120.1098 | pending |
| 2026-09-26 19:57Z | ETH | WATCH | 3m | short | 2681.64 / 2684.32 / 2677.2448 | open |
| 2026-09-26 18:27Z | SOL | WATCH | 5m | short | 121.22 / 121.56 / 120.4312 | open |
| 2026-09-26 18:11Z | BTC | WATCH | 5m | short | 84075.9 / 84177.23 / 83954.304 | open |
| 2026-09-26 08:27Z | ETH | plan:conditional | 1m | short | 2688.3 / 2689.36 / 2685.43 | pending |
| 2026-09-25 22:47Z | SOL | plan:conditional | 1m | long | 122.37 / 122.2 / 122.83 | pending |
| 2026-09-25 22:27Z | BTC | plan:conditional | 1m | long | 83949.3 / 83924.2 / 84042.1 | pending |


## Last 7d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 310 | 73 | 31 | 42 | 1 | 42.5% | −0.26R | −2.18R | 0.39 | 8 | 10 |
| WATCH | 223 | 94 | 17 | 73 | 6 | 18.9% | −0.15R | −2.62R | 1.06 | 24 | 35 |
| GOOD | 5 | 5 | 2 | 3 | 0 | 40% | +0.47R | −2.37R | 1.01 | 3 | 3 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 216 | 90 | 17 | 69 | 6 | 19.8% | −0.11R | −2.52R | – | 24 | 35 |
| rr_below_min | 115 | 73 | 31 | 42 | 1 | 42.5% | −0.26R | −2.18R | 0.39 | 8 | 10 |
| room_at_entry | 98 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 97 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 7 | 4 | 0 | 4 | 0 | 0% | −1.00R | −4.78R | 1.06 | 4 | – |
| ready_flag_plan | 5 | 5 | 2 | 3 | 0 | 40% | +0.47R | −2.37R | 1.01 | 3 | 3 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 8 | 8 | 0 | 8 | 0 | 0% | −1.00R | −2.60R | 1.59 | 8 | – |
| BTC | 3 | 3 | 2 | 1 | 0 | 66.7% | +1.45R | −2.84R | 0.07 | 1 | 3 |
| ETH | 3 | 3 | 2 | 1 | 0 | 66.7% | +2.71R | −6.68R | – | 1 | 5 |


## Last 30d

_provisional; not evidence of an edge_

By class:

| Class | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| BAD | 310 | 73 | 31 | 42 | 1 | 42.5% | −0.26R | −2.18R | 0.39 | 8 | 10 |
| WATCH | 223 | 94 | 17 | 73 | 6 | 18.9% | −0.15R | −2.62R | 1.06 | 24 | 35 |
| GOOD | 5 | 5 | 2 | 3 | 0 | 40% | +0.47R | −2.37R | 1.01 | 3 | 3 |

By reason:

| Reason | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| need_confirmed_flag_plan | 216 | 90 | 17 | 69 | 6 | 19.8% | −0.11R | −2.52R | – | 24 | 35 |
| rr_below_min | 115 | 73 | 31 | 42 | 1 | 42.5% | −0.26R | −2.18R | 0.39 | 8 | 10 |
| room_at_entry | 98 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| chase | 97 | 0 | 0 | 0 | 0 | – | – | – | – | 0 | – |
| entry_condition | 7 | 4 | 0 | 4 | 0 | 0% | −1.00R | −4.78R | 1.06 | 4 | – |
| ready_flag_plan | 5 | 5 | 2 | 3 | 0 | 40% | +0.47R | −2.37R | 1.01 | 3 | 3 |

Ready plans by symbol:

| Symbol | Calls | Fills | TP1 | Stop | Open | Win rate | Exp. (gross R) | Net exp. (net of fees) | Avg net R:R (plan) | Max loss streak | Median min to TP1 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SOL | 8 | 8 | 0 | 8 | 0 | 0% | −1.00R | −2.60R | 1.59 | 8 | – |
| BTC | 3 | 3 | 2 | 1 | 0 | 66.7% | +1.45R | −2.84R | 0.07 | 1 | 3 |
| ETH | 3 | 3 | 2 | 1 | 0 | 66.7% | +2.71R | −6.68R | – | 1 | 5 |


## By day

_provisional; not evidence of an edge_

| Day | Calls | GOOD | WATCH | BAD | Ready | Fills | TP1 | Stop | Exp. |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2026-09-26 | 171 | 2 | 72 | 97 | 2 | 2 | 2 | 0 | +2.67R |
| 2026-09-25 | 191 | 2 | 83 | 106 | 2 | 2 | 0 | 2 | −1.00R |
| 2026-09-24 | 172 | 1 | 65 | 106 | 1 | 1 | 0 | 1 | −1.00R |
| 2026-09-23 | 4 | 0 | 3 | 1 | 0 | 0 | 0 | 0 | – |


## Net floor shadow (NF, not traded)

_provisional; not evidence of an edge_

| Rule | Calls | Calls / day | Fills | Win rate | Exp. (gross R) | Net exp. (dir-cost) |
| --- | --- | --- | --- | --- | --- | --- |
| Live | 14 | 5.93 | 14 | 28.6% | +0.32R | −3.52R |
| NF | 0 | 0 | 0 | – | – | – |

n=14 over 2.36 d (engine 0, backfill 14). Shadow mode: the same live ready calls, scored twice - Live with the plan's own stop, NF with the stop floored at max(0.5 x ATR(15m), 3 x round-trip cost: 0.34 % long / 0.14 % short), TP1 unchanged, taken only when gross >= 2.5R and net >= 1.0R. Net R charges the direction cost once per trade. Calls before the engine published flagTradePlan.shadow.NF are backfilled here (ATR from stored 15m candles, filled at the live ready close) - an approximation. Never traded; never feeds any gate, class or alert.


## Data health

_provisional; not evidence of an edge_

Captures 1212, gaps 21, DATA_UNAVAILABLE 0, mark drift |bps| median 1.4 / max 20.1, missing 1m candles 0.
