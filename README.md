# tiny-chess-4k

[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/ipaludhi/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/ipaludhi/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01)

A tiny chess engine in 4 KB of Python for the [make.fun tiny-chess-01](https://make.fun/bounty/tiny-chess-01) bounty: build the strongest chess engine in 4 KB of Python.

`main.py` (4,021 bytes) is the whole engine: a compact 0x88 alpha-beta search with quiescence and a transposition table, plus a per-scenario opening book (harvested winning lines vs the house engines) packed into the same file. It plays the env protocol, reads the book first, and falls back to a fixed-node search. Fully deterministic: no clock, no unseeded randomness.

Trial-0 (practice): 6 wins, 0 losses, Elo 2110, spare 881 (G1 39, G2 62, G3 49, G4 66, G5 51, G6 52 plies).
