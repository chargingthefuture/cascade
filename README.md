# Cascade

A small, offline, single-file falling-blocks puzzle game — a Tetris-style knock-off.
No build step, no dependencies, no network. Just open it in a browser and play.

## Play

Open `index.html` in any modern browser (double-click it, or serve the folder).
Everything — game logic, rendering, styles — lives in that one file, so it works
fully offline.

## Controls

| Action        | Keys                      |
|---------------|---------------------------|
| Move          | `←` `→`                   |
| Rotate CW     | `↑` or `X`                |
| Rotate CCW    | `Z`                       |
| Soft drop     | `↓`                       |
| Hard drop     | `Space`                   |
| Hold piece    | `C`                       |
| Pause         | `P`                       |
| Start / retry | `Enter` or the Play button|

On touch devices, on-screen buttons appear, and you can also swipe the board:
drag left/right to move, drag down to soft-drop, tap to rotate, and a fast swipe
down hard-drops.

## Features

- Seven standard tetrominoes with **SRS rotation** and wall kicks
- **7-bag randomizer** so piece distribution stays fair
- **Ghost piece** showing where the current piece will land
- **Hold** queue and **Next** preview
- **Lock delay** so resting pieces can still be nudged
- Increasing **gravity** per level, standard line-clear **scoring**, and a
  **best score** saved in `localStorage`
- Responsive layout with mouse, keyboard, and touch support

## Scoring

| Lines cleared | Points (× level) |
|---------------|------------------|
| 1 (single)    | 100              |
| 2 (double)    | 300              |
| 3 (triple)    | 500              |
| 4 (Cascade!)  | 800              |

Soft drop scores 1 per cell, hard drop 2 per cell. You level up every 10 lines,
and each level the pieces fall faster.
