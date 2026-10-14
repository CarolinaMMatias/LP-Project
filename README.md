# Star Battle Solver — Prolog

Project developed for the **Lógica para Programação** (Logic for Programming) course at **Instituto Superior Técnico (IST)**.

---

## 🧩 About the Project

An automated logic puzzle solver for **Star Battle** implemented in **SWI-Prolog**.

### 🎯 Puzzle Rules:
* Played on an $N \times N$ grid (e.g., $9 \times 9$) divided into distinct regions.
* Place **exactly 2 stars** in every row, column, and region.
* **No two stars can touch**, even diagonally (all adjacent positions must be filled with dots).

---

## ⚙️ Implementation & Features

* **Board Representation**: Grid modeled as a list of lists using Prolog variables (`_`), stars (`e`), and dots (`p`).
* **Deductive Strategies**:
  * Line and region completion (`fecha/2`): fills remaining cells with dots when two stars are placed, or inserts stars when only valid spots remain.
  * Pattern detection (`aplicaPadroes/2`): identifies specific sequences (I-patterns and T-patterns) to place stars and dots.
* **Solver (`resolve/2`)**: Iteratively applies logical rules and heuristics until the board reaches a stable solution without brute-force search.

---

## 💻 Tech Stack
* SWI-Prolog
