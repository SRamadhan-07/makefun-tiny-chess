# makefun-tiny-chess

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/SRamadhan-07/makefun-tiny-chess/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/SRamadhan-07/makefun-tiny-chess/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in under 4 KB of Python: negamax alpha-beta search with a transposition table, quiescence (captures plus check evasions), check extensions and null-move pruning, driven by fixed node budgets (75k/50k/28k by game phase) — never a clock — so every replay plays the same moves. Incremental material + piece-square evaluation with Zobrist hashing, a tapered king term, doubled-pawn penalties, and repetition / fifty-move draws scored inside the search. It plays through the env at MAKEFUN_ENV_URL (POST /game, /move, /resign), rebuilding its state from the served FEN each turn. Original code, written for this bounty; `main.py` is the kit-compressed form of the readable source.

## Run it

```sh
python3 -P -s main.py # with MAKEFUN_ENV_URL and MAKEFUN_PROMPT_FILE set (see the kit's RULES.txt)
```

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
