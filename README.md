# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine in 2,952 bytes of Python: full legal move generation
(castling, en passant, promotions), negamax search with alpha-beta
pruning, quiescence search over captures, MVV-LVA move ordering and
iterative deepening under a fixed 20,000-node budget (deterministic,
never clock-based). Evaluation is material plus compact positional
terms (pawn advancement, knight/bishop centrality, rook on the
seventh rank, king shelter). `main.py` is the whole engine, packed as
a zlib payload with its unpacker; it plays the make.fun gauntlet
through the env at MAKEFUN_ENV_URL.

## Run it

```sh
python3 main.py  # MAKEFUN_ENV_URL is set by the trial environment
```

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
