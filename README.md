# Computational Complexity of Puzzles and Games

This repository contains a [document](GamesAndPuzzles/main.pdf) exploring the computational complexity of various puzzles and games. 

## Overview

The project examines the complexity of several well-known puzzles and games, analyzing their generalized versions for arbitrary sizes. It discusses the complexity classes to which these generalized versions belong, such as **NP**, **PSPACE**, and **EXP**.  A proof of **NP**-completeness for a specific type of puzzle known as "cryptarithms" is also presented.

## Included Puzzles and Games

The document discusses the complexity of the following:

* **Chess:**  Classic chess is finite, but the generalized *n* x *n* version is **PSPACE**-complete with the 50-move rule, and **EXP**-complete without it.
* **Reversi (Othello):** The generalized *n* x *n* version is **PSPACE**-complete.
* **15 Puzzle:** While checking the solvability of a given configuration is in **P**, finding a solution with the minimum number of moves is **NP**-complete.
* **Nonograms (Japanese Crosswords):**  **NP**-complete.
* **Go:** The generalized *n* x *n* version is **PSPACE**-complete. A variant with the *ko* rule (forbidding immediate repetition of a previous position) is **EXP**-complete.
* **Cryptarithms:** Generalized to *n*-ary bases, they are **NP**-complete.  The document includes a detailed proof of this.

## Proof of NP-Completeness for Cryptarithms

The document features a proof demonstrating that the language of solvable cryptarithms (CRYPTA) is **NP**-complete. It shows membership in **NP** and then provides a reduction from 3-SAT to CRYPTA.  The proof constructs a cryptarithm from a 3-SAT formula, demonstrating that a solution to the cryptarithm exists if and only if the 3-SAT formula is satisfiable.  The proof leverages specific number-theoretic properties and carefully constructed gadgets within the cryptarithm to ensure the reduction holds.
