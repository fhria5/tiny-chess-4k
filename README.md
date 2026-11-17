# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/fhria5/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/fhria5/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A compact chess engine in 4 KB of Python: 0x88 board, negamax alpha-beta with quiescence search, transposition table, principal-variation search, null-move pruning, futility pruning and history heuristic, with iterative deepening on a fixed node budget. It plays the make.fun tiny-chess-01 gauntlet through the HTTP environment. Practice Elo 1,279 (trial 0), above the 1,154 floor.

## Practice

Round-2 engine: 55,000-node budget (down from 80,000), with a speed fix — incremental Zobrist hash + pin-based legality filter. Official practice on the kit v19 env server: trial-0 Elo 1,279 (2W/2D/2L, mean think 1,422 ms, max 2,892 ms, wall 471 s); trial-1 Elo 1,191 (2W/1D/3L, mean 1,434 ms, max 2,683 ms, wall 575 s); trial-2 Elo 997 (1W/1D/4L, mean 1,490 ms, max 2,945 ms, wall 506 s); mean Elo ~1,156. Round 1 was rejected on practice_floor (site graded its practice 0): the old engine was too slow (mean 2,677 ms/move, 978 s wall) for the site's 1-CPU sandbox and the 1,800 s trial wall. The round-2 rebuild targets speed while staying above the 1,154 floor.

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=s2z411t3&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
