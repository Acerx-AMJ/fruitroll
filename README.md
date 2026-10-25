# Fruitroll
Fruitroll is a fruit-themed CLI slot machine with zero dependencies for destroying productivity. It contains 7 fruits with different roll chances, crit multipliers and a ton of different combos and multipliers. It does not use real money.

## Building
Fruitroll uses no dependencies and can be built using CMake:
```bash
cmake -B build
cmake --build build
```
The executable will be located at `build/fruitroll`. Or build using your favorite compiler:
```bash
g++ -std=c++11 -Iinclude src/*.cpp -o fruitroll
```

## Usage
```bash
./fruitroll [arguments]
```
Arguments:
- `--help`             Display arguments.
- `--version`          Display current version.
- `--info`             Display detailed info.
- `--log-roll`         Enable roll RNG value logging.
- `--log-crit`         Enable crit RNG value logging.
- `--verbose`          Enable roll and crit RNG value logging.
- `--silent`           Completely disable delays and ASCII art.
- `--mute`             Only output final result with no delay.
- `--no-art`           Replace ASCII art with fruit names.
- `--repeat=<value>`   Repeat game `<value>` times.
- `--delay=<value>`    Set all delays to `<value>`ms.
- `--stop-on=<value>`  Force stop the game when jackpot is equal or bigger than `<value>`.
- `--seed=<value>`     Use a fixed RNG seed.

## Credits
This project was made by Daniel Vishnevsky and is licensed under MIT License. It was made in July of 2025 and got published on October 2026 as an effort to make all of my projects open-source.
