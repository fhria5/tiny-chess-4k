# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/fhria5/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/fhria5/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A compact chess engine in 4 KB of Python: 0x88 board, negamax alpha-beta with quiescence search, transposition table, principal-variation search, null-move pruning, futility pruning and history heuristic, with iterative deepening on a fixed node budget. It plays the make.fun tiny-chess-01 gauntlet through the HTTP environment. Practice Elo ~1364 (trial 0), above the sunfish 4K baseline (~1325).

## Practice

Trial 0 on the exact submitted config: Elo 1364, 3 wins / 1 draw / 2 losses, 80,000-node budget, about 1.6 s per move. Trials 1–2 ran an older 60,000-node config (Elo 1099 each) and are not representative of the submitted config.

## Run it

```sh
python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref={referral_code}&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
