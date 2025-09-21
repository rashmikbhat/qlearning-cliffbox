This project implements and evaluates a Reinforcement Learning (RL) algorithm to solve the Cliff Box Pushing grid-world game.

In this environment:
The agent (A) must push a box (B) into the goal (G).
Dangerous cliff cells (x) cause the agent or box to fall, ending the episode with a heavy penalty.
The environment is a fixed 6×14 grid.

The task is modeled as a Markov Decision Process (MDP) with:
State → position of agent + position of box
Action → {up, down, left, right}
Reward → step penalty, distance-based shaping, large penalty for falling, large reward for success

The objective is to train an RL agent that learns to safely push the box to the goal while avoiding cliffs.
