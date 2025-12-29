# AISF-Bipedal-Walker
PPO with Action Smoothing for BipedalWalker-v3 locomotion.
Sophia Wang (sophiawang705@g.ucla.edu)

Project 
This repository contains a Proximal Policy Optimization (PPO) implementation for the BipedalWalker-v3 environment. The goal was to overcome the "limping" local optimum and policy collapse during high-torque training phases.

Results
Final Mean Reward: 271
Explained Variance: 0.955
Training Steps: 1,000,000

Techniques
SDE (State-Dependent Exploration): For consistent leg-swing momentum.
Action Smoothing ($\alpha=0.70$): To reduce joint chattering and stabilize the hull.
VecNormalize: To balance sensor input scales (LIDAR vs. Velocity).

## Repository Structure
- `AISF_Application.ipynb`: Main training and evaluation code.
- `BipedalWalker_Best.zip`: Saved model weights.
- `walker_performance.gif`: Video of the 271-reward run.
