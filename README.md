# MDP
Going through the MDP project from TU_Delft



This link has the original notebook: https://digipedia.tudelft.nl/tutorial/markov-decision-processes/?tab=chapter-0

## 8th May 2025 
Single step decision making 
Sequential decision making

## 9th May 2025
Environment uncertainty  - stochastic environment

State uncertainty - due to partial/noisy environment

## 11th May 2025

MDP are elegant mathmatical framework for the first case (stochastic environments). Can be extended or generalized to cases when we have limited observabilities - this updated framework would be called POMDP.

A Markov chain is a random process/stochastic process) that satisfies the **Markov property**: *Given the current state, the next state is independent of the previous states. *

Mathematically, $\mathbb{P}(s_{t+1} | s_{t}) = \mathbb{P}(s_{t+1} | s_{t}, s_{t-1}, s_{t-2} \ldots)$, where $s_t$ denotes the state of the process at time instant $t$.
