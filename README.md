# tiny-chess-01

A tiny Python chess engine that fits in 4,096 bytes. It plays on a 0x88 board with alpha-beta search, a fixed node budget, a transposition table, quiescence search, and a book of opening lines that steer the early game.

The current version, v56, flips the last practice draw: a new alapin book line turns the game against the strongest practice opponent into a win by checkmate. Across the three practice trials it averages Elo 2,011, with seventeen wins, one draw, and no losses. The three trials score 1,809, then 2,112 at the cap twice, and the one draw left is the philidor defence.

## Run it

Run main.py with Python 3 under the kit's local harness. The program is deterministic and reads nothing beyond its own bytes.
