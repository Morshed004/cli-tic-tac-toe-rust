# rust_learn

## Overview
A small command‑line Tic‑Tac‑Toe game written in Rust. The program lets two players take turns entering row and column numbers to place their marks on a 3×3 board. It detects wins, draws, and prompts for valid moves.

## Features
- Two‑player turn‑based gameplay
- Input validation (row/column must be within bounds and cell must be empty)
- Automatic win detection for rows, columns, and diagonals
- Draw detection when the board is full with no winner
- Simple console output for board state and prompts

## Tech Stack
- **Language:** Rust (edition 2024)
- **Build tool:** Cargo
- **Standard library:** `std::io`, `std::char`, array handling
- **Dependencies:** None (pure standard library)

## Installation
1. Install a recent Rust toolchain (rustup) if you do not have it already.
2. Clone the repository:
   ```bash
   git clone https://github.com/Morshed004/cli-tic-tac-toe-rust.git
   cd rust_learn
   ```
3. Build the project:
   ```bash
   cargo build --release
   ```
   The binary will be placed in `target/release/rust_learn`.

## Usage
Run the compiled binary:
```bash
./target/release/rust_learn
```
The program will display the board and prompt the current player (`X` or `O`) for a row and column. Follow the on‑screen instructions until a win or a draw occurs.

## Project Structure
```
rust_learn/
├─ Cargo.toml          # Package metadata, edition 2024, no dependencies
├─ Cargo.lock          # Generated lock file
├─ src/
│  └─ main.rs         # Implementation of the game logic
├─ .gitignore          # Excludes the `target/` directory
└─ .codereadmeignore   # Git metadata ignored by the README generator
```

## Configuration
No environment variables or configuration files are required for the project. All settings are hard‑coded in the source (board size, player symbols).

## Notes
- The board size is fixed at 3×3; changing it would require code modifications.
- Input is read from standard input; invalid entries trigger a reprompt.
- The program uses only the Rust standard library, so no additional crates are needed.
