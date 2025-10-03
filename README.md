# Chess-Engine-Self-Project

A small C++ **chess engine** that speaks the **UCI** protocol. It plays roughly at an **~1250 rating** (casual/rapid level). The aim is learning and fun-simple search and evaluation, not grandmaster strength.

## What it does (quickly)
- Reads/writes **UCI** commands (so it works in chess GUIs).
- Looks ahead a few moves with a basic **alpha–beta** search.
- Simple **evaluation**: material, piece activity, and king safety.
- A few sensible opening choices (nothing fancy).

## Files
- `engine.cpp` – main program (UCI loop + search/eval).
- `chess.hpp` – header used by the engine.
> Keep both files in the same folder.

## Build
**Linux/macOS**
```bash
g++ -std=c++17 -O2 engine.cpp -o chess_engine
# or
clang++ -std=c++17 -O2 engine.cpp -o chess_engine
