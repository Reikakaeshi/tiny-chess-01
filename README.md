# tiny-chess-01

A tiny Python chess engine squeezed into 4,096 bytes.

It searches on a 0x88 board with alpha-beta pruning, a fixed node budget, a transposition table, and quiescence search. A small book of opening lines steers the early game before the search takes over.

Version 56 breaks the last practice draw: a fresh alapin book line turns the game against the strongest practice opponent into a win by checkmate.

Across the three practice trials it averages Elo 2,011 — seventeen wins, one draw, no losses. The trials score 1,809, then 2,112 at the cap twice. The single remaining draw is the philidor defence.

Run it with Python 3 under the kit's local harness: `python3 main.py`. The program is deterministic and reads nothing beyond its own bytes. No network, no clock, no files outside the program itself.

## Practice trials

Practice trials scored 1,809 in trial 0 and reached the 2,112 cap in trials 1 and 2, with seventeen wins, one draw, and no losses across all three trials.
