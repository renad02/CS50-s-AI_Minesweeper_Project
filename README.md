# CS50's AI Minesweeper Project

This project implements a playable Minesweeper game along with a reasoning-based AI that learns which cells are safe and which are mines by building and updating a logical knowledge base.

The core idea:

- Every revealed number like “2” around a cell is a constraint about nearby hidden cells.

- The AI collects these constraints as sentences and uses set logic (subset reasoning) to infer new safe cells and mines.

- If no safe move is provable, it falls back to a probabilistic move with the lowest estimated risk.
