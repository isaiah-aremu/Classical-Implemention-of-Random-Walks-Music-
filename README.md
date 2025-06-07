**Classical Random Walks for Music Generation — Two Musicians, Two Approaches**

**Overview**
This repository contains Python implementations of classical random walk algorithms for music generation. It focuses on two musicians modeled with distinct musical spaces and two different approaches.

Each musician’s musical space is represented as a directed graph of nodes, where each node encodes a tuple of (note, intensity, duration). The random walk simulates the probabilistic transitions between these musical states, following the Markov property to generate sequences of musical tuples.

**Two Approaches:**
1. **Approach 1:** Random walk graphs constructed separately for each musical attribute (notes, durations, intensities), modeling musician-specific preferences and styles.

2. **Approach 2:** Random walk on the whole tuple space, i.e., nodes correspond to complete tuples combining note, intensity, and duration, allowing more integrated musical transitions.

Both approaches use row-stochastic transition matrices to enforce proper probability distributions and ensure at least two outgoing edges per node for diversity.

**Motivation**
This work explores classical random walks as a probabilistic foundation for generative music, capturing multiple musicians' musical variability and stylistic preferences. Approach 1 emphasizes modular control over individual musical parameters, while Approach 2 offers holistic state transitions. Together, they provide complementary perspectives on stochastic musical composition.

This foundation supports further work on quantum-inspired music generation, where quantum walks extend these models with superposition and interference, offering richer expressive potential.
